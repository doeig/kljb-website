<script>
	import { A, P, Heading, List, Li } from "flowbite-svelte";

	const listing = [
		"Browsertyp und Browserversion",
		"verwendetes BetriebssystemReferrer URL",
		"Hostname des zugreifenden Rechners",
		"Uhrzeit der Serveranfrage"
	];
</script>

<Heading tag="h2" class="text-center mb-10">Datenschutzerklärung</Heading>
<Heading tag="h3" class="mb-4">Datenschutz</Heading>
<P class="mb-3">
	Die Betreiber dieser Seiten nehmen den Schutz Ihrer persönlichen Daten sehr ernst. Wir behandeln
	Ihre personenbezogenen Daten vertraulich und entsprechend der gesetzlichen Datenschutzvorschriften
	sowie dieser Datenschutzerklärung. Die Nutzung unserer Website ist in der Regel ohne Angabe
	personenbezogener Daten möglich. Soweit auf unseren Seiten personenbezogene Daten (beispielsweise
	Name, Anschrift oder E-Mail-Adressen) erhoben werden, erfolgt dies, soweit möglich, stets auf
	freiwilliger Basis. Diese Daten werden ohne Ihre ausdrückliche Zustimmung nicht an Dritte
	weitergegeben. Wir weisen darauf hin, dass die Datenübertragung im Internet (z.B. bei der
	Kommunikation per E-Mail) Sicherheitslücken aufweisen kann. Ein lückenloser Schutz der Daten vor
	dem Zugriff durch Dritte ist nicht möglich.
</P>
<Heading tag="h3" class="mb-4">Server-Log-Files</Heading>
<P class="mb-3">
	Der Provider der Seiten erhebt und speichert automatisch Informationen in so genannten Server-Log
	Files, die Ihr Browser automatisch an uns übermittelt. Dies sind:
</P>
<List class="mb-3 space-y-1 text-gray-900 dark:text-white">
	<Li>Test</Li>
	{#each listing as entry}
		<Li>{entry}</Li>
	{/each}
</List>
<P class="mb-3">
	Diese Daten sind nicht bestimmten Personen zuordenbar. Eine Zusammenführung dieser Daten mit
	anderen Datenquellen wird nicht vorgenommen. Wir behalten uns vor, diese Daten nachträglich zu
	prüfen, wenn uns konkrete Anhaltspunkte für eine rechtswidrige Nutzung bekannt werden.
</P>
<Heading tag="h3" class="mb-4">Facebook-Plugins (Like-Button)</Heading>
<P class="mb-3">
	Auf unseren Seiten sind Plugins des sozialen Netzwerks Facebook, Anbieter Facebook Inc., 1 Hacker
	Way, Menlo Park, California 94025, USA, integriert. Die Facebook-Plugins erkennen Sie an dem
	Facebook-Logo oder dem "Like-Button" ("Gefällt mir") auf unserer Seite. Eine Übersicht über die
	Facebook-Plugins finden Sie hier:
	<A color="text-kljb-green" href="https://developers.facebook.com/docs/plugins">
		https://developers.facebook.com/docs/plugins
	</A>. Wenn Sie unsere Seiten besuchen, wird über das Plugin eine direkte Verbindung zwischen Ihrem
	Browser und dem Facebook-Server hergestellt. Facebook erhält dadurch die Information, dass Sie mit
	Ihrer IP-Adresse unsere Seite besucht haben. Wenn Sie den Facebook "Like-Button" anklicken während
	Sie in Ihrem Facebook-Account eingeloggt sind, können Sie die Inhalte unserer Seiten auf Ihrem
	Facebook-Profil verlinken. Dadurch kann Facebook den Besuch unserer Seiten Ihrem Benutzerkonto
	zuordnen. Wir weisen darauf hin, dass wir als Anbieter der Seiten keine Kenntnis vom Inhalt der
	übermittelten Daten sowie deren Nutzung durch Facebook erhalten. Weitere Informationen hierzu
	finden Sie in der Datenschutzerklärung von Facebook unter
	<A color="text-kljb-green" href="https://de-de.facebook.com/policy.php">
		https://de-de.facebook.com/policy.php
	</A>. Wenn Sie nicht wünschen, dass Facebook den Besuch unserer Seiten Ihrem Facebook-Nutzerkonto
	zuordnen kann, loggen Sie sich bitte aus Ihrem Facebook-Benutzerkonto aus.
</P>
<Heading tag="h3" class="mb-4">Recht auf Auskunft, Löschung, Sperrung</Heading>
<P class="mb-3">
	Sie haben jederzeit das Recht auf unentgeltliche Auskunft über Ihre gespeicherten
	personenbezogenen Daten, deren Herkunft und Empfänger und den Zweck der Datenverarbeitung sowie
	ein Recht auf Berichtigung, Sperrung oder Löschung dieser Daten. Hierzu sowie zu weiteren Fragen
	zum Thema personenbezogene Daten können Sie sich jederzeit unter der im Impressum angegebenen
	Adresse anuns wenden.
</P>
<P>
	Quelle: <A color="text-kljb-green" href="https://www.e-recht24.de">https://www.e-recht24.de</A>
</P>
