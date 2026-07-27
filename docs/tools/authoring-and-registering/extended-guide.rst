FAIR Wizard: extended guide
============================

.. admonition:: About this tool

   The FAIR Assessment Authoring Tool, often referred to as just "FAIR
   Wizard", is a tool that helps users in the registration of FAIR
   Assessment Components (FACs). The FACs that can be registered using
   this tool are: Benchmarks, Metrics and Tests.

   This is not the only way to do this, but it provides a
   straightforward, quick and easy to follow questionnaire that allows
   users to create and submit the metadata for their FACs.

Further information on how to fill in, update, and troubleshoot
projects — independently.


Best practices
---------------

- **Read the instructions and descriptions carefully.**
  You will find detailed descriptions and instructions throughout the
  entire questionnaire, explaining what and how you are expected to
  answer. You will find questions that are marked as ``mandatory``,
  while others are ``optional`` or ``highly recommended``. These tags
  are shown under each question.

  Please, make sure you understand what you're being asked, and how to
  respond to each type of question. Different questions might need or
  allow only a certain type of formatted answers, such as URLs.

- **Make sure you know how to use integration questions properly.**
  See the :ref:`integration-questions` section for more information on
  how to use them correctly.

- **If you are unsure of something or run across a problem/error,
  reach out to the contact person.**
  You can either contact the DSW Team for general technical
  issues/suggestions, or contact ``sara.curiel.manzanas@upm.es`` about
  any specific question/suggestion/problem related to the registration
  of FAIR Assessment Components (FACs) using the OSTrails FAIR
  Assessment Authoring Tool (FAIR Wizard).


.. _integration-questions:

Integration questions
-----------------------

Integration questions are those that allow you to use a browser to
search for and select a value from an external registry (e.g.,
FAIRsharing, ROR or ORCID), rather than typing free text. They are
recognisable by a search/lookup box embedded in the question.

Current integration questions include:

.. list-table::
   :header-rows: 1
   :widths: 25 20 15 25

   * - Question field
     - Integrated registry
     - Cardinality
     - Manual (free text) alternative
   * - License
     - FAIRsharing
     - Single
     - No
   * - Application area of knowledge
     - FAIRsharing
     - Multiple
     - Yes
   * - Taxonomy
     - FAIRsharing
     - Multiple
     - Yes
   * - Keywords
     - FAIRsharing
     - Multiple
     - Yes
   * - Organisation information
     - FAIRsharing / ROR
     - Multiple
     - If not registered in FAIRsharing or ROR
   * - Responsible contact person
     - ORCID
     - Multiple
     - No — Just the email address field
   * - Other related FACs
     - FAIRsharing
     - Multiple
     - Yes

Although some of these questions include an option to manually type in
the answer, it is not recommended to do so. Please, only consider this
option when your answer is not available in the integrated registry.

**Integration questions are the most common source of problems when
filling in the questionnaire.** If you encounter issues, check these
questions first.

Frequent issues related to integration questions:

.. admonition:: Previous answers' format don't match an update
   :class: note

   This is the most common issue. When a Knowledge Model (KM) is
   updated, previously structured answers to these integrations may
   become invalid or incompatible, leading to capturing the
   information in a wrong way that will likely cause errors. In some
   of the cases, you may notice that the text in the answer box is
   displayed with a raw markdown format, e.g. you will see
   ``**text**`` instead of **text**, which is a very clear sign that
   this is happening.

   To fix this, make sure you clean previous answers for all the
   integration questions and answer them again, once you have
   migrated the KM to the latest version.

.. admonition:: Too long in the pipeline
   :class: note

   Since it's not necessary to complete the questionnaire and submit
   the document in one sitting, a project can sometimes go a long time
   without being edited. When this happens, once you want to return to
   complete the remaining sections and submit the document, you will
   need to clear the integration questions and answer them again to
   ensure that the data is being entered correctly.

.. admonition:: Questions not answered properly
   :class: note

   Please, make sure that you select one option from the dropdown
   possible answers. You should click on it, and the answer box should
   update accordingly after doing so, with the corresponding text.

Other relevant considerations when answering integration questions:

