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
  ma-03.03_odp:
    alt-identifier: ma-3.3_prm_1
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
  sort-id: ma-03.03
---

# ma-3.3 - \[Maintenance\] Prevent Unauthorized Removal

## Control Statement

Prevent the removal of maintenance equipment containing organizational information by:

- \[(a)\] Verifying that there is no organizational information contained on the equipment;

- \[(b)\] Sanitizing or destroying the equipment;

- \[(c)\] Retaining the equipment within the facility; or

- \[(d)\] Obtaining an exemption from {{ insert: param, ma-03.03_odp }} explicitly authorizing removal of the equipment from the facility.

## Control Assessment Objective

- \[MA-03(03)(a)\] the removal of maintenance equipment containing organizational information is prevented by verifying that there is no organizational information contained on the equipment; or

- \[MA-03(03)(b)\] the removal of maintenance equipment containing organizational information is prevented by sanitizing or destroying the equipment; or

- \[MA-03(03)(c)\] the removal of maintenance equipment containing organizational information is prevented by retaining the equipment within the facility; or

- \[MA-03(03)(d)\] the removal of maintenance equipment containing organizational information is prevented by obtaining an exemption from {{ insert: param, ma-03.03_odp }} explicitly authorizing removal of the equipment from the facility.

## Control guidance

Organizational information includes all information owned by organizations and any information provided to organizations for which the organizations serve as information stewards.

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
