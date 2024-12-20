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
  ir-02_odp.01:
    alt-identifier: ir-2_prm_1
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  ir-02_odp.02:
    alt-identifier: ir-2_prm_2
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  ir-02_odp.03:
    alt-identifier: ir-2_prm_3
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  ir-02_odp.04:
    alt-identifier: ir-2_prm_4
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
  sort-id: ir-02
---

# ir-2 - \[Incident Response\] Incident Response Training

## Control Statement

- \[a.\] Provide incident response training to system users consistent with assigned roles and responsibilities:

  - \[1.\] Within {{ insert: param, ir-02_odp.01 }} of assuming an incident response role or responsibility or acquiring system access;
  - \[2.\] When required by system changes; and
  - \[3.\] {{ insert: param, ir-02_odp.02 }} thereafter; and

- \[b.\] Review and update incident response training content {{ insert: param, ir-02_odp.03 }} and following {{ insert: param, ir-02_odp.04 }}.

## Control Assessment Objective

- \[IR-02a.\]

  - \[IR-02a.01\] incident response training is provided to system users consistent with assigned roles and responsibilities within {{ insert: param, ir-02_odp.01 }} of assuming an incident response role or responsibility or acquiring system access;
  - \[IR-02a.02\] incident response training is provided to system users consistent with assigned roles and responsibilities when required by system changes;
  - \[IR-02a.03\] incident response training is provided to system users consistent with assigned roles and responsibilities {{ insert: param, ir-02_odp.02 }} thereafter;

- \[IR-02b.\]

  - \[IR-02b.[01]\] incident response training content is reviewed and updated {{ insert: param, ir-02_odp.03 }};
  - \[IR-02b.[02]\] incident response training content is reviewed and updated following {{ insert: param, ir-02_odp.04 }}.

## Control guidance

Incident response training is associated with the assigned roles and responsibilities of organizational personnel to ensure that the appropriate content and level of detail are included in such training. For example, users may only need to know who to call or how to recognize an incident; system administrators may require additional training on how to handle incidents; and incident responders may receive more specific training on forensics, data collection techniques, reporting, system recovery, and system restoration. Incident response training includes user training in identifying and reporting suspicious activities from external and internal sources. Incident response training for users may be provided as part of [AT-2](#at-2) or [AT-3](#at-3) . Events that may precipitate an update to incident response training content include, but are not limited to, incident response plan testing or response to an actual incident (lessons learned), assessment or audit findings, or changes in applicable laws, executive orders, directives, regulations, policies, standards, and guidelines.

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
