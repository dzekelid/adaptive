---
name: VMWare
x-slug: vmware
description: At VMware, we believe that software has the power to unlock new opportunities
  for people and our planet. We look beyond the barriers of compromise to engineer
  new ways to make technologies work together seamlessly. Our software forms a digital
  foundation that powers the apps, services and experiences that are transforming
  the world.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Adaptive
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/adaptive/master/_listings/vmware/apis.md
specificationVersion: "0.14"
apis:
- name: vRealize Operations 6 - Get Agent Status on Upgrade
  x-api-slug: adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get
  description: Need agent ID (token)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/adaptive/master/_listings/vmware/adapterkindsep-ops-adapterresourcekindsep-ops-agentresources-get-openapi.md
- name: vRealize Operations 6 - Get An Adapter Instance(s) of Type (Kind)
  x-api-slug: adapters-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/adaptive/master/_listings/vmware/adapters-get-openapi.md
- name: vRealize Operations 6 - Get Adapter Types (Kinds)
  x-api-slug: apiadapterkinds-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/adaptive/master/_listings/vmware/apiadapterkinds-get-openapi.md
- name: vRealize Operations 6 - Get Adapter Instances
  x-api-slug: apiadapters-get
  description: 'TODO: Add Description'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/adaptive/master/_listings/vmware/apiadapters-get-openapi.md
- name: vRealize Operations 6 - Create a Python Adapter Instance
  x-api-slug: apiadapters-post
  description: "Be sure to check values in the JSON body for credentials.\nAlso note
    you will need to start the adapter using \"Star an adapter instance\" \nafter
    creation using the UUID from the response.\n\nIf you aren't using a CA, the certificate
    will have to be added via the UI\nI do not know of a way to do this via the REST
    API"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/adaptive/master/_listings/vmware/apiadapters-post-openapi.md
- name: vRealize Operations 6 - Start an adapter instance
  x-api-slug: apiadapters617d20fd536a4bea9f5e4c01dd845ddcmonitoringstatestart-put
  description: |-
    Replace the UUID with the ID of the adapter instance you want to start
    This can be retrieved using Get Adapter Instances
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/VMware_logo.png
  humanURL: http://vmware.com
  baseURL: https://example.com//suite-api/api
  tags: Cloud, Compute, Service API, Relative Data, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/adaptive/master/_listings/vmware/apiadapters617d20fd536a4bea9f5e4c01dd845ddcmonitoringstatestart-put-openapi.md
x-common:
- type: x-blog
  url: https://blogs.vmware.com/
- type: x-blog-rss
  url: http://blogs.vmware.com/all-vmware-blogs/wprss
- type: x-github
  url: https://github.com/VMware
- type: x-twitter
  url: https://twitter.com/VMware
- type: x-website
  url: http://vmware.com
- type: x-api-gallery
  url: http://visage.cloud.api.gallery.streamdata.io
- type: x-api-stack
  url: http://vmware.stack.network
- type: x-curated-source
  url: https://blogs.vmware.com/vcloud/2015/12/vmware-vcloud-air-network-compliance-spotlight-hipaa.html
- type: x-website
  url: https://www.vmware.com
- type: x-branding
  url: https://www.vmware.com/brand/our-brand.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---