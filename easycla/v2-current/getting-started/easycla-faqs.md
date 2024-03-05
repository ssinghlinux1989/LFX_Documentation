# EasyCLA FAQs

**Who do I contact to enable my Linux Foundation-hosted project to use EasyCLA?**

Open [https://jira.linuxfoundation.org/plugins/servlet/theme/portal/4/create/143](https://jira.linuxfoundation.org/plugins/servlet/theme/portal/4/create/143), submit the form describing your requirements, and import your existing CLAs.

**Why does The Linux Foundation ask contributors of some projects to sign CLAs?**

Some project communities have elected to use CLAs as a required step for code contributions. The Linux Foundation wants to ensure that contributions comply with the IP (Intellectual Property) policies of that project.

**What is the difference between a Corporate CLA (CCLA) and an Individual CLA (ICLA)?**

A Corporate CLA needs to be in place if you are contributing code on behalf of your employer. A Corporate CLA should be signed by an individual who is authorized to enter into legal agreement on behalf of the company. After the Corporate CLA is signed, your email address needs to be included in an approved list for the project. A CCLA manager for your company is responsible for managing the approved list.

An Individual CLA is signed by an individual for contributions that they contribute on their own behalf, as opposed to contributions on behalf of their employer or another entity.

**How can I contribute to GitHub/Gerrit/GitLab repositories?**

If you are an individual contributor, see [Individual Contributor](../contributors/individual-contributor.md). If you are a corporate contributor, see [Corporate Contributor](../contributors/corporate-contributor.md) for details.

#### **How can I view my ICLA document after I sign it?**

Open your email, which you provided while signing the ICLA, to check the signed ICLA that was sent from The Linux Foundation. If you have not received the email, you can open a support ticket to have it resent.

#### **Which CCLA approval criteria option has the lowest maintenance overhead?**

Using the Domain **Approval Criteria** requires less overhead because CCLA signatories and CCLA managers do not need to add and manage numerous employee email addresses.

**I contribute to an open source project on behalf of my employer. Do I need to sign anything?**

Probably not. If your company's CCLA signatory has signed a Corporate CLA, and if you are included in the approved list under that company's CLA, then you simply confirm your association with the company during your code submission process.

However, if you are the first one from your company to contribute to a project, then your company's CCLA signatory will need to sign a Corporate CLA as part of the EasyCLA setup process. Depending on the company, you might be an authorized CCLA signatory (please check with the legal counsel of your company to be sure).

Otherwise, if your company has already signed a Corporate CLA but you are not yet on your company's approved list, you must be included on the approved list by your company's CCLA manager as part of the EasyCLA process.

**When I am trying to contribute code under a CCLA, what should I do if my company is not listed?**

You must add your company as described [here](../contributors/corporate-contributor.md#if-your-company-is-not-in-the-list) before you can contribute code under corporate CLA (CCLA).

**If my project community has elected to use CLAs as a required step for contributions to their code, do I need to be authorized under a CLA for each project to which I contribute?**

Yes, provided that the project has a CLA.

* If you are contributing as an individual—you must sign an Individual CLA for each project to which you contribute.
* If you are contributing as an employee of a company, your company's CCLA signatory must sign a Corporate CLA.

**Do I have to sign a CLA every time I contribute code to a project?**

If you have already signed CLA for a project, then you don't need to sign every time to contribute to the project. Signing a CLA for a project covers all code contributions to that project. You may, however, need to sign additional CLAs if you choose to contribute to other projects that require CLAs.

#### **Where do I view my individual CLA (ICLA) after I sign the ICLA?**

Your ICLA will be emailed to the email address you provided when signing it, as soon as you sign it. If you did not receive the email, you can open a support ticket to have it resent.

#### Why is my EasyCLA status not updated even after I complete the process.

(Individual Contributors) Wait for the few seconds or refresh the page to get your EasyCLA status updated.

(Corporate Contributors) After you complete the process, you must acknowledge [acknowledging company contribution](../contributors/corporate-contributor.md#acknowledge-company-contribution). If you have already acknowledged company contributions, wait for few seconds or refresh the page to get your EasyCLA status updated.

**Why does EasyCLA redirect and update a previously opened PR instead of the one I performed the signature on?**

When there are two or more opened PRs in the same repository, during the signature process, EasyCLA will always redirect and update the earliest opened PR. Once the signature has been completed, you can add a `"/easycla"` comment on the other PRs to trigger the EasyCLA bot and update your authorization status for each open PR.

**The cla/linuxfoundation check on my PR for a Kubernetes repo is not marked as passed after signing the CNCF CLA through EasyCLA?**

Kubernetes repositories are in the process of migrating from CLA v1 (cla/linuxfoundation check) to EasyCLA (EasyCLA check). During this migration, the cla/linuxfoundation check is not being updated even when the users have properly signed the CLA. If the PR has the label "cncf-cla: yes,"  it means the authorization for the user has been granted. Note that the cla/linuxfoundation check is neither a requirement nor a blocker for merging the PR once all the required labels have been included.

Once the migration has been completed cla/linuxfoundation check will be removed.

**What is the acceptable email format?**

A valid email address with an email prefix and an email domain, for example _abc@mail.com_

The allowed characters for the email prefix are letters (a-z), numbers, underscores, periods, and dashes, and an underscore, period, or dash must be followed by one or more letters or numbers, for example:\
_abc-d@mail.com/abc.def@mail.com/abc@mail.com/abc\_def@mail.com_

The allowed characters for an email domain are letters, numbers, and dashes, and the last portion of the domain must be at least two characters, for example:.com,.org,.cc.
