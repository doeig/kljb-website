<script>
	import { A, Heading, Table, TableBody, TableBodyCell, TableBodyRow } from "flowbite-svelte";
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
	</div>
</section>
