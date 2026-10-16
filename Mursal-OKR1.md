# StudentShare: Responsible File Sharing and Copyright Protection
**Prepared by: Mursal Hamidy**  
**Course: CS230**

## 0. Company Summary

### Company Overview and Stakeholders

StudentShare is a peer-to-peer academic file-sharing platform for students. It will be available as an app and website. The purpose of StudentShare is to make academic file sharing more convenient while protecting safety, privacy, fairness, academic integrity, and intellectual-property rights.

StudentShare will help students share their own notes, public-domain documents, and study resources they have permission to distribute. The platform may also become a student hub where users can find useful academic resources, organize documents, and collaborate with classmates without being overwhelmed by unnecessary features.

The main stakeholders are students, instructors, universities, school information-technology departments, authors, publishers, copyright owners, StudentShare employees, and developers. Students want convenient and affordable access to useful study resources. Instructors and universities want students to collaborate without sharing prohibited materials or violating academic-integrity policies. Authors and publishers want their original work protected. StudentShare developers must design the system so that useful sharing does not encourage misuse.

StudentShare’s mission is to make the most convenient, easy-to-use file-sharing tool without sacrificing the quality of the user experience or user safety. Its core values are convenience, safety and responsibility, privacy, fairness, and accessibility.

During the next five years, StudentShare plans to become a central student platform by reaching one million registered users, working with 100 schools, supporting 25 million shared files each year, and building active participation at CSU and UC campuses in California.

### Technical Architecture, Computation, and Storage

StudentShare uses a hybrid technical model. It combines direct peer-to-peer sharing with cloud-based services that support connections, temporary storage, a marketplace, and a library.

First, direct peer-to-peer file transfers occur between students’ devices. A student can create a secure sharing code and send it to another student. The receiving student uses the code to connect and receive the document. The primary file transfer happens directly between the devices instead of permanently storing every shared file on a central server. WebRTC can support this type of browser-based peer-to-peer data transfer [1].

Second, StudentShare uses a central server for backend authentication, signaling, and connection support. The platform aims to reduce unnecessary login barriers, but it is not intended to promise complete anonymity. Authentication can occur behind the scenes so that StudentShare can provide security, reporting, and appeals while keeping the user experience simple. The central server may also temporarily store files when a direct transfer fails. Temporary files should be encrypted and automatically deleted after a limited period, such as 24 hours, unless a user chooses to retry the transfer.

Third, StudentShare will maintain cloud-based storage for its marketplace and library services. These areas are different from direct peer-to-peer sharing because files may remain available for longer periods. Therefore, permanently stored library or marketplace resources must be original student materials, public-domain resources, licensed materials, or resources shared with clear permission from the owner. This distinction is important because direct transfers, temporary cloud storage, and permanent cloud resources have different privacy, copyright, cost, and ethical responsibilities.

## 1. Objective and Key Results

### Objective

Encourage ethical sharing of documents while safeguarding intellectual-property rights, privacy, and student control over the items they share.

StudentShare is intended to allow students to share their own notes, public-domain documents, and any resources they have permission to share. However, the site must also discourage users from posting copyrighted textbook pages, lecture recordings, answer keys, plagiarized work, or other material they do not have permission to distribute. Copyright is legal protection for original works of authorship, such as books, movies, music, and software [2].

This objective supports StudentShare’s values of safety, responsibility, privacy, fairness, and convenience. The company should make responsible behavior easy to understand without making the platform difficult to use.

### Key Results

1. Before a student uploads or shares a document, 100% of upload and sharing screens will display a clear reminder about copyright, privacy, and academic-integrity responsibilities.

2. At least 90% of copyright, privacy, or responsible-sharing reports will receive an acknowledgment or initial response within 48 hours.

3. In a usability test with 20 students, at least 80% of participants will correctly identify which materials they may share and successfully choose an appropriate access setting for a file or folder.

4. At least 80% of students who complete the usability test will rate the sharing guidance as clear and easy to understand on a survey scale of 1 to 10.

## 2. Metrics and Experimentation

StudentShare will measure the number of uploads, direct file transfers, shared links, reports, response times, restricted content, appeals, appeal outcomes, and use of privacy controls. The company will also measure whether students understand the sharing rules and can choose suitable access settings.

The main experiment will be a usability test with 20 students who represent the platform’s target users. Each participant will read the upload rules and use a StudentShare prototype. They will decide whether they may share the following materials:

- Their own class notes
- A full textbook chapter
- A lecture recording
- An answer key for a quiz or exam
- A study guide created with permission
- A file containing another student’s private information

Participants will also choose appropriate access settings. For example, they may choose to keep a document private, share it with a small study group, or share it with a class. The experiment will measure task completion, correct answers, time required, participant confidence, and feedback about the instructions.

