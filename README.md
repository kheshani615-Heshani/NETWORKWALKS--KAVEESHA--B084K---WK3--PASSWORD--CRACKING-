<div align="center">
  <h1>🔐 Week 3: PDF Password Cracking & Hash Extraction Lab</h1>
  
  <p><strong>Networkwalks Academy — Cybersecurity & Ethical Hacking Program</strong></p>

  <img src="https://img.shields.io/badge/Week-3%20Project-0A66C2?style=for-the-badge" alt="Week 3 Project">
    <img src="https://img.shields.io/badge/Module%201-John%20the%20Ripper%20%26%20Johnny-1F6FEB?style=for-the-badge" alt="W3-PM1">
    <img src="https://img.shields.io/badge/Module%202-Networkwalks%20NW%20Tools-8250DF?style=for-the-badge" alt="W3-PM2">
    <img src="https://img.shields.io/badge/Status-Completed-2EA043?style=for-the-badge" alt="Status Completed">
  </p>
</div>

<hr>
  <p>
    
  <img width="1920" height="1080" alt="w3 s1" src="https://github.com/user-attachments/assets/e97114e3-c0fa-4841-9a83-014b01bbaa35" />
    

  <img width="1920" height="1080" alt="w3 s12" src="https://github.com/user-attachments/assets/5a16401b-6181-4d3e-bed1-67a59bda5058" />
  

  <img width="1920" height="1080" alt="w3 s2" src="https://github.com/user-attachments/assets/ba65712a-4c03-4f5a-902d-41ae073f44f2" />

  </p>
</div>

<hr>

<h2>📋 Project Overview</h2>
<p>
  This repository documents the completion of the <strong>Week 3 Essential Project Modules</strong> for the Networkwalks Academy Cybersecurity Program. The objective of these labs is to demonstrate how password-protected documents store credentials as cryptographic hashes, how those hashes are extracted, and how dictionary attacks recover weak passwords—highlighting the importance of strong password policies.
</p>

<table>
  <thead>
    <tr>
      <th>Module Code</th>
      <th>Module Title</th>
      <th>Tools Used</th>
      <th>Target Files</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>W3-PM1</strong></td>
      <td>Password Cracking with JTR</td>
      <td>John the Ripper (1.9.0-jumbo-1), Johnny GUI, OnlineHashCrack PDF Extractor, Notepad</td>
      <td><code>My Locked PDF1.pdf</code>, <code>My Locked PDF2.pdf</code>, <code>My Locked PDF3.pdf</code></td>
      <td>✅ Completed</td>
    </tr>
    <tr>
      <td><strong>W3-PM2</strong></td>
      <td>Password Cracking with NW Tools</td>
      <td>Networkwalks Hash Calculator, Networkwalks Password Cracker (Browser-based)</td>
      <td><code>My Locked PDF1.pdf</code>, <code>My Locked PDF2.pdf</code>, <code>My Locked PDF3.pdf</code></td>
      <td>✅ Completed</td>
    </tr>
  </tbody>
</table>

<blockquote>
  <strong>⚠️ Legal & Ethical Disclaimer:</strong> All password recovery and hash extraction activities in this project were performed strictly within an authorized educational lab environment using Networkwalks training files.
</blockquote>

<hr>

<h2>🛠️ Module 1 (W3-PM1): Password Cracking with John the Ripper & Johnny</h2>

