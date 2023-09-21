<script>
	import { A, P, Heading, Table, TableBody, TableBodyCell, TableBodyRow } from "flowbite-svelte";

	const clubContact = {
		address: "KLJB Kläham-Oberergoldsbach e.V.<br/>Raiffeisenstraße 6<br/>84061 Ergoldsbach",
		mail: "info@kljb-klaeham.de",
		cellPhone: "0170 811 81 96"
	};
	const personContacts = [
		{ name: "Florian Sedlmeier", address: "Hauptstraße 29<br/>84098 Hohenthann", gender: "m" },
		{ name: "Kilian Prosch", address: "Unkofen 34<br/>84098 Hohenthann", gender: "m" },
		{
			name: "Lea Eichmeier",
			address: "Ludwig-Stiegler-Straße 1<br/>84061 Ergoldsbach",
			gender: "f"
		}
	];
</script>

<Heading tag="h2" class="text-center mb-10">Impressum</Heading>
<Heading tag="h3" class="mb-4">Angaben gemäß §5 TMG:</Heading>
<Table divClass="max-w-md mb-3">
	<TableBody>
		<TableBodyRow>
			<TableBodyCell class="italic">Anschrift:</TableBodyCell>
			<TableBodyCell>
				{@html clubContact.address}
			</TableBodyCell>
		</TableBodyRow>
		<TableBodyRow>
			<TableBodyCell class="italic">Mail:</TableBodyCell>
			<TableBodyCell>
				<A color="text-kljb-green" href={`mailto:${clubContact.mail}`}>{clubContact.mail}</A>
			</TableBodyCell>
		</TableBodyRow>
		<TableBodyRow>
			<TableBodyCell class="italic">Mobil:</TableBodyCell>
			<TableBodyCell>{clubContact.cellPhone}</TableBodyCell>
		</TableBodyRow>
	</TableBody>
</Table>
<Heading tag="h3" class="mb-3">Vertretungsberechtigte Personen:</Heading>
<Table divClass="max-w-md mb-3">
	<TableBody>
		{#each personContacts as person, i}
			<TableBodyRow>
				<TableBodyCell class="italic">
					{`${i + 1}. ${person.gender == "m" ? "Vorsitzender" : "Vorsitzende"}`}
				</TableBodyCell>
				<TableBodyCell>
					{person.name}
					<br />
					{@html person.address}
				</TableBodyCell>
			</TableBodyRow>
		{/each}
	</TableBody>
</Table>
<Heading tag="h3" class="mb-4">Vereinsregister:</Heading>
<Table divClass="max-w-md mb-3">
	<TableBody>
		<TableBodyRow>
			<TableBodyCell class="italic">Registergericht:</TableBodyCell>
			<TableBodyCell>Amtsgericht Landshut</TableBodyCell>
		</TableBodyRow>
		<TableBodyRow>
			<TableBodyCell class="italic">Registernummer:</TableBodyCell>
			<TableBodyCell>VR 200 699</TableBodyCell>
		</TableBodyRow>
	</TableBody>
</Table>
<Heading tag="h3" class="mb-4">Verantwortung für die Inhalte der Website:</Heading>
Sebastian Böhm:
<A class="mb-3" color="text-kljb-green" href="mailto:webmaster@kljb-klaeham.de">
	webmaster@kljb-klaeham.de
</A>
<Heading tag="h3" class="mb-4">Haftung für Inhalte</Heading>
<P class="mb-3">
	Als Diensteanbieter sind wir gemäß § 7 Abs.1 TMG für eigene Inhalte auf diesen Seiten nach den
	allgemeinen Gesetzen verantwortlich. Nach §§ 8 bis 10 TMG sind wir als Diensteanbieter jedoch
	nicht verpflichtet, übermittelte oder gespeicherte fremde Informationen zu überwachen oder nach
	Umständen zu forschen, die auf eine rechtswidrige Tätigkeit hinweisen. Verpflichtungen zur
	Entfernung oder Sperrung der Nutzung von Informationen nach den allgemeinen Gesetzen bleiben
	hiervon unberührt. Eine diesbezügliche Haftung ist jedoch erst ab dem Zeitpunkt der Kenntnis einer
	konkreten Rechtsverletzung möglich. Bei Bekanntwerden von entsprechenden Rechtsverletzungen werden
	wir diese Inhalte umgehend entfernen.
</P>

<Heading tag="h3" class="mb-4">Haftung für Links</Heading>
<P class="mb-3">
	Unser Angebot enthält Links zu externen Websites Dritter, auf deren Inhalte wir keinen Einfluss
	haben. Deshalb können wir für diese fremden Inhalte auch keine Gewähr übernehmen. Für die Inhalte
	der verlinkten Seiten ist stets der jeweilige Anbieter oder Betreiber der Seiten verantwortlich.
	Die verlinkten Seiten wurden zum Zeitpunkt der Verlinkung auf mögliche Rechtsverstöße überprüft.
	Rechtswidrige Inhalte waren zum Zeitpunkt der Verlinkung nicht erkennbar. Eine permanente
	inhaltliche Kontrolle der verlinkten Seiten ist jedoch ohne konkrete Anhaltspunkte einer
	Rechtsverletzung nicht zumutbar. Bei Bekanntwerden von Rechtsverletzungen werden wir derartige
	Links umgehend entfernen.
</P>

<Heading tag="h3" class="mb-4">Urheberrecht</Heading>
<P class="mb-3">
	Die durch die Seitenbetreiber erstellten Inhalte und Werke auf diesen Seiten unterliegen dem
	deutschen Urheberrecht. Die Vervielfältigung, Bearbeitung, Verbreitung und jede Art der Verwertung
	außerhalb der Grenzen des Urheberrechtes bedürfen der schriftlichen Zustimmung des jeweiligen
	Autors bzw. Erstellers. Downloads und Kopien dieser Seite sind nur für den privaten, nicht
	kommerziellen Gebrauch gestattet.
	<br />
	<br />
	Soweit die Inhalte auf dieser Seite nicht vom Betreiber erstellt wurden, werden die Urheberrechte Dritter
	beachtet. Insbesondere werden Inhalte Dritter als solche gekennzeichnet. Sollten Sie trotzdem auf eine
	Urheberrechtsverletzung aufmerksam werden, bitten wir um einen entsprechenden Hinweis. Bei Bekanntwerden
	von Rechtsverletzungen werden wir derartige Inhalte umgehend entfernen.
</P>

<P>
	Quelle: <A color="text-kljb-green" href="https://www.e-recht24.de/impressum-generator.html">
		https://www.e-recht24.de/impressum-generator.html
	</A>
</P>