Usability testing helps organizations determine whether representative users can understand and effectively use a product [3]. If fewer than 80% of participants correctly identify allowed content or choose a suitable sharing setting, StudentShare will improve its upload guidance, privacy controls, and interface before expanding the platform.

## 3. Ethical Impacts and Issues

One major ethical concern is copyright infringement. Students may upload paid textbook pages, lecture recordings, copyrighted study materials, or other content without permission. This could negatively affect authors, publishers, instructors, and educational institutions.

This concern relates to *MGM Studios, Inc. v. Grokster, Ltd.* In that case, the Supreme Court explained that peer-to-peer technology itself was not automatically unlawful. However, a company could be responsible when it intentionally encouraged copyright infringement [4]. StudentShare must therefore avoid promoting or benefiting from unauthorized sharing. Its design and messaging should encourage lawful and responsible use.

A second concern is academic integrity. Students could misuse the platform to distribute quiz answers, exam answers, plagiarized notes, or unauthorized assignment materials. StudentShare must make clear that convenient sharing does not mean every document is appropriate to upload.

A third concern is privacy. Students may accidentally share names, grades, email addresses, student identification numbers, or other personal information. Students need clear privacy settings and meaningful control over who can access their files.

A fourth concern is fairness. An automated detection system may incorrectly flag original notes or authorized materials. Automatically removing content without an explanation or appeal could unfairly restrict students from sharing legitimate resources.

These issues connect to the ACM Code of Ethics. Computing professionals should avoid adverse impacts, respect privacy, respect the work required to create original materials, and be honest and trustworthy with users [5].

## 4. Ethical Safeguards

StudentShare will provide clear rules before every upload or sharing action. The platform will explain that users should share only their own work, public-domain materials, or materials they have permission to distribute. Students will be shown a clear warning before they share a file, rather than being expected to locate the rules themselves.

The platform will include sharing controls so students can decide whether a document is private, limited to a selected group, or shared more broadly. Direct peer-to-peer transfers will not automatically create a permanent public copy of a file. Temporary cloud storage for failed transfers will be encrypted and deleted after a limited retention period. The optional sync feature will allow students to choose which folders, if any, are included.

StudentShare will also create a reporting and appeal process. Copyright owners, instructors, and students will be able to report concerns. The platform will acknowledge or respond to at least 90% of reports within 48 hours. When a system flags possible copyrighted or inappropriate content, StudentShare will explain why the content was flagged and give the user an opportunity to appeal.

When possible, a trained person will review flagged content before a final removal decision. This safeguard recognizes that automated systems can make mistakes. Students whose content is restricted will have an opportunity to explain whether they own the material or have permission to share it.

Several experts and stakeholders should help design these safeguards:

- A copyright or intellectual-property expert can advise the team about responsible sharing and reporting procedures.
- A university librarian can help identify legitimate academic resources, public-domain materials, and licensing options.
- An instructor or academic-integrity officer can advise the team about prohibited quiz, exam, and assignment materials.
- A privacy and cybersecurity expert can help protect user files, sharing codes, and personal information.
- Student representatives can test whether the rules and settings are understandable and accessible.

StudentShare can find these experts by working with university libraries, campus information-technology offices, instructors, accessibility offices, and qualified legal or privacy professionals. The company will measure the effectiveness of safeguards through report response times, appeal results, usability-test results, privacy-setting usage, and the number of repeated violations. These results will show whether the platform is balancing convenience with responsible sharing.

## Conclusion

StudentShare should be convenient and useful for students to share files while also respecting privacy, academic integrity, and the rights of creators. The platform should give students clear directions before they share documents, allow them to decide who can access their files, and provide a fair process for reporting concerns and submitting appeals.

My OKR supports StudentShare’s purpose by balancing convenience and accountability. Copyright reminders, privacy controls, timely report responses, usability testing, and human review when possible can help students collaborate without encouraging unauthorized sharing or unfairly restricting approved materials.

## References

[1] Mozilla Developer Network. “WebRTC API.” n.d. https://developer.mozilla.org/en-US/docs/Web/API/WebRTC_API

[2] U.S. Copyright Office. “What Is Copyright?” n.d. https://www.copyright.gov/what-is-copyright/

[3] Interaction Design Foundation. “Usability Testing.” 2026. https://ixdf.org/literature/topics/usability-testing

[4] Supreme Court of the United States. *Metro-Goldwyn-Mayer Studios Inc. v. Grokster, Ltd.* June 27, 2005. https://w2.eff.org/IP/P2P/MGM_v_Grokster/04-480.pdf

[5] Association for Computing Machinery. “ACM Code of Ethics and Professional Conduct.” 2018. https://www.acm.org/code-of-ethics
