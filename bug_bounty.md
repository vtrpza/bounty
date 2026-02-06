About this engagement

We’re pleased to announce that we are expanding our Bug Bounty Program to include select safety and abuse issues. As AI technology rapidly evolves, so do the potential ways it can be misused. We believe it’s essential to recognize and reward responsible disclosures involving critical safety and abuse scenarios.
Program Rules

    Qualifying issues must represent a design or implementation issue in an active OpenAI product that can be abused by an attacker to cause material harm. For safety issues in particular, the report must contain a plausible harm scenario that indicates the harm is something that is substantially enabled or amplified by our models; for example, using our models to find potentially dangerous information that is freely available on search engines is out of scope for rewards.
    Reports must be addressable via a clear set of recommended steps or mitigations. The goal of this program is to reward for bug fixes and we cannot reward requests for general product improvements.
    Qualifying issues must be consistently reproducible. Researchers should provide enough steps and evidence to reproduce the issue reliably under typical conditions. We may accept partial or probabilistic exploits if the result is still high impact, but the burden of proof is on the researcher to demonstrate it is not a one-off fluke.
    We only reward for issues that have not already been submitted to us.
    Any accounts used as victims must be test accounts owned by the researcher. Any testing that affects accounts, assets, or services owned by others is strictly prohibited.
    Final reward decisions and amounts are up to OpenAI discretion, especially when applied to safety issues.

Scope and rewards
Credentials

You may test with your personal account or sign up for an additional testing account using your @bugcrowdninja.com email address. We prefer testing using this email address, but it is not mandatory.

Please note that authorized testing does not exempt you from all of OpenAI's terms of service. Abusing the service may result in rate limiting, blocking, or banning. Automated vulnerability scanners may trigger these outcomes. If your account or IP is rate-limited or blocked, please wait for the block to expire; we cannot manually remove it. If your account is banned, contact support@bugcrowd.com to provide an explanation and request un-banning. We will only do this a limited number of times, at our discretion, and never for content violations. You will be removed from the program for repeated ban evasion.

You will not be reimbursed for any upgrades or purchases made on your account.
Names and references to unreleased products/features

We welcome submissions of findings where references to projects or features that have not yet been publicly announced are discovered. This could be in source-code, API responses, Cloudflare enumerations, etc. These submissions are reviewed by another team on a case-by-case basis, but usually includes:

    The name or existence of an unannounced product or feature
    Internal project names for unannounced products or features

Accepted submissions in this category are eligible for a bounty.
Safe Harbor

OpenAI will not threaten or bring any legal action against anyone who makes a good faith effort to comply with this bug bounty policy. This includes any claim under the DMCA for circumventing technological measures to protect the services and applications eligible under this policy.

As long as you comply with this policy:

    We consider your safety and security research to be "authorized" under the Computer Fraud and Abuse Act (and/or similar state laws), and
    We waive any restrictions in our applicable Terms of Use and Usage Policies that would prohibit your participation in this policy, but only for the limited purpose of your safety and security research under this policy.

OpenAI systems and services may be interconnected with third-party systems and services. If you submit a report through our bug bounty program that affects a third party service, we will limit what we share with the affected third party. Please understand that, while we can authorize your research on OpenAI’s systems and services, we cannot authorize your efforts on third-party products or guarantee they won’t pursue legal action against you. That said, if legal action is initiated by a third party against you because of your participation in this bug bounty program, and you have complied with our bug bounty policy, we will take steps to make it known that your actions were conducted in compliance with this policy. This is not, and should not be understood as, any agreement on our part to defend, indemnify, or otherwise protect you from any third party action based on your actions.

You are expected, as always, to comply with all applicable laws.

