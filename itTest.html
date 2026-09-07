import os

# HTML/CSS/JS single-file website code
web_code = """<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IT Fundamentals & Cybersecurity Interactive Assessment</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --card-border: #334155;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --accent: #0284c7;
            --accent-hover: #0369a1;
            --correct: #10b981;
            --correct-bg: rgba(16, 185, 129, 0.15);
            --wrong: #ef4444;
            --wrong-bg: rgba(239, 68, 68, 0.15);
            --selected: #3b82f6;
            --selected-bg: rgba(59, 130, 246, 0.15);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
        }

        header {
            width: 100%;
            max-width: 800px;
            margin-bottom: 24px;
            text-align: center;
            padding: 24px;
            background: var(--card-bg);
            border-radius: 12px;
            border: 1px solid var(--card-border);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.3);
        }

        header h1 {
            font-size: 1.8rem;
            color: var(--text-main);
            margin-bottom: 8px;
        }

        header p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .stats-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 100%;
            max-width: 800px;
            margin-bottom: 20px;
            background: var(--card-bg);
            padding: 12px 20px;
            border-radius: 8px;
            border: 1px solid var(--card-border);
        }

        .progress-container {
            width: 100%;
            max-width: 800px;
            background: var(--card-border);
            height: 8px;
            border-radius: 4px;
            margin-bottom: 24px;
            overflow: hidden;
        }

        .progress-bar {
            height: 100%;
            width: 0%;
            background: var(--accent);
            transition: width 0.3s ease;
        }

        .quiz-card {
            width: 100%;
            max-width: 800px;
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: 12px;
            padding: 28px;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.3);
        }

        .q-tag {
            display: inline-block;
            background: rgba(2, 132, 199, 0.2);
            color: #38bdf8;
            padding: 4px 10px;
            border-radius: 6px;
            font-size: 0.8rem;
            font-weight: 600;
            margin-bottom: 12px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .question-text {
            font-size: 1.15rem;
            font-weight: 500;
            line-height: 1.5;
            margin-bottom: 24px;
        }

        .options-list {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .option-btn {
            background: #0f172a;
            border: 1px solid var(--card-border);
            color: var(--text-main);
            padding: 14px 18px;
            border-radius: 8px;
            text-align: left;
            font-size: 1rem;
            cursor: pointer;
            transition: all 0.2s ease;
            display: flex;
            align-items: center;
        }

        .option-btn:hover:not(:disabled) {
            border-color: var(--accent);
            background: #1e293b;
        }

        .option-btn.selected {
            border-color: var(--selected);
            background: var(--selected-bg);
        }

        .option-btn.correct {
            border-color: var(--correct) !important;
            background: var(--correct-bg) !important;
            color: #6ee7b7 !important;
            font-weight: 600;
        }

        .option-btn.wrong {
            border-color: var(--wrong) !important;
            background: var(--wrong-bg) !important;
            color: #fca5a5 !important;
        }

        .btn-prefix {
            font-weight: 700;
            margin-right: 12px;
            color: var(--text-muted);
            min-width: 24px;
        }

        .controls {
            display: flex;
            justify-content: space-between;
            margin-top: 28px;
        }

        .nav-btn {
            background: var(--accent);
            color: white;
            border: none;
            padding: 12px 24px;
            border-radius: 8px;
            font-size: 0.95rem;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.2s;
        }

        .nav-btn:hover {
            background: var(--accent-hover);
        }

        .nav-btn:disabled {
            background: var(--card-border);
            color: var(--text-muted);
            cursor: not-allowed;
        }

        .results-container {
            display: none;
            text-align: center;
            width: 100%;
            max-width: 800px;
            background: var(--card-bg);
            border: 1px solid var(--card-border);
            border-radius: 12px;
            padding: 40px 28px;
        }

        .results-score {
            font-size: 3rem;
            font-weight: 700;
            color: var(--accent);
            margin: 16px 0;
        }

        .restart-btn {
            margin-top: 24px;
            background: var(--correct);
            color: white;
            border: none;
            padding: 14px 28px;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
        }

        @media (max-width: 600px) {
            body { padding: 12px; }
            .quiz-card { padding: 18px; }
            .question-text { font-size: 1rem; }
            .option-btn { font-size: 0.9rem; padding: 12px; }
        }
    </style>
</head>
<body>

    <header>
        <h1>IT Fundamentals & Cybersecurity Assessment</h1>
        <p>Interactive Practice Exam • Unit 1 & Chapter 3</p>
    </header>

    <div class="stats-bar" id="statsBar">
        <span id="questionNum">Question 1 of 60</span>
        <span id="scoreTracker">Score: 0</span>
    </div>

    <div class="progress-container">
        <div class="progress-bar" id="progressBar"></div>
    </div>

    <div class="quiz-card" id="quizCard">
        <div class="q-tag" id="topicTag">Topic Name</div>
        <div class="question-text" id="questionText">Question prompt goes here...</div>
        <div class="options-list" id="optionsList"></div>
        
        <div class="controls">
            <button class="nav-btn" id="prevBtn" onclick="prevQuestion()" disabled>Previous</button>
            <button class="nav-btn" id="nextBtn" onclick="nextQuestion()">Next Question</button>
        </div>
    </div>

    <div class="results-container" id="resultsContainer">
        <h2>Assessment Completed!</h2>
        <div class="results-score" id="finalScore">0 / 60</div>
        <p id="feedbackText">Great job testing your knowledge!</p>
        <button class="restart-btn" onclick="restartQuiz()">Retake Quiz</button>
    </div>

    <script>
        const questions = [
            { id: 1, topic: "Supercomputer Applications", q: "A meteorologist needs to execute complex numerical simulations to predict the path of a category 5 hurricane using millions of variables. Which class of computer is specifically designed for this level of intense computational task?", options: ["Mainframe Computer", "Supercomputer", "Enterprise Workstation", "Microcontroller"], answer: 1 },
            { id: 2, topic: "Mainframe Transaction Handling", q: "A major international bank handles millions of ATM transactions and credit card processing simultaneously across the globe without crashing. Which architecture is best suited for high-throughput transactional reliability?", options: ["Mainframe Computer", "Embedded System", "Personal Computer", "Quantum Simulator"], answer: 0 },
            { id: 3, topic: "Workstations for CAD/3D", q: "An architectural firm requires specialized hardware with a high-end GPU and ECC RAM to render complex 3D CAD models smoothly for clients. Which machine type fits this requirement best?", options: ["Supercomputer", "Workstation", "Microcontroller", "Mainframe"], answer: 1 },
            { id: 4, topic: "Microcontrollers & Embedded OS", q: "An engineer is designing an automated washing machine that monitors water level, temperature, and spin cycles using a tiny integrated circuit. What type of computer system is being used?", options: ["Server", "Workstation", "Microcontroller / Embedded System", "Mainframe"], answer: 2 },
            { id: 5, topic: "Data vs. Information Processing", q: "A hospital administrator enters raw numbers representing patient heart rates into a dashboard, which compiles them into a trend graph showing critical spike patterns. The trend graph represents:", options: ["Data", "Information", "Hardware", "Firmware"], answer: 1 },
            { id: 6, topic: "RAM Volatility & Power Loss", q: "While working on a lengthy document, Sarah experiences a sudden power outage. When her computer restarts, the unsaved last two pages are lost. Which component held the unsaved data?", options: ["Hard Disk Drive (HDD)", "Read-Only Memory (ROM)", "Random Access Memory (RAM)", "Solid State Drive (SSD)"], answer: 2 },
            { id: 7, topic: "Firmware / BIOS Execution", q: "When turning on a laptop, the screen initially displays a manufacturer logo and initializes the essential hardware components before loading the OS. What stored instructions execute this initial process?", options: ["System Software in RAM", "Firmware / BIOS stored in ROM", "Application Software on NVMe", "Utility Software in Cache"], answer: 1 },
            { id: 8, topic: "SSD vs HDD Performance", q: "A video editor notices that rendering files takes too long because files are stored on a mechanical magnetic drive with moving parts. Upgrading to which non-volatile flash storage would drastically improve read/write speed?", options: ["DRAM", "Solid State Drive (SSD)", "Optical Disk (BD-RE)", "SRAM"], answer: 1 },
            { id: 9, topic: "Phishing Attacks", q: "An employee receives an email appearing to come from the company IT department, asking them to click a link to re-verify their credentials immediately. What type of attack is this?", options: ["Ransomware", "Phishing", "Man-in-the-Middle", "Distributed Denial of Service"], answer: 1 },
            { id: 10, topic: "Ransomware Identification", q: "A company’s main files suddenly become inaccessible, replaced with .locked extensions and a text file demanding cryptocurrency payment for decryption keys. What malware infected the system?", options: ["Spyware", "Keylogger", "Ransomware", "Adware"], answer: 2 },
            { id: 11, topic: "DDoS Attack Vectors", q: "An e-commerce platform becomes completely unreachable during Black Friday because millions of fake request packets flood its web server simultaneously from thousands of infected IoT devices. This is a:", options: ["Phishing attack", "Distributed Denial of Service (DDoS) attack", "Trojan attack", "SQL Injection attack"], answer: 1 },
            { id: 12, topic: "Tailgating & Social Engineering", q: "A hacker poses as an IT technician in a company lobby, holding a box and asking an employee to hold the secure electronic door open for them. This psychological manipulation technique is known as:", options: ["Tailgating / Social Engineering", "Port Scanning", "Zero-Day Exploit", "Spoofing"], answer: 0 },
            { id: 13, topic: "Digital Footprint & Online Presence", q: "A job candidate is surprised when an interviewer brings up controversial blog comments they posted five years ago under their full name. This scenario demonstrates the permanence of a person’s:", options: ["Digital Divide", "Digital Footprint", "Net Neutrality", "Encrypted Cache"], answer: 1 },
            { id: 14, topic: "The Digital Divide", q: "A rural school district lacks high-speed fiber internet and modern computers, placing its students at a disadvantage compared to urban students with high-speed access. What issue does this highlight?", options: ["Digital Divide", "Computer Ethics", "Net Rights Violation", "Algorithmic Bias"], answer: 0 },
            { id: 15, topic: "OS Multitasking & Multi-user", q: "An IT administrator needs an operating system that allows multiple administrative users to execute commands, allocate CPU resources, and run background services concurrently. This capability is called:", options: ["Multitasking & Multi-user support", "Single-user execution", "Dual-core virtualization", "File Compression"], answer: 0 },
            { id: 16, topic: "Device Drivers Functions", q: "A user plugs a brand-new graphics card into their desktop motherboard, but the OS fails to utilize its advanced features until a specific piece of hardware-translating software is installed. This software is a:", options: ["Utility Program", "Device Driver", "Firmware Upgrade", "Application Patch"], answer: 1 },
            { id: 17, topic: "Lossless vs Lossy Compression", q: "A graphics designer wants to compress a set of high-resolution JPEG photos to send via email, but needs to make sure no image quality or pixel data is permanently lost upon extraction. Which compression method is appropriate?", options: ["Lossy Compression", "Lossless Compression", "Destructive Archiving", "Downsampling"], answer: 1 },
            { id: 18, topic: "Open Source Software (OSS)", q: "A developer chooses to download an open-source web server application because they need to modify its underlying source code to add custom security features. What license type permits this?", options: ["Proprietary / Commercial", "Open Source Software (OSS)", "Shareware", "Freeware (Closed Source)"], answer: 1 },
            { id: 19, topic: "Spreadsheet Software Applications", q: "A financial team needs to build dynamic financial models with complex mathematical formulas, cross-sheet references, and automatic sum calculations. What software class should they use?", options: ["Word Processor", "Database Management System", "Spreadsheet Application", "Presentation Software"], answer: 2 },
            { id: 20, topic: "Database Management (DBMS)", q: "A university registry manages hundreds of thousands of student records, requiring strict relational structures, query capabilities, and data integrity constraints. Which software is best suited?", options: ["Database Management System (DBMS)", "Spreadsheet Application", "Desktop Publishing Application", "Utility Suite"], answer: 0 },
            { id: 21, topic: "Boot Process (POST)", q: "During a system boot, the computer checks hardware integrity through POST before loading the kernel into memory. What does POST stand for?", options: ["Power-On Self Test", "Primary Operation System Test", "Pre-Operational System Check", "Program Output Control Test"], answer: 0 },
            { id: 22, topic: "Shareware Licensing Model", q: "A software company releases a free 30-day trial version of its video editing tool, after which users must purchase a license key to continue using advanced features. What distribution model is this?", options: ["Freeware", "Shareware", "Open Source", "Public Domain"], answer: 1 },
            { id: 23, topic: "Cloud Computing / SaaS", q: "A corporate user logs into an online portal where they can create documents and store spreadsheets directly over the web without installing software locally. This is an example of:", options: ["Cloud Computing / SaaS", "On-Premise Virtualization", "Embedded System Operations", "Firmware Execution"], answer: 0 },
            { id: 24, topic: "Secure Data Destruction", q: "An individual wants to ensure that a discarded hard drive cannot be read by third parties. What action provides the highest data destruction assurance?", options: ["Deleting all files to Recycle Bin", "Quick Formatting the drive", "Physical destruction or degaussing", "Renaming the system folder"], answer: 2 },
            { id: 25, topic: "Network Firewalls", q: "A network technician installs a dedicated hardware appliance between the internal corporate network and the internet to filter incoming traffic based on security rules. This device is a:", options: ["Network Bridge", "Firewall", "Repeater", "Modem"], answer: 1 },
            { id: 26, topic: "Credential Harvesting / Phishing", q: "An employee receives an email containing a link that looks identical to their corporate login page: www.updaate-company.com. Entering credentials here would lead to:", options: ["Credential Harvesting via Phishing", "Automated Patch Management", "Secure Single Sign-On", "DNS Amplification"], answer: 0 },
            { id: 27, topic: "Keyloggers & Spyware", q: "A system administrator notices that a server is sluggish. Inspection reveals a rogue background program silently recording every keystroke typed by the root user. What type of threat is this?", options: ["Ransomware", "Keylogger / Spyware", "Worm", "Logic Bomb"], answer: 1 },
            { id: 28, topic: "Worms vs Computer Viruses", q: "Unlike a traditional computer virus, a malicious software program spreads automatically across a corporate network without requiring any user action or host file execution. This threat is a:", options: ["Computer Worm", "Macro Virus", "Trojan Horse", "Adware"], answer: 0 },
            { id: 29, topic: "Trojan Horse Identification", q: "A user downloads what appears to be a free utility software for PC optimization, but running the installer secretly installs a background backdoor. This software is classified as a:", options: ["Rootkit", "Trojan Horse", "Boot Sector Virus", "Keylogger"], answer: 1 },
            { id: 30, topic: "Multi-Factor Authentication (MFA)", q: "A cybersecurity manager mandates that all corporate logins require a password, a physical security key, and a fingerprint scan. This security framework is called:", options: ["Single-Factor Authentication", "Multi-Factor Authentication (MFA)", "Biometric Encryption", "Passcode Redundancy"], answer: 1 },
            { id: 31, topic: "Data Encryption Principles", q: "A user sets up a wireless router and enables standard encryption to scramble wireless data packets so unauthorized neighbors cannot intercept sensitive web sessions. This process is:", options: ["Data Decryption", "Encryption", "Compression", "Defragmentation"], answer: 1 },
            { id: 32, topic: "Ethical Hacking (White Hat)", q: "An ethical hacker is hired by a firm to attempt penetrating their network perimeter to identify security vulnerabilities before cybercriminals exploit them. The ethical hacker is a:", options: ["Black Hat Hacker", "White Hat Hacker", "Script Kiddie", "Hacktivist"], answer: 1 },
            { id: 33, topic: "Academic Integrity / Plagiarism", q: "A student copies several paragraphs directly from a research website into their final term paper without quoting or citing the author, claiming the work as their own. This violates academic integrity via:", options: ["Copyright Infringement", "Plagiarism", "Digital Piracy", "Slander"], answer: 1 },
            { id: 34, topic: "Intellectual Property & Copyright", q: "A user downloads illegally cracked commercial CAD software from an untrusted torrent site. Aside from security risks, this unauthorized distribution violates:", options: ["Public Domain Rights", "Intellectual Property & Copyright Laws", "Fair Use Protocols", "Net Neutrality Standards"], answer: 1 },
            { id: 35, topic: "Disk Defragmentation Utility", q: "A computer technician notices that an OS is running slow due to fragmented sectors spread across a mechanical hard drive. Which utility software should be executed?", options: ["Disk Defragmenter", "Disk Cleanup", "Antivirus Scanner", "Partition Assistant"], answer: 0 },
            { id: 36, topic: "Virtual Memory Management", q: "When a computer's physical RAM becomes completely full from running multiple heavy apps, the OS temporary uses a reserved section of the storage drive as:", options: ["Read-Only Memory", "Virtual Memory", "Flash Cache", "Firmware Expansion"], answer: 1 },
            { id: 37, topic: "Disaster Recovery & Off-site Backups", q: "A small business wants to ensure their systems can recover quickly if their primary server hardware completely fails or is destroyed in a fire. What backup strategy component is vital?", options: ["On-site Local Temp Cache", "Off-site / Cloud Data Backup", "System Restore Points on the same drive", "RAID 0 Mirroring"], answer: 1 },
            { id: 38, topic: "CPU Architecture (ALU)", q: "Which fundamental component of the CPU is responsible for performing mathematical calculations (e.g., addition, subtraction) and logical evaluations (e.g., AND, OR)?", options: ["Control Unit (CU)", "Arithmetic Logic Unit (ALU)", "Register File", "System Bus"], answer: 1 },
            { id: 39, topic: "CPU Control Unit (CU)", q: "Which component of the CPU acts as the supervisor, directing the flow of data and instructions between the CPU, memory, and input/output devices?", options: ["Arithmetic Logic Unit", "Control Unit", "L3 Cache", "BIOS Chip"], answer: 1 },
            { id: 40, topic: "CPU Clock Speed (GHz)", q: "A computer buyer sees a processor spec listed as 3.8 GHz. What does this clock speed metric measure?", options: ["The total memory bandwidth", "The number of instruction cycles per second", "The physical temperature threshold", "The maximum storage capacity"], answer: 1 },
            { id: 41, topic: "Cache Memory Hierarchy", q: "Which type of memory is directly built onto or adjacent to the CPU die, providing ultra-fast access speed to frequently used instructions?", options: ["Cache Memory", "Virtual Memory", "Secondary Storage", "CMOS Memory"], answer: 0 },
            { id: 42, topic: "Input Devices (Barcode Scanner)", q: "A worker uses a barcode scanner at a retail checkout counter to scan items. The barcode scanner functions as what type of hardware device?", options: ["Output Device", "Input Device", "Processing Unit", "Storage Device"], answer: 1 },
            { id: 43, topic: "Output Devices (3D Printers)", q: "A 3D printer creates physical prototype components layer-by-layer based on digital CAD blueprints. The 3D printer acts as a(n):", options: ["Input Device", "Output Device", "Storage Device", "System Control Unit"], answer: 1 },
            { id: 44, topic: "Presentation Software", q: "An office manager wants software that allows them to create sleek presentation slides containing embedded videos, transitions, and bullet points for board meetings. They should use:", options: ["Desktop Publishing Software", "Presentation Software", "Word Processing Software", "Spreadsheet Software"], answer: 1 },
            { id: 45, topic: "Vector Graphics Software", q: "A graphic designer works with vector images that can scale infinitely without pixelation or loss of quality. What tool is designed for vector artwork design?", options: ["Vector Illustration Software", "Raster Photo Editor", "CAD Application", "DBMS Utility"], answer: 0 },
            { id: 46, topic: "Computer-Aided Design (CAD)", q: "A civil engineer needs software to design detailed geometric layouts, structural dimensions, and architectural blueprints for a new bridge. What application category is required?", options: ["Computer-Aided Design (CAD)", "Computer-Aided Manufacturing (CAM)", "Presentation Graphics", "Desktop Publishing"], answer: 0 },
            { id: 47, topic: "EULA & Licensing Compliance", q: "A company policy prohibits downloading pirated software, stating that software usage must adhere to terms specified in the software license agreement known as:", options: ["EULA (End User License Agreement)", "SLA (Service Level Agreement)", "NDA (Non-Disclosure Agreement)", "GPL (General Protection Limit)"], answer: 0 },
            { id: 48, topic: "Vishing (Voice Phishing)", q: "An employee receives an unexpected call from someone claiming to be from the IT Help Desk, asking for their password to fix an urgent account error. This attack is:", options: ["Vishing (Voice Phishing)", "Shoulder Surfing", "Dumpster Diving", "Man-in-the-Middle"], answer: 0 },
            { id: 49, topic: "Shoulder Surfing", q: "A malicious actor stands behind an ATM user and discreetly records their PIN code as it is typed into the numeric keypad. What social engineering physical attack is this?", options: ["Piggybacking", "Shoulder Surfing", "Pretexting", "Baiting"], answer: 1 },
            { id: 50, topic: "Baiting Social Engineering", q: "An attacker leaves a virus-infected USB flash drive labeled 'Executive Salaries Q4' in a corporate breakroom, hoping a curious employee plugs it into a workstation. This attack is:", options: ["Baiting", "Phishing", "Scareware", "Watering Hole Attack"], answer: 0 },
            { id: 51, topic: "Scareware Malware Tactics", q: "A web browser pop-up suddenly warns a user that their computer is infected with 15 viruses and urges them to immediately download a specific cleaning utility, which is actually malware. This tactic is:", options: ["Ransomware", "Scareware", "Spyware", "Rootkit"], answer: 1 },
            { id: 52, topic: "Operating System Kernel", q: "Which operating system component is responsible for managing system memory, CPU tasks, hardware communication, and low-level system calls directly with hardware?", options: ["User Interface (UI)", "Kernel", "File Manager", "Bootloader"], answer: 1 },
            { id: 53, topic: "Command-Line Interface (CLI)", q: "An operating system interface that requires users to type text commands sequentially at a prompt without graphical windows or icons is called a:", options: ["Graphical User Interface (GUI)", "Command-Line Interface (CLI)", "Touch User Interface (TUI)", "Natural Language Interface (NLI)"], answer: 1 },
            { id: 54, topic: "Graphical User Interface (GUI)", q: "A mobile phone operating system like Android or iOS uses icons, gestures, windows, and visual menus. This type of user interaction environment is known as a:", options: ["Command Line Interface", "Graphical User Interface (GUI)", "Batch Processing System", "Text-based Interface"], answer: 1 },
            { id: 55, topic: "Print Spooling Management", q: "When a printer is sent multiple document jobs from different users simultaneously, the OS organizes them into a print queue in memory. This process is known as:", options: ["Spooling", "Buffering", "Caching", "Paging"], answer: 0 },
            { id: 56, topic: "File Compression Utilities", q: "A user wants to archive an entire folder containing 50 Word documents into a single, smaller zip file for easier email delivery. What system tool performs this task?", options: ["File Compression Utility", "Disk Defragmenter", "System Restore Utility", "Firewall Manager"], answer: 0 },
            { id: 57, topic: "Antivirus Scanning Utilities", q: "A system utility that regularly checks software files against a library of known malware signatures to isolate threats is an:", options: ["Antivirus / Anti-malware Utility", "Intrusion Prevention System", "Encryption Engine", "Disk Cleanup Utility"], answer: 0 },
            { id: 58, topic: "Public Domain Licensing", q: "A software developer releases software for free under a public domain dedication, completely waiving copyright rights. Anyone can use, modify, or sell it without restrictions. This is:", options: ["Commercial Software", "Public Domain Software", "Shareware", "Proprietary Software"], answer: 1 },
            { id: 59, topic: "Software License Agreements (EULA)", q: "A user is installing software and is asked to accept terms stating they cannot reverse engineer, resell, or distribute the software binary. This document is the:", options: ["End-User License Agreement (EULA)", "General Public License (GPL)", "Privacy Policy", "Service Level Agreement (SLA)"], answer: 0 },
            { id: 60, topic: "Cloud Models (IaaS)", q: "A cloud service provides access to virtual infrastructure, storage, and networking hardware over the internet where administrators configure their own operating systems. This cloud model is:", options: ["Software as a Service (SaaS)", "Infrastructure as a Service (IaaS)", "Platform as a Service (PaaS)", "Function as a Service (FaaS)"], answer: 1 }
        ];

        let currentIdx = 0;
        let userAnswers = new Array(questions.length).fill(null);

        function renderQuestion() {
            const qData = questions[currentIdx];
            
            document.getElementById("topicTag").innerText = qData.topic;
            document.getElementById("questionNum").innerText = `Question ${currentIdx + 1} of ${questions.length}`;
            document.getElementById("questionText").innerText = qData.q;
            
            const optionsContainer = document.getElementById("optionsList");
            optionsContainer.innerHTML = "";

            const labels = ["A", "B", "C", "D"];
            
            qData.options.forEach((opt, idx) => {
                const btn = document.createElement("button");
                btn.className = "option-btn";
                
                if (userAnswers[currentIdx] !== null) {
                    if (idx === qData.answer) {
                        btn.classList.add("correct");
                    } else if (idx === userAnswers[currentIdx]) {
                        btn.classList.add("wrong");
                    }
                    btn.disabled = true;
                }

                btn.innerHTML = `<span class="btn-prefix">${labels[idx]})</span> ${opt}`;
                btn.onclick = () => selectOption(idx);
                optionsContainer.appendChild(btn);
            });

            // Update progress & buttons
            document.getElementById("progressBar").style.width = `${((currentIdx + 1) / questions.length) * 100}%`;
            document.getElementById("prevBtn").disabled = currentIdx === 0;
            
            if (currentIdx === questions.length - 1) {
                document.getElementById("nextBtn").innerText = "Finish Quiz";
            } else {
                document.getElementById("nextBtn").innerText = "Next Question";
            }

            updateScoreDisplay();
        }

        function selectOption(idx) {
            if (userAnswers[currentIdx] === null) {
                userAnswers[currentIdx] = idx;
                renderQuestion();
            }
        }

        function updateScoreDisplay() {
            let score = 0;
            userAnswers.forEach((ans, i) => {
                if (ans === questions[i].answer) score++;
            });
            document.getElementById("scoreTracker").innerText = `Score: ${score}`;
        }

        function nextQuestion() {
            if (currentIdx < questions.length - 1) {
                currentIdx++;
                renderQuestion();
            } else {
                showResults();
            }
        }

        function prevQuestion() {
            if (currentIdx > 0) {
                currentIdx--;
                renderQuestion();
            }
        }

        function showResults() {
            document.getElementById("quizCard").style.display = "none";
            document.getElementById("statsBar").style.display = "none";
            document.querySelector(".progress-container").style.display = "none";
            
            let finalScore = 0;
            userAnswers.forEach((ans, i) => {
                if (ans === questions[i].answer) finalScore++;
            });

            document.getElementById("resultsContainer").style.display = "block";
            document.getElementById("finalScore").innerText = `${finalScore} / ${questions.length}`;

            let percentage = (finalScore / questions.length) * 100;
            let feedback = "";
            if (percentage >= 90) feedback = "Outstanding performance! You have mastered these IT fundamentals.";
            else if (percentage >= 75) feedback = "Great job! You have a solid grasp of IT & Cybersecurity concepts.";
            else if (percentage >= 50) feedback = "Good effort! Review the questions you missed to sharpen your skills.";
            else feedback = "Keep practicing! Review Unit 1 & Chapter 3 concepts and try again.";

            document.getElementById("feedbackText").innerText = feedback;
        }

        function restartQuiz() {
            currentIdx = 0;
            userAnswers = new Array(questions.length).fill(null);
            document.getElementById("quizCard").style.display = "block";
            document.getElementById("statsBar").style.display = "flex";
            document.querySelector(".progress-container").style.display = "block";
            document.getElementById("resultsContainer").style.display = "none";
            renderQuestion();
        }

        // Initial render
        renderQuestion();
    </script>
</body>
</html>
"""

with open("index.html", "w", encoding="utf-8") as f:
    f.write(web_code)

print("HTML site created.")