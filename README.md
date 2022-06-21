# Insomnia-Findings-SBOM
Contains sample REST API calls for findings and to create an agent SCA SBOM

Tim Jarret has created a <a href="https://veracode.atlassian.net/wiki/spaces/~TJarrett/pages/6791918/Accessing+Veracode+APIs+with+Insomnia">Confluence page </a> describing how to enable HMAC authentication and how to use Insomnia to send GET requests to Veracode's APIs.  Please follow the steps, described there, to not only set up authentication but also to gain a basic understanding of how to install and use Insomnia.

After following the steps outlined in Tim's document, you can then import this repository as an Insomnia Collection.  The steps to create an SBOM are documented within the description of each of the GET requests that are required to generate an SBOM.  There are a total of 3 GET requests that must be used and they should be sent in this order:
<ol><li>1-agentSbomWsGuid</li><li>2-agentSbomProjGuid</li><li>3-agentSbomCreate</li></ol>

The results will be the generation of an agent-SCA SBOM in CycloneDx format

There are also REST API calls to create a Collection.