.. tip:: Searching effectively

   Entering the full text for an answer (e.g. *Gene Ontology
   Consortium*) may return no results, even when the option should be
   available. When this happens, try using 1–2 keywords instead (e.g.
   *Gene Ontology* or *Consortium*).

   If results still seem wrong or empty, try abbreviations or
   alternative names for the resource.

.. tip:: Adding multiple answers

   For questions that allow multiple answers (Cardinality
   "Multiple"), you must click the "Add" button for each answer you
   wish to enter. This also applies to questions that allow manual
   entry as an alternative, for cases when the term you need isn't
   available in the integrated registry — please use the "Add" button
   in that case as well. If you're combining both the integrated
   browser and manual entry for the same question, make sure every
   individual answer is added via its own "Add" click.


.. _km-updates:

Knowledge Model and Document Template updates
------------------------------------------------

Occasionally the Knowledge Model (KM) underlying the questionnaire is
updated — questions may be added, restructured, or deleted. Whenever
an update is available, a small yellow tag that looks like the one
below will appear next to your project:

.. image:: https://raw.githubusercontent.com/saracuriel/OSTrails-FAIR-Wizard-guide/main/update-km.png
   :alt: update available badge
   :height: 24px

Here is what to expect:

- By clicking on the yellow button, you will be prompted to migrate
  your project to the new KM version. Follow the on-screen steps — in
  most cases this is straightforward.
- Review integration questions after migration, clear the answers to
  those questions and re-answer them if needed, to avoid any issues.
- Check for new required questions and modifications of the already
  existing ones. Updates may add questions not present when you
  originally filled in the form. You will be notified of all the
  changes affecting the questionnaire when migrating.
- Do not ignore update prompts. Working on an outdated KM version may
  mean your output doesn't reflect the current template and could
  cause submission errors.

Unfortunately, when a Document Template is updated, you will not be
notified. To make sure your project is working with the latest
template, make sure to check for updates when generating new documents
and before submitting them. You will know if any new version is
available by clicking on the selected template under the "Default
document template" section in the "Settings" tab of a project.


.. _how-to-update:

How to update records
-----------------------

If you wish to update your FAC, once you have already submitted it for
registration, you should consider the following aspects:

For Benchmarks and Metrics records
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

When you first submit your FAC document, it will feed into both
FAIRsharing and the FAIR Champion FDP Index (via GitHub). If you wish
to update your FAC, you will need to submit a new version of the
document. This will create a new record in the GitHub repository and
will eventually be updated in the FAIR Champion FDP Index. However, if
your record was already accepted to register in FAIRsharing, any
further modification should also be made through the FAIRsharing
platform. Submitting an updated version of your FAIR Wizard project
will **not** push any changes into FAIRsharing.

For Tests records
~~~~~~~~~~~~~~~~~~~

Updates can be made by simply submitting the updated version of the
project document.


.. _submission-errors:

Submission errors
-------------------

If submission fails or returns an error, work through these steps:

1. **Check for KM and/or Document Template updates.** You may be
   working with an outdated version of the KM or template. Check the
   :ref:`km-updates` section for more information. This is the most
   common source of errors when you try to submit a document and you
   get the following message: *"There are no submission services
   configured for this type of document"*.
2. **Re-answer integration questions.** These are the most common
   source of submission and preview-rendering errors.
3. **Check for unanswered mandatory questions.**
4. **Contact the OSTrails team.** If you have tried the above and
   still encounter issues, reach out to
   ``sara.curiel.manzanas@upm.es`` for further assistance.


.. _quick-reference:

Other issues you may encounter
---------------------------------

.. list-table::
   :header-rows: 1
   :widths: 35 65

   * - Issue
     - What to do
   * - Answers not saving into the answer box
     - Re-answer it; for integration questions, make sure to select an
       option from the drop-down results
   * - Search returns no results
     - Try 1–2 keywords, not the full name
   * - Submission fails
     - Check mandatory questions + re-answer integration questions
   * - KM update prompt appears for your project
     - Migrate + review integration questions
   * - Output document looks wrong or incomplete
     - Check the answers to integration questions + check whether some
       answers are not saved into the answer box + re-generate the
       document
