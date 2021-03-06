---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Citations
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework - List all citation styles
  x-api-slug: citationsstyles-get
  description: |-
    A paginated list of all standard citation styles available for rendering citations.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 citation styles. Each resource in the array is a separate citation syle and contains the full representation of the citation style object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    This request should never return an error.
    #### Filtering
    You can optionally request that the response only include citation styles that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/citations/styles/?filter[title]=open.

    Citation styles may be filtered by their `id`, `title`, `short-title`, and `summary`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/citationsstyles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/citationsstyles-get-openapi.md
- name: Open Science Framework - Retrieve a citation style
  x-api-slug: citationsstylesstyle-id-get
  description: |-
    Retrieves the details of a citation style.
    #### Returns
    Returns a JSON object with a `data` key containing the representation of the requested citation style, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/citationsstylesstyle-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/citationsstylesstyle-id-get-openapi.md
- name: Open Science Framework - List all citation styles
  x-api-slug: registrationsregistration-idcitations-get
  description: |-
    A paginated list of the registration's alternative citation styles

    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 citation styles. Each resource in the array is a separate citation styles object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include citation styles that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/citations/?filter[title]=open.

    Citation styles may be filtered by their `id`, `title`, `short-title`, and `summary`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/registrationsregistration-idcitations-get-openapi.md
- name: Open Science Framework - Retrieve a citation
  x-api-slug: registrationsregistration-idcitationscitation-id-get
  description: |-
    Retrieves the citation style details for a registration, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the citation style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/registrationsregistration-idcitationscitation-id-get-openapi.md
- name: Open Science Framework - Retrieve citation details
  x-api-slug: nodesnode-idcitation-get
  description: |-
    The citation details for a node, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the node citation.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/nodesnode-idcitation-get-openapi.md
- name: Open Science Framework - Retrieve a styled citation
  x-api-slug: nodesnode-idcitationstyle-id-get
  description: |-
    The citation for a node in a specific style.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the node citation, in the requested style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/nodesnode-idcitationstyle-id-get-openapi.md
- name: Open Science Framework - Retrieve citation details
  x-api-slug: preprintspreprint-idcitation-get
  description: |-
    The citation details for a preprint, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the preprint citation.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/preprintspreprint-idcitation-get-openapi.md
- name: Open Science Framework - Retrieve a styled citation
  x-api-slug: preprintspreprint-idcitationstyle-id-get
  description: |-
    The citation for a preprint in a specific style.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the preprint citation, in the requested style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/preprintspreprint-idcitationstyle-id-get-openapi.md
- name: Open Science Framework - Retrieve a citation
  x-api-slug: registrationsregistration-idcitationscitation-id-get
  description: |-
    Retrieves the citation style details for a registration, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the citation style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/registrationsregistration-idcitationscitation-id-get-openapi.md
- name: Open Science Framework - Retrieve citation details
  x-api-slug: nodesnode-idcitation-get
  description: |-
    The citation details for a node, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the node citation.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/nodesnode-idcitation-get-openapi.md
- name: Open Science Framework - Retrieve a styled citation
  x-api-slug: nodesnode-idcitationstyle-id-get
  description: |-
    The citation for a node in a specific style.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the node citation, in the requested style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/nodesnode-idcitationstyle-id-get-openapi.md
- name: Open Science Framework - Retrieve citation details
  x-api-slug: preprintspreprint-idcitation-get
  description: |-
    The citation details for a preprint, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the preprint citation.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/preprintspreprint-idcitation-get-openapi.md
- name: Open Science Framework - Retrieve a styled citation
  x-api-slug: preprintspreprint-idcitationstyle-id-get
  description: |-
    The citation for a preprint in a specific style.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the preprint citation, in the requested style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/preprintspreprint-idcitationstyle-id-get-openapi.md
- name: Open Science Framework - Retrieve a citation
  x-api-slug: registrationsregistration-idcitationscitation-id-get
  description: |-
    Retrieves the citation style details for a registration, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the citation style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/registrationsregistration-idcitationscitation-id-get-openapi.md
- name: Open Science Framework - Retrieve a citation
  x-api-slug: registrationsregistration-idcitationscitation-id-get
  description: |-
    Retrieves the citation style details for a registration, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the citation style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/registrationsregistration-idcitationscitation-id-get-openapi.md
- name: Open Science Framework - Retrieve a styled citation
  x-api-slug: preprintspreprint-idcitationstyle-id-get
  description: |-
    The citation for a preprint in a specific style.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the preprint citation, in the requested style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/preprintspreprint-idcitationstyle-id-get-openapi.md
- name: Open Science Framework - Retrieve citation details
  x-api-slug: preprintspreprint-idcitation-get
  description: |-
    The citation details for a preprint, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the preprint citation.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/preprintspreprint-idcitation-get-openapi.md
- name: Open Science Framework - Retrieve a styled citation
  x-api-slug: nodesnode-idcitationstyle-id-get
  description: |-
    The citation for a node in a specific style.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the node citation, in the requested style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/nodesnode-idcitationstyle-id-get-openapi.md
- name: Open Science Framework - Retrieve citation details
  x-api-slug: nodesnode-idcitation-get
  description: |-
    The citation details for a node, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the node citation.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/citations/master/_listings/open-science-framework/nodesnode-idcitation-get-openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-api-gallery
  url: http://open.fintech.api.gallery.streamdata.io
- type: x-api-stack
  url: http://open.science.framework.stack.network
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---