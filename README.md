# Open Source Overview

## Chapter 1: Open Source Motivation and Vision

### A. Open Source Motivation (Why Restricted Sharing?)

- This project adopts a strictly restricted source-available model, rather than traditional open source. Its core motivation is to maximize value in a controlled and trusted environment:

#### 1. Accelerate Technical Transparency and Integration for Partners:

- Provide source code to core partners who have signed the NDA, enabling them to deeply understand the project's internal mechanisms, data flows, and integration points, significantly shortening the cycle of technical docking and system integration.

#### 2. Enhance Security and Compliance:

- By authorizing professional third-party organizations (such as security auditing firms) or partner teams to conduct security audits and independent verification, leveraging the power of external experts, the reliability, robustness, and security of the code are improved without disclosing core intellectual property rights.

#### 3. Promote Cutting-Edge Academic Exchange and Verification:

- Provide code to specific academic research institutions as a verification basis or data source for theoretical research, to jointly promote cutting-edge exploration and progress in related technical fields in non-commercial areas.

### B. Project Vision (Goals in a Constrained Environment)

The vision of this project is to become a technological cornerstone within a controlled ecosystem, achieving the following goals:

#### 1. Become the Gold Standard for Security Auditing in the Industry:

- Through continuous external audits performed by trusted partners, establish this project's codebase as a widely validated reference implementation in terms of security and reliability within specific technology areas.

#### 2. Establish an Efficient Trust Collaboration Cycle:

- Within a strict NDA framework, establish an efficient, low-risk collaboration cycle to ensure that feedback from partners and research institutions is applied promptly and accurately to the iteration of core code, forming a unique competitive advantage.

#### 3. Protect Core Intellectual Property While Achieving Technological Evolution:

Under the umbrella of legal agreements and customized licenses, the project can absorb optimization and security suggestions from external sources, achieving continuous technological evolution while resolutely protecting our company's core business value and intellectual property from misuse.


## Chapter 2: Licensing and Prohibitions

⚠️ Important Note: This is not a traditional open-source project ⚠️ Please note that this project does not follow the traditional open-source project definition of the Open Source Initiative (OSI). It is a source-available project, with the core goal of knowledge sharing and collaboration with trusted partners in a controlled environment, rather than maximizing free community participation.

### 2.1 Scope and Strict License Restrictions
This project uses a Custom Source-Available License to support specific academic research and security enhancement purposes. Usage of this project is subject to extremely strict restrictions, primarily in the following two core dimensions:

#### A. License Scope
The license for this project strictly limits its use. Any commercial use, product integration, redistribution, or creation of derivative works without the project's written authorization is prohibited (see Section 2.2). This license is the general license for this account.

- Permitted Uses:
* **Purely Academic Research Use:** Limited to code understanding, algorithm analysis, and paper publication within non-commercial institutions (such as universities and non-profit research institutes) (source of the code must be acknowledged).

* **Security Audit and Vulnerability Analysis:** Limited to security vulnerability detection, compliance audits, or functional safety assessments of the project code.

* **Prohibited Uses:**
* **Commercial Use or Integration:** Integration of the project code or any part thereof directly or indirectly into any commercial product or service is prohibited.

* **Public Release or Redistribution:** Public release, sharing, or distribution of the code to any third party without a signed agreement is prohibited.

#### B. Strict Audience Restriction
Due to the sensitive technology or proprietary information involved in this project, access and use are strictly limited:

* **Primary Audience:** This project is only open to partners who have signed a valid Non-Disclosure Agreement (NDA) or Collaborative Development Agreement with our company. All code visitors and users must first: be bound by a valid legal agreement.

We commit to strictly adhering to the confidentiality clauses in the NDA regarding code, technology, and project information.

- Excluded Audience: Any independent developer, the general public, potential commercial competitors, or entity that does not meet the above academic/security requirements without signing the NDA is not authorized to access or use the project code.

### 2.2 License Selection and Compliance

Selected License: [License](./ref/CBC-OpenSource-License.md) - CipherSafe Source-Available Non-Commercial License (CS-NC License) V1.0

#### A. Necessity and Basis for Customized License

- Because this project aims to balance technical transparency (for auditing/research) with the protection of core business secrets, we have chosen the highly customized CS-NC License.

