# Introduction

This DAML example illustrates a virtual (pre)script(ion) that can only be

* Created by a doctor for a patient they have an existing care provider
  relationship with;
* Submitted by a patient to a pharmacy while the script has not expired;
* Accepted by a pharmacy while the script has not expired; and
* Is destroyed once it is filled.

Besides the virtualization of the prescription mechanism, this example
decouples doctors (or their support staff) from having to transmit a
prescription to pharmacy and allows a patient to submit the prescription to the
pharmacy that is most convenient for them at the time.

# Extensions

There are a number of potential extenstions to this example that were not
implemented in order to keep the example small and simple. Some of the possible
extensions are as follows:

* Creating a patient contract that captures a patients pending and current
  prescriptions. This could be used to, for example, prevent a patient from
  going to multiple different doctors to acquire excess amounts of a drug.

* This example does not model the mutual authorization by patient and doctor of
  the care provider relationship.

* Creating drug and condition contracts that would prevent doctors from
  prescribing a drug in a fashion contrary to its intended dosage or usage.
