\documentclass[letterpaper,11pt]{article}

\usepackage[empty]{fullpage}
\usepackage{titlesec}
\usepackage{marvosym}
\usepackage[usenames,dvipsnames]{color}
\usepackage{enumitem}
\usepackage[hidelinks]{hyperref}
\usepackage{fancyhdr}
\usepackage[english]{babel}
\usepackage{tabularx}
\usepackage{fontawesome5}
\input{glyphtounicode}

\hypersetup{
  colorlinks=true,
  urlcolor=blue,
}

\pagestyle{fancy}
\fancyhf{}
\fancyfoot{}
\renewcommand{\headrulewidth}{0pt}
\renewcommand{\footrulewidth}{0pt}

% Adjust margins
\addtolength{\oddsidemargin}{-0.6in}
\addtolength{\evensidemargin}{-0.5in}
\addtolength{\textwidth}{1.19in}
\addtolength{\topmargin}{-.7in}
\addtolength{\textheight}{1.4in}

\urlstyle{same}

\raggedbottom
\raggedright
\setlength{\tabcolsep}{0in}

% Section formatting
\titleformat{\section}{
  \vspace{-4pt}\scshape\raggedright\large\bfseries
}{}{0em}{}[\color{black}\titlerule \vspace{-5pt}]

% Make PDF machine-readable
\pdfgentounicode=1

