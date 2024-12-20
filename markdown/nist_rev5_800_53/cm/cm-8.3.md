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
  cm-8.3_prm_1:
    aggregates:
      - cm-08.03_odp.01
      - cm-08.03_odp.02
      - cm-08.03_odp.03
    profile-param-value-origin: <REPLACE_ME>
  cm-08.03_odp.01:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  cm-08.03_odp.02:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  cm-08.03_odp.03:
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  cm-08.03_odp.04:
    alt-identifier: cm-8.3_prm_2
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  cm-08.03_odp.05:
    alt-identifier: cm-8.3_prm_3
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
  cm-08.03_odp.06:
    alt-identifier: cm-8.3_prm_4
    profile-values:
      - <REPLACE_ME>
    profile-param-value-origin: <REPLACE_ME>
x-trestle-global:
  profile:
    title: NIST Special Publication 800-53 Revision 5 HIGH IMPACT BASELINE
  sort-id: cm-08.03
---

# cm-8.3 - \[Configuration Management\] Automated Unauthorized Component Detection

## Control Statement

- \[(a)\] Detect the presence of unauthorized hardware, software, and firmware components within the system using {{ insert: param, cm-8.3_prm_1 }} {{ insert: param, cm-08.03_odp.04 }} ; and

- \[(b)\] Take the following actions when unauthorized components are detected: {{ insert: param, cm-08.03_odp.05 }}.

## Control Assessment Objective

- \[CM-08(03)(a)\]

  - \[CM-08(03)(a)[01]\] the presence of unauthorized hardware within the system is detected using {{ insert: param, cm-08.03_odp.01 }} {{ insert: param, cm-08.03_odp.04 }};
  - \[CM-08(03)(a)[02]\] the presence of unauthorized software within the system is detected using {{ insert: param, cm-08.03_odp.02 }} {{ insert: param, cm-08.03_odp.04 }};
  - \[CM-08(03)(a)[03]\] the presence of unauthorized firmware within the system is detected using {{ insert: param, cm-08.03_odp.03 }} {{ insert: param, cm-08.03_odp.04 }};

- \[CM-08(03)(b)\]

  - \[CM-08(03)(b)[01]\] {{ insert: param, cm-08.03_odp.05 }} are taken when unauthorized hardware is detected;
  - \[CM-08(03)(b)[02]\] {{ insert: param, cm-08.03_odp.05 }} are taken when unauthorized software is detected;
  - \[CM-08(03)(b)[03]\] {{ insert: param, cm-08.03_odp.05 }} are taken when unauthorized firmware is detected.

## Control guidance

Automated unauthorized component detection is applied in addition to the monitoring for unauthorized remote connections and mobile devices. Monitoring for unauthorized system components may be accomplished on an ongoing basis or by the periodic scanning of systems for that purpose. Automated mechanisms may also be used to prevent the connection of unauthorized components (see [CM-7(9)](#cm-7.9) ). Automated mechanisms can be implemented in systems or in separate system components. When acquiring and implementing automated mechanisms, organizations consider whether such mechanisms depend on the ability of the system component to support an agent or supplicant in order to be detected since some types of components do not have or cannot support agents (e.g., IoT devices, sensors). Isolation can be achieved , for example, by placing unauthorized system components in separate domains or subnets or quarantining such components. This type of component isolation is commonly referred to as "sandboxing."

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
