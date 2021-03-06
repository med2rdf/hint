# HiNT

RDF Converter for HiNT

## Downloading data
Download data from the following web site.

    http://hint.yulab.org/download/

Store the source file(tsv) to be converted in the following directory.

    data_h

![image](https://github.com/med2rdf/document/blob/master/hint_file_download.png)

## Cinfiguration
Edit the following definition file.

    tsv2rdf_hint.json


```
{
	"organism":{
		"HomoSapiens":{
			"binary_all":"HomoSapiens_binary_all.txt",
			"binary_hq":"HomoSapiens_binary_hq.txt",
			"cocomp_all":"HomoSapiens_cocomp_all.txt",
			"cocomp_hq":"HomoSapiens_cocomp_hq.txt"
		},
		"ArabidopsisThaliana":{
			"binary_all":"ArabidopsisThaliana_binary_all.txt",
			"binary_hq":"ArabidopsisThaliana_binary_hq.txt",
			"cocomp_all":"ArabidopsisThaliana_cocomp_all.txt",
			"cocomp_hq":"ArabidopsisThaliana_cocomp_hq.txt"
		},
		"BacillusSubtilisSubspSubtilisStr168":{
			"binary_all":"BacillusSubtilisSubspSubtilisStr168_binary_all.txt",
			"binary_hq":"BacillusSubtilisSubspSubtilisStr168_binary_hq.txt",
			"cocomp_all":"BacillusSubtilisSubspSubtilisStr168_cocomp_all.txt",
			"cocomp_hq":"BacillusSubtilisSubspSubtilisStr168_cocomp_hq.txt"
		},
		"BosTaurus":{
			"binary_all":"BosTaurus_binary_all.txt",
			"binary_hq":"BosTaurus_binary_hq.txt",
			"cocomp_all":"BosTaurus_cocomp_all.txt",
			"cocomp_hq":"BosTaurus_cocomp_hq.txt"
		},
		"CaenorhabditisElegans":{
			"binary_all":"CaenorhabditisElegans_binary_all.txt",
			"binary_hq":"CaenorhabditisElegans_binary_hq.txt",
			"cocomp_all":"CaenorhabditisElegans_cocomp_all.txt",
			"cocomp_hq":"CaenorhabditisElegans_cocomp_hq.txt"
		},
		"DrosophilaMelanogaster":{
			"binary_all":"DrosophilaMelanogaster_binary_all.txt",
			"binary_hq":"DrosophilaMelanogaster_binary_hq.txt",
			"cocomp_all":"DrosophilaMelanogaster_cocomp_all.txt",
			"cocomp_hq":"DrosophilaMelanogaster_cocomp_hq.txt"
		},
		"EscherichiaColiK12":{
			"binary_all":"EscherichiaColiK12_binary_all.txt",
			"binary_hq":"EscherichiaColiK12_binary_hq.txt",
			"cocomp_all":"EscherichiaColiK12_cocomp_all.txt",
			"cocomp_hq":"EscherichiaColiK12_cocomp_hq.txt"
		},
		"MusMusculus":{
			"binary_all":"MusMusculus_binary_all.txt",
			"binary_hq":"MusMusculus_binary_hq.txt",
			"cocomp_all":"MusMusculus_cocomp_all.txt",
			"cocomp_hq":"MusMusculus_cocomp_hq.txt"
		},
		"OryzaSativa":{
			"binary_all":"OryzaSativa_binary_all.txt",
			"binary_hq":"OryzaSativa_binary_hq.txt",
			"cocomp_all":"OryzaSativa_cocomp_all.txt"
		},
		"RattusNorvegicus":{
			"binary_all":"RattusNorvegicus_binary_all.txt",
			"binary_hq":"RattusNorvegicus_binary_hq.txt",
			"cocomp_all":"RattusNorvegicus_cocomp_all.txt",
			"cocomp_hq":"RattusNorvegicus_cocomp_hq.txt"
		},
		"SaccharomycesCerevisiaeS288C":{
			"binary_all":"SaccharomycesCerevisiaeS288C_binary_all.txt",
			"binary_hq":"SaccharomycesCerevisiaeS288C_binary_hq.txt",
			"cocomp_all":"SaccharomycesCerevisiaeS288C_cocomp_all.txt",
			"cocomp_hq":"SaccharomycesCerevisiaeS288C_cocomp_hq.txt"
		},
		"SchizosaccharomycesPombe972H":{
			"binary_all":"SchizosaccharomycesPombe972H_binary_all.txt",
			"binary_hq":"SchizosaccharomycesPombe972H_binary_hq.txt",
			"cocomp_all":"SchizosaccharomycesPombe972H_cocomp_all.txt",
			"cocomp_hq":"SchizosaccharomycesPombe972H_cocomp_hq.txt"
		}
	},
	"template":{
		"prefix":"templ_hint.ttl.prefix",
		"body":"templ_hint.ttl",
		"evidence":"templ_hint.ttl.evi"
	},
	"output_file":"hint_sample.ttl",
	"data_path":"data_h"

}
```

## Usage

        $ ./tsv2rdf_hint.sh
