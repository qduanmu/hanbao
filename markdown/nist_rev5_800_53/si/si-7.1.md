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
  si-7.1_prm_1:
    aggregates:
      - si-07.01_odp.01
      - si-07.01_odp.05
      - si-07.01_odp.09
    profile-param-value-origin: <REPLACE_ME>
  si-7.1_prm_2:
    aggregates:
      - si-07.01_odp.02
      - si-07.01_odp.06
      - si-07.01_odp.10
    profile-param-value-origin: <REPLACE_ME>
  si-7.1_prm_3:
    aggregates:
      - si-07.01_odp.03
      - si-07.01_odp.07
      - si-07.01_odp.11
    profile-param-value-origin: <REPLACE_ME>
  si-7.1_prm_4:
    aggregates:
      - si-07.01_odp.04
      - si-07.01_odp.08
      - si-07.01_odp.12
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.01:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.02:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.03:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.04:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.05:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.06:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.07:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.08:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.09:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.10:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.11:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  si-07.01_odp.12:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
  sort-id: si-07.01
---

# si-7.1 - \[System and Information Integrity\] Integrity Checks

## Control Statement

Perform an integrity check of {{ insert: param, si-7.1_prm_1 }} {{ insert: param, si-7.1_prm_2 }}.

## Control Assessment Objective

- \[SI-07(01)[01]\] an integrity check of {{ insert: param, si-07.01_odp.01 }} is performed {{ insert: param, si-07.01_odp.02 }};

- \[SI-07(01)[02]\] an integrity check of {{ insert: param, si-07.01_odp.05 }} is performed {{ insert: param, si-07.01_odp.06 }};

- \[SI-07(01)[03]\] an integrity check of {{ insert: param, si-07.01_odp.09 }} is performed {{ insert: param, si-07.01_odp.10 }}.

## Control guidance

Security-relevant events include the identification of new threats to which organizational systems are susceptible and the installation of new hardware, software, or firmware. Transitional states include system startup, restart, shutdown, and abort.

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
