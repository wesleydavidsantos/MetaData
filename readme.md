# MetaData PHP Class

A small library for scraping all the meta data from a given URL, including open graph tags.

## Usage
	require_once('metadata.class.php');

	$metaData = MetaData::fetch('http://www.ted.com/talks/amanda_bennett_a_heroic_narrative_for_letting_go.html');
	
	// returns an associative array
	var_dump($metaData->tags());

	foreach ($metaData as $key => $value) {
		echo "$key => $value";
	}