% Custom commands
\newcommand{\resumeItem}[1]{\item\small{{#1 \vspace{-2pt}}}}
\newcommand{\resumeSubheading}[4]{
  \vspace{-2pt}\item
    \begin{tabular*}{1.0\textwidth}[t]{l@{\extracolsep{\fill}}r}
      \textbf{#1} & \textbf{\small #2} \\
      \textit{\small#3} & \textit{\small #4} \\
    \end{tabular*}\vspace{-7pt}
}

\newcommand{\resumeProjectHeading}[2]{
  \item
  \begin{tabular*}{1.0\textwidth}{l@{\extracolsep{\fill}}r}
    \small#1 & \textbf{\small #2} \\
  \end{tabular*}\vspace{-7pt}
}

\renewcommand\labelitemi{$\vcenter{\hbox{\tiny$\bullet$}}$}
\newcommand{\resumeSubHeadingListStart}{\begin{itemize}[leftmargin=0.0in, label={}]}
\newcommand{\resumeSubHeadingListEnd}{\end{itemize}}
\newcommand{\resumeItemListStart}{\begin{itemize}}
\newcommand{\resumeItemListEnd}{\end{itemize}\vspace{-5pt}}

%-------------------------------------------
%%%%%%  RESUME STARTS HERE  %%%%%%%%%%%%%%%%%%%%%%%%%%%%

\begin{document}

%----------HEADING----------
\begin{center}
  {\Huge \scshape Gourab Singha} \\ \vspace{2pt}
  \small \raisebox{-0.1\height}\faPhone\ +91-8794451269 ~ 
  \href{mailto:gaurabsingha16@gmail.com}{\raisebox{-0.2\height}\faEnvelope\ \underline{gaurabsingha16@gmail.com}} ~
  \href{https://www.linkedin.com/in/gourab-singha-6a0690245/}{\raisebox{-0.2\height}\faLinkedin\ \underline{LinkedIn}} ~
  \href{https://github.com/gourabsingha1}{\raisebox{-0.2\height}\faGithub\ \underline{GitHub}} ~
  \href{https://portfolio-one-kappa-34.vercel.app/}{\raisebox{-0.2\height}\faLink\ \underline{Portfolio}}
\end{center}

%-----------EDUCATION-----------
\section{Education}
\resumeSubHeadingListStart
  \resumeSubheading
    {National Institute of Technology (NIT), Agartala}{2021 -- 2025}
    {Bachelor of Technology in Computer Science and Engineering}{CGPA: 8.0/10.0}
\resumeSubHeadingListEnd

%-----------EXPERIENCE-----------
\section{Experience}
\resumeSubHeadingListStart

  \resumeSubheading
    {Visa}{June 2025 -- Present}
    {Software Engineer}{Bangalore, India}
    \resumeItemListStart
      \resumeItem{{\bf Real-Time Data Platform:} Architected an event-driven {\bf Auth \& Settlement pipeline} using {\bf Kafka and Spring Boot}, processing {\bf millions of transactions/month} with auth-settlement matching, cross-DC resilience, and deduplication guarantees, ensuring {\bf financial-grade consistency at scale}.}
      
      \resumeItem{{\bf Legacy Modernization:} Analyzed and explained {\bf 15K+ lines} of complex SQL to facilitate the ETL migration to a Fast Data Architecture, and built the {\bf Audit service from scratch in Java}, tracking and handling {\bf 500K+ records/month}.}
      
      \resumeItem{{\bf Fault Tolerance:} Engineered a {\bf circuit-breaker-driven architecture} with {\bf tiered error classification} and {\bf system-level retries}, enabling {\bf 10s failure containment}, {\bf automatic back-pressure}, and {\bf zero data loss via DLQ}.}

      \resumeItem{{\bf Data Compare Tool:} Built a full-stack reconciliation platform ({\bf React, Java, MySQL}) validating and comparing data across {\bf 50+ tables}, standardizing E2E testing and debugging.}

      \resumeItem{{\bf Compliance:} Implemented {\bf WCAG 2.2 accessibility standards} across critical user flows, ensuring inclusive design for global users with diverse navigation needs.}
    \resumeItemListEnd

  \resumeSubheading
    {CRED}{January 2025 -- June 2025}
    {Backend Engineer Intern}{Bangalore, India}
  \resumeItemListStart
  \resumeItem{{\bf Developer Productivity:} Built and drove adoption of a {\bf centralized metric publishing library}, reducing instrumentation effort by {\bf 87.5\%} (8 hrs $\rightarrow$ 1 hr) across distributed backend teams.}
  
  \resumeItem{{\bf Risk Mitigation:} Eliminated {\bf 2,000+ erroneous loan transitions/month} by enforcing {\bf runtime validations} and {\bf database-level constraints} within the core loan engine.}
  
  \resumeItem{{\bf Data Reliability:} Corrected large-scale financial inconsistencies impacting {\bf 10,000+ users} by designing {\bf automated Python orchestration pipelines} for interest recalculation.}
  
  \resumeItem{{\bf Compliance \& Payments Integration:} Partnered with {\bf Payments, Finance, and Legal} to implement {\bf AML-compliant workflows}, validated across {\bf UPI, AutoPay, Net Banking, Debit, and Credit Card} flows, ensuring {\bf 100\% regulatory adherence}.}
\resumeItemListEnd

\resumeSubHeadingListEnd

%-----------PROJECTS-----------
\section{Projects}
\resumeSubHeadingListStart
  \resumeProjectHeading
    {{\href{https://github.com/gourabsingha1/Find-It}{\textbf{Find It}}} $|$ \emph{Kotlin, XML, Material Design, Firebase, Android Studio}}{November 2022}
  \resumeItemListStart
    \resumeItem{Leveraged \textbf{Google Maps API} to find products at the nearest store; implemented efficient location-based search.}
    \resumeItem{Implemented separation between UI and data layers; built \textbf{role-based user/admin sections}.}
  \resumeItemListEnd
  \resumeProjectHeading
    {{\href{https://github.com/gourabsingha1/MERN-E-Commerce-Backend}{\textbf{E-Commerce Backend}}} $|$ \emph{JavaScript, MongoDB, Express.js, Node.js}}{March 2024}
  \resumeItemListStart
    \resumeItem{Developed scalable \textbf{RESTful APIs} for product management, orders, and user sessions with auth and validation.}
    \resumeItem{Added health and metrics endpoints enabling basic monitoring and \textbf{readiness checks} for production deployments.}
  \resumeItemListEnd
\resumeSubHeadingListEnd

%-----------ACHIEVEMENTS-----------
\section{Achievements}
\vspace{-20pt}
\resumeSubHeadingListStart
  \resumeProjectHeading {}{}
    \resumeItemListStart
      \resumeItem{{\bf Guardian} on \href{https://leetcode.com/gourabsingha1/}{\bf LeetCode} (1800+ problems) with \href{https://drive.google.com/file/d/1sDLOh306Tom15Y1knU6rwFNDqKfaMg2g/view?usp=sharing}{\bf Global Rank 376} in contests.}
      \resumeItem{{\bf Expert} on \href{https://codeforces.com/profile/gourabsingha1}{\bf Codeforces} with 500+ problems solved.}
      \resumeItem{{\bf 5-star} on \href{https://www.codechef.com/users/gourabsingha2}{\bf CodeChef} (400+ problems) with \href{https://drive.google.com/file/d/1e8ORLtW6SqO8WDwINjQg2xKyH6dwzpWd/view?usp=sharing}{\bf Global Rank 3} and \href{https://drive.google.com/file/d/1fQjXsvZatdMw-A6mgFhKhmgvcceH5RzP/view?usp=sharing}{\bf Global Rank 27} in contests.}
      \resumeItem{Open-source contributor: {\bf OneBusAway-Android}, {\bf Anki-Android}.}
    \resumeItemListEnd
\resumeSubHeadingListEnd

%-----------TECHNICAL SKILLS-----------
\section{Technical Skills}
\begin{itemize}[leftmargin=0.15in, label={}]
  \small{\item{
    \textbf{Languages}{: C++, Java, C, Dart, Kotlin, Python, SQL, XML, HTML, CSS, JavaScript, TypeScript} \\
    \textbf{Tools}{: IntelliJ, VS Code, Android Studio, Docker, Kubernetes, Datagrip, GitHub, Postman, Grafana, Jenkins, Cursor} \\
    \textbf{Frameworks}{: Spring Boot, Flutter, Next.js, Angular, JUnit, Express.js, Node.js, React.js, React Native} \\
    \textbf{Cloud/Databases}{: Supabase, AWS, Kafka, Firebase, MySQL, PostgreSQL, MongoDB, Databricks} \\
    \textbf{Core Competencies}{: Distributed Systems, System Design, Technical Mentorship, Remote Collaboration, WCAG 2.2}
  }}
\end{itemize}

\end{document}