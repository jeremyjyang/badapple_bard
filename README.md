# `UNM_BIOCOMP_BARD` <img align="right" src="/project/doc/images/bard_logo.png" height="120">

_(Mavenization in progress. Need separate [JW]ARs, e.g. `bardplugin_badapple`, for
each plugin and `bard_util` JAR artifact.)_

Badapple promiscuity plugin developed for the BARD project, and more.

For info on BARD, see <http://bard.nih.gov/>.

## Dependencies

* `unm_biocomp_badapple`, `unm_biocomp_hscaf`, `unm_biocomp_db`, `unm_biocomp_util` 
* <https://github.com/ncats/bard>
* N.B.: NCATS libs depend on ChemAxon JChem 5.8.3. Follow their build instructions.

```
ant plugins
```

### Maven configuration

* The BARD API JAR must be built and installed locally.

```
mvn install:install-file -Dfile=bardplugin.jar -DgroupId=gov.nih.ncats -DartifactId=bardplugin -Dversion=1.0-SNAPSHOT -Dpackaging=jar -DlocalRepositoryPath=/home/www/htdocs/.m2/
```

## Compilation

```
mvn clean install
```

## Usage

## Deployment

## References

* BioAssay Research Database (BARD): chemical biology and probe-development enabled by
structured metadata and result types, Howe, et al., Nucleic Acids Res. 2015 Jan;
43:D1163-70. DOI: 10.1093/nar/gku1244, <http://www.ncbi.nlm.nih.gov/pubmed/25477388>.
