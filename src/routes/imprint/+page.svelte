<script>
	import { A, P, Heading, Table, TableBody, TableBodyCell, TableBodyRow } from "flowbite-svelte";
</script>

<section class="bg-white dark:bg-gray-900">
	<div class="py-8 px-4 mx-auto max-w-screen-xl lg:py-16 lg:px-6">
		<Heading tag="h1">Impressum</Heading>
		<Heading tag="h3">Angaben gemäß §5 TMG:</Heading>
		<Table divClass="max-w-md">
			<TableBody>
				<TableBodyRow>
					<TableBodyCell class="italic">Anschrift:</TableBodyCell>
					<TableBodyCell>
						KLJB Kläham-Oberergoldsbach e.V.
						<br />
						Raiffeisenstraße 6
						<br />
						84061 Ergoldsbach
					</TableBodyCell>
				</TableBodyRow>
				<TableBodyRow>
					<TableBodyCell class="italic">Mail:</TableBodyCell>
					<TableBodyCell>
						<A color="text-cyan-400" href="mailto:info@kljb-klaeham.de">info@kljb-klaeham.de</A>
					</TableBodyCell>
				</TableBodyRow>
				<TableBodyRow>
					<TableBodyCell class="italic">Mobil:</TableBodyCell>
					<TableBodyCell>0170 811 81 96</TableBodyCell>
				</TableBodyRow>
			</TableBody>
		</Table>
		<Heading tag="h3">Vertretungsberechtigte Personen:</Heading>
		<Table divClass="max-w-md">
			<TableBody>
				<TableBodyRow>
					<TableBodyCell class="italic">1. Vorsitzender</TableBodyCell>
					<TableBodyCell>
						Florian Sedlmeier
						<br />
						Hauptstraße 29
						<br />
						84098 Hohenthann
					</TableBodyCell>
				</TableBodyRow>
				<TableBodyRow>
					<TableBodyCell class="italic">2. Vorsitzender</TableBodyCell>
					<TableBodyCell>
						Kilian Prosch
						<br />
						Unkofen 34
						<br />
						84098 Hohenthann
					</TableBodyCell>
				</TableBodyRow>
				<TableBodyRow>
					<TableBodyCell class="italic">3. Vorsitzende</TableBodyCell>
					<TableBodyCell>
						Lea Eichmeier
						<br />
						Ludwig-Stiegler-Straße 1
						<br />
						84061 Ergoldsbach
					</TableBodyCell>
				</TableBodyRow>
			</TableBody>
		</Table>
		<Heading tag="h3">Vereinsregister:</Heading>
		<Table divClass="max-w-md">
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
		<Heading tag="h3">Verantwortung für die Inhalte der Website:</Heading>
		Sebastian Böhm:
		<A href="mailto:webmaster@kljb-klaeham.de">webmaster@kljb-klaeham.de</A>
		<Heading tag="h3" class="mb-4">Haftung für Inhalte</Heading>
		<P class="mb-4">
			Als Diensteanbieter sind wir gemäß § 7 Abs.1 TMG für eigene Inhalte auf diesen Seiten nach den
			allgemeinen Gesetzen verantwortlich. Nach §§ 8 bis 10 TMG sind wir als Diensteanbieter jedoch
			nicht verpflichtet, übermittelte oder gespeicherte fremde Informationen zu überwachen oder
			nach Umständen zu forschen, die auf eine rechtswidrige Tätigkeit hinweisen. Verpflichtungen
			zur Entfernung oder Sperrung der Nutzung von Informationen nach den allgemeinen Gesetzen
			bleiben hiervon unberührt. Eine diesbezügliche Haftung ist jedoch erst ab dem Zeitpunkt der
			Kenntnis einer konkreten Rechtsverletzung möglich. Bei Bekanntwerden von entsprechenden
			Rechtsverletzungen werden wir diese Inhalte umgehend entfernen.
		</P>

		<Heading tag="h3" class="mb-4">Haftung für Links</Heading>
		<P class="mb-4">
			Unser Angebot enthält Links zu externen Websites Dritter, auf deren Inhalte wir keinen
			Einfluss haben. Deshalb können wir für diese fremden Inhalte auch keine Gewähr übernehmen. Für
			die Inhalte der verlinkten Seiten ist stets der jeweilige Anbieter oder Betreiber der Seiten
			verantwortlich. Die verlinkten Seiten wurden zum Zeitpunkt der Verlinkung auf mögliche
			Rechtsverstöße überprüft. Rechtswidrige Inhalte waren zum Zeitpunkt der Verlinkung nicht
			erkennbar. Eine permanente inhaltliche Kontrolle der verlinkten Seiten ist jedoch ohne
			konkrete Anhaltspunkte einer Rechtsverletzung nicht zumutbar. Bei Bekanntwerden von
			Rechtsverletzungen werden wir derartige Links umgehend entfernen.
		</P>

		<Heading tag="h3" class="mb-4">Urheberrecht</Heading>
		<P class="mb-4">
			Die durch die Seitenbetreiber erstellten Inhalte und Werke auf diesen Seiten unterliegen dem
			deutschen Urheberrecht. Die Vervielfältigung, Bearbeitung, Verbreitung und jede Art der
			Verwertung außerhalb der Grenzen des Urheberrechtes bedürfen der schriftlichen Zustimmung des
			jeweiligen Autors bzw. Erstellers. Downloads und Kopien dieser Seite sind nur für den
			privaten, nicht kommerziellen Gebrauch gestattet.
			<br />
			<br />
			Soweit die Inhalte auf dieser Seite nicht vom Betreiber erstellt wurden, werden die Urheberrechte
			Dritter beachtet. Insbesondere werden Inhalte Dritter als solche gekennzeichnet. Sollten Sie trotzdem
			auf eine Urheberrechtsverletzung aufmerksam werden, bitten wir um einen entsprechenden Hinweis.
			Bei Bekanntwerden von Rechtsverletzungen werden wir derartige Inhalte umgehend entfernen.
		</P>

		<P>Quelle: <A>https://www.e-recht24.de/impressum-generator.html</A></P>
	</div>
</section>
