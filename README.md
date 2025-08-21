# FHIR examples JSON

FHIR, pronounced "fire," stands for Fast Healthcare Interoperability Resources. FHIR is standard for exchanging healthcare information between different systems, designed to be flexible and easy to implement. It uses modern web technologies like RESTful APIs and JSON, XML, or RDF for data representation.

<https://www.hl7.org/>

This repository contains the worldwide-compatible FHIR examples JSON files.

<https://www.hl7.org/fhir/downloads.html>

This is the master set of worldwide-compatible files that should be the
first choice whenever generating any implementation artifacts that you want to
work as a baseline across all worldwide HL7 FHIR implementations, extensions,
derivations, and the like.

If you're specifically interested in HL7 FHIR for GIG Cymru NHS Wales, then see this:

<https://simplifier.net/guide/fhir-standards-wales-implementation-guide/Home>

## Do it yourself

Here's how you can create this repository from scratch:

```sh
mkdir fhir-specifications-json && cd $_
```

Download the HL7 FHIR JSON definitions, examples, and validations:

```sh
curl -sSSO https://www.hl7.org/fhir/examples-json.zip
unzip -d fhir-examples-json examples-json.zip && rm $_
```

Because there are so many files, we choose to move files into subdirectories by using a custom shell script:

Run:

```sh
bin/move-files-into-subdirectories
```