If you have concerns or are unsure whether your safety and security research aligns with this policy, please contact support@bugcrowd.com before proceeding.

    Agentic Tools
    In scope
    Payment reward chart

    P1
        $5500 – $7500
    P2
        $2500 – $3500
    P3
        $750 – $1500
    P4
        $250 – $500

    Abuse risks in our agentic products including Operator, Deep Research, built-in ChatGPT tools, etc.
        In Scope: "Third party" or "indirect" prompt injection: an attacker is able to hijack a victim’s agent (e.g. Operator, Deep Research) resulting in leaking the victim’s sensitive private data from or performing a harmful action on an account owned by the victim.
        In Scope: An agentic tool like Operator creates new OpenAI user accounts at scale - at least 10 accounts without human interaction. This objective proves the concept of manipulating an agentic tool like Operator into performing a disallowed action without having to do so on a website not owned by OpenAI, which is prohibited.
        Case-by-case: Operator or another agent model performs some potentially harmful action not listed above.
        Out of Scope: Prompt injection vulnerabilities in the API or Codex CLI when connected to other, non-OpenAI models or services.
    Name / Location	Tags	Known issues
    Agentic Tools	
        Artificial Intelligence
    Fine-Tuning
    In scope
    Payment reward chart

    P1
        $3500 – $4500
    P2
        $1500 – $2500
    P3
        $500 – $750
    P4
        $175 – $225

    Fine-tuning smaller, cost-efficient models using outputs from more capable models.
        Case-by-case: Techniques that evade our detection of malicious fine-tuning training data. For example, a technique that allows a user to fine-tune on training data intended and able to move the model out of alignment.
        Out of Scope: Fine-tuning a model to generate policy violative content that doesn’t pose a plausible risk of real-world harm.
    Name / Location	Tags	Known issues
    Fine-Tuning Tools	
        Artificial Intelligence
    OpenAI Proprietary Information
    In scope
    Payment reward chart

    P1
        $5500 – $7500
    P2
        $2500 – $3500
    P3
        $750 – $1500
    P4
        $250 – $500

    Vulnerabilities or model issues that return OpenAI internal information, intellectual property, or otherwise confidential data.
        In Scope: Vulnerabilities that return proprietary information related to reasoning, e.g. o1's full unsummarized Chain of Thought.
        In Scope (already covered by the existing Security Bug Bounty scope): Vulnerabilities that enable the exposure of other OpenAI proprietary information (e.g. insider information) - this is already covered by the existing Security Bug Bounty scope and should be reported here.
        Out of Scope: Model responses that appear to expose internal OpenAI proprietary information.
        Out of Scope: System prompts, or any other information present in the model context window at inference time except for CoTs.
    Name / Location	Tags	Known issues
    *.openai.com	
        Website TestingAzurePython
    Account and Platform Integrity
    In scope
    Payment reward chart

    P1
        $5500 – $7500
    P2
        $2500 – $3500
    P3
        $750 – $1500
    P4
        $250 – $500

    The ability to bypass our safeguards against abuse on our platform.
        In Scope: Vulnerabilities in our account integrity and platform integrity signals, e.g. automating mass creation of OpenAI accounts.
        In Scope (already covered by the existing Security Bug Bounty scope): Exploits that allow users to access features, data, or functionalities beyond their authorized permissions. This is already covered by the existing Security Bug Bounty scope and should be reported here.
        Out of Scope: Evading controls around geographic access restrictions.
        Out of Scope: Testing that facilitates genuine fraud or requires social engineering, e.g. creating fraudulent OpenAI Startup Fund accounts.
    Name / Location	Tags	Known issues
    openai.com	
        Website TestingAzurePython
    Content Issues
    Out of scope

    The model generates responses that violate OpenAI's policy on disallowed content.
        All content/model response issues are out of scope - these issues are complex and not addressable through traditional security fixes.
    Name / Location	Tags	Known issues
    OpenAI models	
    Other Novel Abuse
    In scope
    Payment reward chart

    P1
        $5500 – $7500
    P2
        $2500 – $3500
    P3
        $750 – $1500
    P4
        $250 – $500

        Case-by-case: Outside of the examples listed above, if your report contains a flaw that facilitates a direct path to user harm and actionable, discrete remediation steps we may still consider it in scope for rewards.
        Out of Scope: Using OpenAI products in an abuse scenario that is already possible with other tools. For example, the model answers questions about potentially dangerous topics with content that is already available online via search engines.
    Name / Location	Tags	Known issues
    Other	
        Artificial Intelligence

Known Issues

    Counts of P1 – P4 vulnerabilities
    Includes imported issues tracked outside of Bugcrowd.
    Excludes Out of scope vulnerabilities.

    Unique 27 Includes issues in Triaged, Unresoved, and Informational states
    Total 64 Includes Duplicate of unique known issues