<h3>Step-by-Step Execution</h3>
<ol>
  <li>
    <strong>Environment Setup (JTR & Johnny GUI):</strong><br>
    Downloaded <code>John the Ripper 1.9.0-jumbo-1</code> (Windows 64-bit) and installed the <strong>Johnny GUI</strong> client. Configured Johnny under <em>Settings</em> by pointing the executable path to <code>run/john.exe</code> until Johnny confirmed: <code>Detected John the Ripper 1.9.0-jumbo-1 OMP</code>.
  </li>
  <li>
    <strong>PDF Hash Extraction:</strong><br>
    Uploaded each encrypted target file (<code>My Locked PDF1.pdf</code>, <code>My Locked PDF2.pdf</code>, and <code>My Locked PDF3.pdf</code>) to the OnlineHashCrack PDF Hash Extractor tool to extract their <code>$pdf$4*4*128*...</code> hashes.
  </li>
  <li>
    <strong>Hash Formatting & Storage:</strong><br>
    Copied each clean hash string starting directly with <code>$pdf$</code> (verifying no leading characters like <code>b'</code> were included) and saved them via Windows Notepad as <code>hash1.txt</code>, <code>hash2.txt</code>, and <code>hash3.txt</code>.
  </li>
  <li>
    <strong>Dictionary Attack via Johnny GUI:</strong><br>
    Loaded each hash file into Johnny using <em>Open password file → Open password file (PASSWD format)</em> and clicked <strong>Start new attack</strong> to recover the plaintext passwords.
  </li>
  <li>
    <strong>Document Decryption & Flag Capture:</strong><br>
    Entered each recovered password into its corresponding locked PDF file to unlock the document and capture the embedded flag.
  </li>
</ol>

<h3>📸 Module 1 Evidence & Screenshots</h3>
<table>
  <tr>
    <td align="center" width="50%">
      
  <img width="1920" height="1080" alt="w3 s1" src="https://github.com/user-attachments/assets/a865fb60-e73d-4663-9759-b2c9a6559a03" />

  <sub><b>1. Johnny GUI linked to john.exe</b></sub>
    </td>
    <td align="center" width="50%">
    
  <img width="1920" height="1080" alt="w3 s5" src="https://github.com/user-attachments/assets/be6db8b6-f0b2-47b3-830d-e56dc434d486" />

  <sub><b>2. Extracting $pdf$ Hash</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      
   <img width="1920" height="1080" alt="w3 s2" src="https://github.com/user-attachments/assets/b548a5f8-a851-4b9f-a604-9c66f6a6435f" />

  <sub><b>3. Cracking Hash in Johnny GUI</b></sub>
    </td>
    <td align="center" width="50%">
    
  <img width="1920" height="1080" alt="w3 s10" src="https://github.com/user-attachments/assets/6cc0b5eb-6e5d-4783-8c22-813a10f93f0f" />
  
<img width="1920" height="1080" alt="w3 s9" src="https://github.com/user-attachments/assets/bcfff744-9e2a-4fc6-888e-f1ab25cbf74e" />

  <sub><b>4. Unlocked PDF & Captured Flag</b></sub>
    </td>
  </tr>
</table>

<hr>

<h2>🌐 Module 2 (W3-PM2): Password Cracking with Networkwalks Tools</h2>

<h3>Step-by-Step Execution</h3>
<ol>
  <li>
    <strong>Download Target Files:</strong><br>
    Downloaded the encrypted lab files (<code>My Locked PDF1.pdf</code>, <code>My Locked PDF2.pdf</code>, and <code>My Locked PDF3.pdf</code>) from the Networkwalks project lab portal.
  </li>
  <li>
    <strong>Browser-Based Hash Extraction:</strong><br>
    Opened the <strong>Networkwalks Hash Calculator</strong> (<code>networkwalks.com/hash-calculator/</code>) and uploaded each locked PDF locally in the browser to extract its complete <code>$pdf$...</code> hash.
  </li>
  <li>
    <strong>Browser-Based Dictionary Attack:</strong><br>
    Opened the <strong>Networkwalks Password Cracker</strong> (<code>networkwalks.com/password-cracker/</code>), pasted each full <code>$pdf$...</code> hash string into the input box, and clicked <strong>START CRACKING</strong>.
  </li>
  <li>
    <strong>Verification & Unlocking:</strong><br>
    Copied the cracked plaintext passwords returned by the tool and unlocked all three PDF documents to verify access.
  </li>
</ol>

<h3>📸 Module 2 Evidence & Screenshots</h3>
<table>
  <tr>
    <td align="center" width="33%">
      
  <img width="1920" height="1080" alt="w3 s5" src="https://github.com/user-attachments/assets/37f46bab-b6be-4cc6-bfff-7d292934cf64" />

  
<img width="1920" height="1080" alt="w3 s4" src="https://github.com/user-attachments/assets/77cdff01-4b4f-4e23-935d-8915d83a006d" />

  <sub><b>1. NW Hash Calculator Output</b></sub>
    </td>
    <td align="center" width="33%">
    
  <img width="1920" height="1080" alt="w3 s8" src="https://github.com/user-attachments/assets/6f23d12a-dda0-4429-94b7-376ab5c064c0" />

  
<img width="1920" height="1080" alt="w3 s6" src="https://github.com/user-attachments/assets/dce9ba3c-ff35-4b13-9851-1eed39b802b7" />

  <sub><b>2. NW Password Cracker Match</b></sub>
    </td>
    <td align="center" width="33%">
    
  <img width="1920" height="1080" alt="w3 s10" src="https://github.com/user-attachments/assets/2d7ccef5-b700-4411-945a-0abb2c00b40a" />

  <sub><b>3. PDF Unlocked Successfully</b></sub>
    </td>
  </tr>
</table>

<hr>

<h2>🏆 Summary of Recovered Results</h2>
<table>
  <thead>
    <tr>
      <th>Target File</th>
      <th>Hash Format</th>
      <th>Recovered Password</th>
      <th>Captured Flag</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>My Locked PDF1.pdf</code></td>
      <td><code>$pdf$4*4*128*...</code> (128-bit)</td>
      <td><code>password1</code></td>
      <td><code>nw{cybersecurity_flag_captured_2608}</code></td>
    </tr>
    <tr>
      <td><code>My Locked PDF2.pdf</code></td>
      <td><code>$pdf$4*4*128*...</code> (128-bit)</td>
      <td><code>[Enter PDF2 Password]</code></td>
      <td><code>[Enter Flag 2]</code></td>
    </tr>
    <tr>
      <td><code>My Locked PDF3.pdf</code></td>
      <td><code>$pdf$4*4*128*...</code> (128-bit)</td>
      <td><code>[Enter PDF3 Password]</code></td>
      <td><code>[Enter Flag 3]</code></td>
    </tr>
  </tbody>
</table>

<hr>

<h2>🔧 Troubleshooting & Lessons Learned</h2>
<ul>
  <li>
    <strong>Locating <code>john.exe</code> when Windows Hides File Extensions:</strong><br>
    <em>Issue:</em> When browsing the <code>run</code> folder inside Johnny's Settings dialog, multiple applications appeared as <code>john</code>, <code>john-avx</code>, and <code>john-sse41</code> without visible <code>.exe</code> extensions.<br>
    <em>Solution:</em> Identified the primary executable by selecting the top <code>Application</code> entry named <code>john</code> (6,938 KB), which successfully linked <code>john.exe</code> to Johnny.
  </li>
  <li>
    <strong>Blank Password Column Before Starting Attack in Johnny:</strong><br>
    <em>Issue:</em> After importing <code>hash1.txt</code> into Johnny, the <em>Password</em> column remained blank initially.<br>
    <em>Solution:</em> Clicked <strong>Start new attack</strong> on the top toolbar to initiate John the Ripper's cracking session and populate the cracked password.
  </li>
  <li>
    <strong>Clean Hash Formatting:</strong><br>
    <em>Issue:</em> Extra prefix characters or truncated strings prevent hash crackers from recognizing PDF hashes.<br>
    <em>Solution:</em> Verified that every saved <code>.txt</code> hash file and pasted input began strictly with <code>$pdf$</code>.
  </li>
</ul>

<hr>

<h2>📚 Key Takeaways: Encryption vs. Hashing</h2>
<ul>
  <li><strong>Encryption (Two-Way):</strong> Protects sensitive file contents using an algorithm and a key/password; data can be decrypted back into plaintext when the valid key is supplied.</li>
  <li><strong>Hashing (One-Way):</strong> Converts a password into a fixed-format digest (such as <code>$pdf$...</code>) that cannot be mathematically reversed—attackers must test candidate passwords by hashing guesses until a digest match is found.</li>
  <li><strong>Defense Recommendation:</strong> Short, dictionary-based passwords (like <code>password1</code>) are cracked within seconds; using long, high-entropy passphrases (12+ mixed characters) mitigates offline and online dictionary attacks.</li>
</ul>

<div align="center">
  <p>Submitted by <strong>Kaveesha Heshani</strong> | Networkwalks Academy Cybersecurity Program</p>
</div>
