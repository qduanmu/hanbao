---
x-trestle-set-params:
    # This section contains the parameters that are part of this control.
  # Each parameter has properties. Only the profile-values and display-name properties are editable.
  # The other properties are informational.
  #
  # The values property for a parameter represents values inherited from the OSCAL catalog.
  # To override the catalog settings, use bullets under profile-values as shown below:
  #
  #   profile-values:
  #     - value 1
  #     - value 2
  #
  # If the "- <REPLACE_ME>" placeholder appears under profile-values, it is the same as if
  # the profile-values property were left empty.
  #
  # Some parameters may show an aggregates property which lists other parameters. This means
  # the parameter value is made up of the values from the other parameters. For parameters
  # that aggregate, profile-values is not applicable.
  #
  # Property param-value-origin is meant for putting the origin from where that parameter comes from.
  # In order to be changed in the current profile, profile-param-value-origin property will be displayed with
  # the placeholder "<REPLACE_ME>" for you to be replaced. If a parameter already has a param-value-origin
  # coming from an inherited profile, do no change this value, instead use profile-param-value-origin as follows:
  #
  #    param-value-origin: DO NOT REPLACE - this is the original value
  #    profile-param-value-origin: <REPLACE_ME> - replace the new value required HERE
  #
  sc-07.04_odp:
    alt-identifier: sc-7.4_prm_1
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
  sort-id: sc-07.04
---

# sc-7.4 - \[System and Communications Protection\] External Telecommunications Services

## Control Statement

- \[(a)\] Implement a managed interface for each external telecommunication service;

- \[(b)\] Establish a traffic flow policy for each managed interface;

- \[(c)\] Protect the confidentiality and integrity of the information being transmitted across each interface;

- \[(d)\] Document each exception to the traffic flow policy with a supporting mission or business need and duration of that need;

- \[(e)\] Review exceptions to the traffic flow policy {{ insert: param, sc-07.04_odp }} and remove exceptions that are no longer supported by an explicit mission or business need;

- \[(f)\] Prevent unauthorized exchange of control plane traffic with external networks;

- \[(g)\] Publish information to enable remote networks to detect unauthorized control plane traffic from internal networks; and

- \[(h)\] Filter unauthorized control plane traffic from external networks.

## Control Assessment Objective

- \[SC-07(04)(a)\] a managed interface is implemented for each external telecommunication service;

- \[SC-07(04)(b)\] a traffic flow policy is established for each managed interface;

- \[SC-07(04)(c)\]

  - \[SC-07(04)(c)[01]\] the confidentiality of the information being transmitted across each interface is protected;
  - \[SC-07(04)(c)[02]\] the integrity of the information being transmitted across each interface is protected;

- \[SC-07(04)(d)\] each exception to the traffic flow policy is documented with a supporting mission or business need and duration of that need;

- \[SC-07(04)(e)\]

  - \[SC-07(04)(e)[01]\] exceptions to the traffic flow policy are reviewed {{ insert: param, sc-07.04_odp }};
  - \[SC-07(04)(e)[02]\] exceptions to the traffic flow policy that are no longer supported by an explicit mission or business need are removed;

- \[SC-07(04)(f)\] unauthorized exchanges of control plan traffic with external networks are prevented;

- \[SC-07(04)(g)\] information is published to enable remote networks to detect unauthorized control plane traffic from internal networks;

- \[SC-07(04)(h)\] unauthorized control plane traffic is filtered from external networks.

## Control guidance

External telecommunications services can provide data and/or voice communications services. Examples of control plane traffic include Border Gateway Protocol (BGP) routing, Domain Name System (DNS), and management protocols. See [SP 800-189](#f5edfe51-d1f2-422e-9b27-5d0e90b49c72) for additional information on the use of the resource public key infrastructure (RPKI) to protect BGP routes and detect unauthorized BGP announcements.

# Editable Content

<!-- Make additions and edits below -->
<!-- The above represents the contents of the control as received by the profile, prior to additions. -->
<!-- If the profile makes additions to the control, they will appear below. -->
<!-- The above markdown may not be edited but you may edit the content below, and/or introduce new additions to be made by the profile. -->
<!-- If there is a yaml header at the top, parameter values may be edited. Use --set-parameters to incorporate the changes during assembly. -->
<!-- The content here will then replace what is in the profile for this control, after running profile-assemble. -->
<!-- The current profile has no added parts for this control, but you may add new ones here. -->
<!-- Each addition must have a heading either of the form ## Control my_addition_name -->
<!-- or ## Part a. (where the a. refers to one of the control statement labels.) -->
<!-- "## Control" parts are new parts added after the statement part. -->
<!-- "## Part" parts are new parts added into the top-level statement part with that label. -->
<!-- Subparts may be added with nested hash levels of the form ### My Subpart Name -->
<!-- underneath the parent ## Control or ## Part being added -->
<!-- See https://oscal-compass.github.io/compliance-trestle/tutorials/ssp_profile_catalog_authoring/ssp_profile_catalog_authoring for guidance. -->