- Differentiating from Traditional Open Source: This license does not conform to the Open Source Initiative (OSI) definition of "open source," which primarily prohibits commercial use and restricts the target audience (see Section 2.1 B) to ensure the project operates within a trust chain.

- Legal Basis: All terms of the CS-NC License are designed to complement the Non-Disclosure Agreement (NDA) signed by our company, ensuring maximum protection of the project's intellectual property and commercial interests during access to, research of, and use of the code.

#### B. Contributor License Agreement (CLA) Requirements

- Given the highly sensitive nature of this project, to ensure a single legal source for the codebase and clarity of intellectual property rights, the project requires:

- CLA Mechanism: All collaborators or individuals submitting code modifications (Pull Requests) to this project must sign a Contributor License Agreement (CLA) beforehand.

- Purpose: Through the CLA, contributors authorize our company to possess the necessary rights to the submitted code so that our company can:

- i. Include it within the scope of the CS-NC License;

- ii. Use the code for commercial purposes in the future without requiring duplicate licensing.

#### C. Third-Party Dependency License Compliance

- This project uses necessary third-party components during its build process, and we will strictly adhere to the open-source licenses of these components:

- Auditing and Isolation: In Phase 1 (timeline), all third-party dependencies will undergo license auditing. All dependencies must be compatible with the project's non-commercial targets, typically MIT, Apache 2.0, or similar permissive licenses.

- Distribution Restrictions: Although this project relies on certain open-source libraries, the CS-NC License restricts the distribution and use of the entire codebase. Licensees may not exploit this project to bypass the original license terms of third-party libraries.

## Chapter 3: Timeline & Phase Goals

### 3.1 Open Source Timeline & Execution

### 3.2 Phase Goals:

| Milestones (Phase) | Core Goals and Scope of Open Source Components | Key Tasks List (Compliance and Execution) | Planned Completion Time |
|---|---|---|---|
|Phase 1: Front-end Application and Emergency Units | Goals:<br />Verify the effectiveness of the controlled release process, complete the open-sourcing of the front-end application code, allowing it to be reviewed and discussed appropriately;<br />In addition, prioritize addressing the immediate security audit needs of some merchant node projects. |Complete the secure delivery of the first batch of code and internally fix critical and serious security issues.<br />1. Code Cleanup and Audit: Remove production environment privacy data from the front-end code.<br />2. Permission Settings: Complete the user whitelist settings for the GitHub repository and assign access permissions to the first batch of partners who have signed the NDA.<br />3. Documentation Release: Release the CS-NC License simultaneously with the code. |Late December|
|Phase 2: MPC Core Dependency Library|Goal:<br />Release the core dependency library for MPC (Multi-Party Secure Computation) with high security requirements, for partners to conduct in-depth security and algorithm audits. |Internally fix critical and serious security issues and ensure a clear boundary between the library and the "proprietary knowledge" described in the CS-NC License.<br /> 2. Dependency Audit Confirmation: Finalize the licenses of all third-party components depended on by the MPC library and list compliance statements in the corresponding README.<br /> 3. If necessary, write technical guidelines: Write specific algorithm principles and security audit guidelines for the MPC library. |Late December|
|Phase 3: Blockchain Access Layer and Others|Goal:<br />Complete controlled open-source coverage of the project's core technology stack and build a complete code audit/research environment. |Internally fix critical and serious security issues and plan to provide an overall architecture design update to facilitate partners' understanding of the system architecture. |Late January next year|

## Chapter 4: Scope Boundary of Open Source Components
### 4.1 Frontend Part: 
<table>
  <tr>
    <th colspan="3">CipherBC Flexify App</th>
  </tr>
  <tr>
    <td colspan="3">Link: ...</td>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
  </tr>
  <tr>
    <td>API Reference</td>
    <td>1</td>
  </tr>
  <tr>
    <td>dapp</td>
    <td>1</td>
  </tr>
  <tr>
    <td>MPC Logic Reference</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Related to CipherSafe</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Wallet backup</td>
    <td>1</td>
  </tr>
  <tr>
    <td>CipherCard</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Approval</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Risk Control</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Login and register</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Member/Department/Role Permissions</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Team/Wallet Creation</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Exchange</td>
    <td>2</td>
  </tr>
</table>

<table>
  <tr>
    <th colspan="2">CipherBC Flexify Desk</th>
  </tr>
  <tr>
    <td colspan="2">Link: ...</td>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
  </tr>
  <tr>
    <td>API Reference</td>
    <td>1</td>
  </tr>
  <tr>
    <td>DApp</td>
    <td>1</td>
  </tr>
  <tr>
    <td>WaaS</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Exchange</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Approval</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Risk Control</td>
    <td>2</td>
  </tr>
  <tr>
    <td>Team</td>
    <td>2</td>
  </tr>
</table>

<table>
  <tr>
    <th colspan="2">CipherSafe</th>
  </tr>
  <tr>
    <td colspan="2">Link: ...</td>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
  </tr>
  <tr>
    <td>Fingerprint SDK Reference</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Storage SDK Reference</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Bluetooth Interaction</td>
    <td>1</td>
  </tr>
  <tr>
    <td>MPC data processing</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Wallet Creation</td>
    <td>1</td>
  </tr>
  <tr>
    <td>Signature Verification</td>
    <td>1</td>
  </tr>
  <tr>
    <td>MPC create/clone/recover/sign</td>
    <td>1</td>
  </tr>
</table>

<table>
  <tr>
    <th>Module</th>
    <th>Stage</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>Key recovery tool</td>
    <td>1</td>
    <td></td>
  </tr>
</table>


### 4.2 MPC Part: 

<table>
  <tr>
    <th colspan="4">CipherSafe / Flexify</th>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>mpc sdk for ios/ andriod api</td>
    <td>1</td>
    <td></td>
  </tr>
  <tr>
    <td>recovery tool</td>
    <td>2</td>
    <td></td>
  </tr>
</table>

<table>
  <tr>
    <th colspan="4">WaaS(4/4, 1.0)</th>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>商户节点</td>
    <td>1</td>
    <td></td>
  </tr>
</table>

<table>
  <tr>
    <th colspan="4">Waas(m/n)</th>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>商户节点</td>
    <td>3</td>
    <td></td>
  </tr>
</table>


### 4.3 Blockchain Layer: 

<table>
  <tr>
    <th colspan="4">Waas</th>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>2019 Signature Machine</td>
    <td>3</td>
    <td></td>
  </tr>
  <tr>
    <td>2023 Signature Machine</td>
    <td>3</td>
    <td></td>
  </tr>
  <tr>
    <td>JS Signature Machine</td>
    <td>3</td>
    <td></td>
  </tr>
  <tr>
    <td>Merchant payment address contract source code</td>
    <td>3</td>
    <td></td>
  </tr>
</table>

<table>
  <tr>
    <th colspan="4">Flexify</th>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>Withdrawal (and MPC interaction) service</td>
    <td>3</td>
    <td></td>
  </tr>
  <tr>
    <td>Integration with business wallet tools</td>
    <td>3</td>
    <td></td>
  </tr>
</table>

<table>
  <tr>
    <th colspan="4">GemW</th>
  </tr>
  <tr>
    <th>Module</th>
    <th>Stage</th>
    <th>Link</th>
  </tr>
  <tr>
    <td>Seal machine service</td>
    <td>3</td>
    <td></td>
  </tr>
  <tr>
    <td>Signature machine service</td>
    <td>3</td>
    <td></td>
  </tr>
</table>

## Chapter 5: Macro Design
### 5.1 Architecture OverAll
<img src="./ref/OmnibusWallet/Architecture-OverAll.png" alt="drawing" width="800"/>

### 5.2 Solution of OmnibusWallet - OverAll
<img src="./ref/OmnibusWallet/Solution_of_OmnibusWallet.png" alt="drawing" width="800"/>

#### 5.2.1 Solution of OmnibusWallet - Level 1
<img src="./ref/OmnibusWallet/Level1-Solution_of_OmnibusWallet.png" alt="drawing" width="800"/>

#### 5.2.2 Solution of OmnibusWallet - Level 2
<img src="./ref/OmnibusWallet/Level2-Solution_of_OmnibusWallet_Arch.png" alt="drawing" width="800"/>

### 5.3 CipherSafe Overview

<img src="./ref/CipherSafe/CipherD-HWWSide-HWWAppActionFlow.png" alt="drawing" width="800"/>

<img src="./ref/CipherSafe/CipherDCloudStorage.png" alt="drawing" width="800"/>
