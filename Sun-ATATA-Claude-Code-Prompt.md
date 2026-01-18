# ATATA Website Development - Claude Code Prompt

## Project Overview

Create a professional, elegant website called **ATATA** (www.atata.com) to showcase and celebrate the achievements of Tamil Brahmins who have made significant contributions to society.

**ATATA** stands for **"Arun Thondu Attriya Thamizhaga Andhanarkal"** (அருந் தொண்டு ஆற்றிய தமிழக அந்தணர்கள்) - meaning "Tamil Brahmins who rendered rare service."

---

## Design Requirements

### Color Scheme (CSS Variables)
```css
--primary-gold: #C9A227;
--primary-maroon: #722F37;
--deep-maroon: #4A1C23;
--cream: #FDF8F0;
--warm-white: #FFFEF9;
--text-dark: #2C1810;
--text-medium: #5C4033;
--accent-copper: #B87333;
--border-gold: #D4AF37;
--shadow-warm: rgba(114, 47, 55, 0.15);
```

### Fonts
- **Headings**: Playfair Display (serif) - for elegant, traditional look
- **Body**: Source Sans Pro (sans-serif) - for readability
- **Tamil Text**: Noto Sans Tamil

### Overall Aesthetic
- Professional, dignified, and elegant
- Traditional yet modern feel
- Warm colors (maroon, gold, cream)
- Subtle gradients and shadows
- Smooth animations and transitions

---

## Page Structure

### 1. Header (Sticky)
- **Logo Emblem**: Circular gold badge with Tamil letter "அ" (for Andhanarkal)
- **Title**: "ATATA" in large Playfair Display font (gold color)
- **Subtitle**: Tamil text "அருந் தொண்டு ஆற்றிய தமிழக அந்தணர்கள்"
- **English Translation**: "(Arun Thondu Attriya Thamizhaga Andhanarkal - Tamil Brahmins who rendered rare service)"
- **Tagline** (right side): "Celebrating the extraordinary contributions of Tamil Brahmins to Science & Mathematics"
- Background: Deep maroon gradient

### 2. Main Layout (Two-Panel)

#### Left Sidebar (320px width, sticky)
- **Title**: "Distinguished Luminaries" with users icon
- **Collapsible Categories** with:
  - Category headers (maroon background, gold text)
  - Category icons (Font Awesome)
  - Expandable/collapsible person lists
  - Click to select a person and display profile
  - Active state indication

#### Right Content Area (Flexible width)
- **Welcome Screen** (default): Displays welcome message and instructions
- **Profile Card** (when person selected): Full profile display

### 3. Profile Card Structure
When a person is selected, display:

**Profile Header** (Maroon gradient background):
- Profile image (160x200px, gold border, rounded corners)
- Serial number badge (e.g., "SCI/01", "MTH/02")
- Full name
- Birth and death dates
- Brief tagline (first achievement)

**Profile Body** (Cream background):

**Info Grid** (2-column responsive grid):
1. **Birthplace Card**: Place and District
2. **Parents Card**: Father and Mother names
3. **Education - Schooling Card**: School details
4. **Education - College Card**: College/University details
5. **Career Card** (full width): Jobs and positions held

**Sections**:
1. **Key Achievements**: Bulleted list with decorative markers (✦)
2. **Impact on Society**: Paragraph describing contributions
3. **Awards & Recognition**: Horizontal flex grid of award badges (gold gradient)

**Action Buttons**:
- "Save as Image" (maroon, primary)
- "Save as PDF" (gold, secondary)
- "Share on WhatsApp" (green, WhatsApp brand)

### 4. Footer
- Visitor counter badge
- Copyright notice: "© 2026 ATATA - Arun Thondu Attriya Thamizhaga Andhanarkal"
- Developer credit: "Developed by Suraja Technologies | Powered by Jignyashika Consulting | Under the guidance of Dr. Sundararaman Chintamani"
- Image attribution disclaimer

---

## Categories and Profile Data

### Category 1: Science (SCI)
Icon: `fas fa-atom`

| # | Name | Serial |
|---|------|--------|
| 1 | Sir Chandrasekhara Venkata Raman (C.V. Raman) | SCI/01 |
| 2 | Dr. Subrahmanyan Chandrasekhar | SCI/02 |
| 3 | Sir Kariamanickam Srinivasa Krishnan (K.S. Krishnan) | SCI/03 |
| 4 | Dr. G. Srinivasan Venkataraman | SCI/04 |
| 5 | Prof. C. Mahadevan | SCI/05 |
| 6 | Dr. T.R. Govindachari | SCI/06 |
| 7 | Sir T.S. Venkataraman | SCI/07 |
| 8 | Dr. K. Venkataraman | SCI/08 |
| 9 | Prof. Gopalasamudram Narayana Ramachandran (G.N. Ramachandran) | SCI/09 |

### Category 2: Mathematics (MTH)
Icon: `fas fa-calculator`

| # | Name | Serial |
|---|------|--------|
| 1 | Shri Srinivasa Ramanujan | MTH/01 |
| 2 | Dr. Tirukkannapuram Vijayaraghavan | MTH/02 |
| 3 | Shri Raghava Sasthri | MTH/03 |
| 4 | Prof. V. Ganapathy Iyer | MTH/04 |

---

## Detailed Profile Data

### SCI/01 - Sir C.V. Raman
```javascript
{
  name: "Sir Chandrasekhara Venkata Raman",
  shortName: "Sir C.V. Raman",
  serial: "SCI/01",
  birth: "November 7, 1888",
  death: "November 21, 1970",
  birthPlace: "Tiruchirappalli, Tamil Nadu",
  district: "Tiruchirappalli District",
  parents: "Father: Chandrasekhar Ramanathan Iyer (Physics & Mathematics Lecturer), Mother: Parvathi Ammal",
  schooling: "St. Aloysius' Anglo-Indian High School, Visakhapatnam (Matriculated at age 11)",
  college: "Presidency College, Madras - B.A. (1904, age 16) & M.A. (1907, age 18)",
  jobs: "Indian Finance Department (1907-1917), Palit Professor of Physics at University of Calcutta (1917-1933), Director of Indian Institute of Science, Bangalore (1933-1948), Founder-Director of Raman Research Institute (1948-1970)",
  achievements: [
    "Discovered the Raman Effect (1928) - demonstrating that light changes wavelength when scattered through transparent materials",
    "First Asian and non-White person to win the Nobel Prize in Physics (1930)",
    "Founded the Indian Academy of Sciences (1934)",
    "Established the Raman Research Institute, Bangalore (1948)",
    "Founded the Indian Journal of Physics (1926)",
    "Pioneered research in acoustics, optics, and crystallography"
  ],
  impact: "Revolutionized spectroscopy and molecular analysis worldwide. The Raman Effect became a fundamental tool in chemistry, physics, and medicine for analyzing material composition. National Science Day (February 28) commemorates his discovery. Mentored future scientific leaders including Homi Bhabha and Vikram Sarabhai.",
  awards: ["Nobel Prize in Physics (1930)", "Bharat Ratna (1954)", "Lenin Peace Prize (1957)", "Fellow of the Royal Society (1924)", "Knighthood (1929)", "Hughes Medal"]
}
```

### SCI/02 - Dr. S. Chandrasekhar
```javascript
{
  name: "Dr. Subrahmanyan Chandrasekhar",
  shortName: "Dr. S. Chandrasekhar",
  serial: "SCI/02",
  birth: "October 19, 1910",
  death: "August 21, 1995",
  birthPlace: "Lahore, British India (now Pakistan)",
  district: "Tamil Brahmin family settled in Madras",
  parents: "Father: Chandrasekhara Subrahmanya Ayyar (Deputy Auditor General), Mother: Sita Balakrishnan (translated Ibsen's 'A Doll's House' into Tamil)",
  schooling: "Hindu High School, Madras",
  college: "Presidency College, Madras (1925-1930), Trinity College, Cambridge - PhD (1933)",
  jobs: "Fellow at Trinity College, Cambridge (1933-1937), University of Chicago - Professor of Astrophysics (1938-1995), Morton D. Hull Distinguished Service Professor",
  achievements: [
    "Chandrasekhar Limit - the maximum mass of a stable white dwarf star (~1.4 solar masses)",
    "Nobel Prize in Physics (1983) for theoretical studies of stellar structure and evolution",
    "Contributions to radiative transfer, stellar dynamics, and black hole theory",
    "Managing Editor of Astrophysical Journal for 19 years (1952-1971)",
    "Author of 'An Introduction to the Study of Stellar Structure' and other seminal works",
    "Nephew of Nobel Laureate C.V. Raman"
  ],
  impact: "Fundamentally changed our understanding of stellar evolution and the fate of massive stars. The Chandrasekhar Limit is crucial for understanding supernovae and neutron stars. NASA named the Chandra X-ray Observatory in his honor.",
  awards: ["Nobel Prize in Physics (1983)", "Copley Medal of Royal Society (1984)", "National Medal of Science, USA (1966)", "Padma Vibhushan (1968)", "Fellow of the Royal Society (1944)"]
}
```

### SCI/03 - Sir K.S. Krishnan
```javascript
{
  name: "Sir Kariamanickam Srinivasa Krishnan",
  shortName: "Sir K.S. Krishnan",
  serial: "SCI/03",
  birth: "December 4, 1898",
  death: "June 14, 1961",
  birthPlace: "Watrap, Tamil Nadu",
  district: "Virudhunagar District",
  parents: "Father: Srinivasa Iyer (Revenue Officer)",
  schooling: "Hindu High School, Srivilliputtur",
  college: "American College, Madurai - B.A. (1918), Madras Christian College - M.A. (1920)",
  jobs: "Assistant to C.V. Raman at IACS (1920-1928), Professor of Physics at University of Dacca (1928-1933), Professor at University of Allahabad (1933-1942), Director of National Physical Laboratory (1947-1961)",
  achievements: [
    "Co-discovered the Raman Effect with C.V. Raman (1928)",
    "Pioneering work in magnetism and crystal physics",
    "Established National Physical Laboratory, New Delhi as a premier research institution",
    "First Director of NPL and shaped India's measurement standards",
    "Pioneering research on magnetic anisotropy of crystals",
    "Significant contributions to theoretical physics"
  ],
  impact: "Played a crucial role in establishing India's scientific infrastructure. Built NPL into a world-class institution. His work on crystal physics and magnetism laid foundations for material science research in India.",
  awards: ["Fellow of the Royal Society (1940)", "Padma Bhushan (1954)", "Knighthood (1946)", "Bhatnagar Prize"]
}
```

### SCI/04 - Dr. G.S. Venkataraman
```javascript
{
  name: "Dr. G. Srinivasan Venkataraman",
  shortName: "Dr. G.S. Venkataraman",
  serial: "SCI/04",
  birth: "1932 (approx.)",
  death: "Living",
  birthPlace: "Tamil Nadu",
  district: "Tamil Nadu",
  parents: "Details being researched",
  schooling: "Details being researched",
  college: "M.Sc. from Madras University, Ph.D. from University of Pittsburgh",
  jobs: "Scientist at Bhabha Atomic Research Centre, Professor at Indian Institute of Science, Director of IGCAR, Distinguished Faculty at Sri Sathya Sai Institute",
  achievements: [
    "Pioneering research in condensed matter physics and lattice dynamics",
    "Contributions to understanding atomic movements in solids",
    "Renowned science communicator and author",
    "Former Director of Indira Gandhi Centre for Atomic Research",
    "Prolific writer on scientific and spiritual topics",
    "Combined scientific excellence with spiritual exploration"
  ],
  impact: "Made complex physics accessible through his writings and lectures. Bridged science and spirituality, inspiring a generation of scientists. His books on physics are used in institutions worldwide.",
  awards: ["Padma Shri", "S.N. Bose Medal", "Raja Ramanna Fellow", "Honorary Doctorates from multiple universities"]
}
```

### SCI/05 - Prof. C. Mahadevan
```javascript
{
  name: "Prof. Chitrabhanu Mahadevan",
  shortName: "Prof. C. Mahadevan",
  serial: "SCI/05",
  birth: "Details being researched",
  death: "Details being researched",
  birthPlace: "Tamil Nadu",
  district: "Tamil Nadu",
  parents: "Details being researched",
  schooling: "Details being researched",
  college: "Details being researched",
  jobs: "Details being researched",
  achievements: [
    "Contributed to scientific advancement in Tamil Nadu",
    "Research contributions being documented",
    "Note: This profile is under research - if you have biographical information about Prof. C. Mahadevan, please contact the ATATA team"
  ],
  impact: "Contributions being researched and documented.",
  awards: ["Details being researched"]
}
```

### SCI/06 - Dr. T.R. Govindachari
```javascript
{
  name: "Dr. Tiruvenkatacharya Rajagopalan Govindachari",
  shortName: "Dr. T.R. Govindachari",
  serial: "SCI/06",
  birth: "December 23, 1915",
  death: "January 13, 2001",
  birthPlace: "Thiruvananthapuram, Kerala",
  district: "Tamil Brahmin Family",
  parents: "Details being researched",
  schooling: "Details being researched",
  college: "Presidency College, Madras - M.Sc., University of Manchester - Ph.D. under Alexander Todd",
  jobs: "Professor at Presidency College, Head of CIBA Research Centre (Bombay), Consultant to pharmaceutical industry",
  achievements: [
    "One of India's greatest organic chemists",
    "Isolated and identified structures of over 150 alkaloids",
    "Pioneering work on Indian medicinal plants",
    "Authored over 400 research papers",
    "Developed new synthetic methodologies",
    "Trained generations of Indian chemists"
  ],
  impact: "Revolutionized the study of Indian medicinal plants. His work on alkaloids laid the foundation for pharmaceutical research in India. Created a school of natural product chemistry that continues to influence drug discovery.",
  awards: ["Shanti Swarup Bhatnagar Prize (1959)", "Fellow of the Royal Society (1972)", "Padma Bhushan (1974)", "INSA Award"]
}
```

### SCI/07 - Sir T.S. Venkataraman
```javascript
{
  name: "Sir Thiruvengadam Srinivasa Venkataraman",
  shortName: "Sir T.S. Venkataraman",
  serial: "SCI/07",
  birth: "1893",
  death: "1963",
  birthPlace: "Tamil Nadu",
  district: "Tamil Nadu",
  parents: "Details being researched",
  schooling: "Details being researched",
  college: "Cambridge University",
  jobs: "Director of Imperial Agricultural Research Institute, Director of Sugarcane Breeding Institute Coimbatore, Vice-Chancellor of Madras University",
  achievements: [
    "Father of the Indian Sugar Industry",
    "Developed high-yielding, disease-resistant sugarcane varieties (Co varieties)",
    "Revolutionized sugarcane cultivation in India",
    "Pioneering research in plant breeding",
    "Established scientific sugarcane breeding in India",
    "Transformed India from sugar importer to exporter"
  ],
  impact: "Single-handedly transformed India's sugar industry. The Co varieties he developed are used worldwide and form the basis of modern sugarcane cultivation. Saved India billions in sugar imports.",
  awards: ["Knighthood (1943)", "Fellow of the Royal Society", "Padma Vibhushan", "Several honorary doctorates"]
}
```

### SCI/08 - Dr. K. Venkataraman
```javascript
{
  name: "Dr. Krishnasami Venkataraman",
  shortName: "Dr. K. Venkataraman",
  serial: "SCI/08",
  birth: "June 7, 1901",
  death: "May 16, 1981",
  birthPlace: "Sattur, Tamil Nadu",
  district: "Virudhunagar District",
  parents: "Father: Krishnasami Iyer",
  schooling: "Sattur High School",
  college: "Madras University - M.Sc., Manchester University - D.Sc. under Robert Robinson",
  jobs: "Director of National Chemical Laboratory (1957-1966), Professor at University of Mumbai, Consultant to Dyestuffs industry",
  achievements: [
    "Pioneer in synthetic organic chemistry and natural product chemistry",
    "Authority on flavonoid chemistry - authored 'Chemistry of Flavonoid Compounds'",
    "Developed indigenous processes for dyes and pharmaceuticals",
    "Director of NCL during its formative years",
    "Authored over 500 research papers",
    "Trained hundreds of chemists"
  ],
  impact: "Made India self-reliant in dyes and intermediates. His work on flavonoids is a classic reference in the field. Established a strong tradition of organic chemistry research in India.",
  awards: ["Shanti Swarup Bhatnagar Prize", "Padma Bhushan (1961)", "Fellow of the Royal Society (1955)", "Acharya P.C. Ray Memorial Award"]
}
```

### SCI/09 - Prof. G.N. Ramachandran
```javascript
{
  name: "Prof. Gopalasamudram Narayana Ramachandran",
  shortName: "Prof. G.N. Ramachandran",
  serial: "SCI/09",
  birth: "October 8, 1922",
  death: "April 7, 2001",
  birthPlace: "Ernakulam, Kerala",
  district: "Tamil Brahmin family",
  parents: "Father: G.R. Narayana Iyer (Professor of Mathematics)",
  schooling: "Maharaja's College, Ernakulam",
  college: "Maharaja's College, Ernakulam - B.Sc. (1942), St. Stephen's College, Delhi - M.Sc. (1944), Cambridge University - Ph.D. under Raman (1949)",
  jobs: "Professor at University of Madras (1952-1970), Head of Molecular Biophysics Unit, IISc (1971-1978), Professor at University of Chicago",
  achievements: [
    "Created the Ramachandran Plot - fundamental tool for understanding protein structure",
    "Proposed the triple helical structure of collagen",
    "Founded molecular biophysics in India",
    "Pioneering work in X-ray crystallography",
    "Developed convolution and its applications",
    "Authored over 200 research papers"
  ],
  impact: "The Ramachandran Plot is used by every structural biologist worldwide. His work on collagen structure is fundamental to understanding connective tissue. Established the field of molecular biophysics in India.",
  awards: ["Fellow of the Royal Society (1977)", "Shanti Swarup Bhatnagar Prize (1961)", "Padma Bhushan", "Ewald Prize (International Union of Crystallography)", "Nominated for Nobel Prize multiple times"]
}
```

### MTH/01 - Shri Srinivasa Ramanujan
```javascript
{
  name: "Shri Srinivasa Ramanujan Iyengar",
  shortName: "Shri Srinivasa Ramanujan",
  serial: "MTH/01",
  birth: "December 22, 1887",
  death: "April 26, 1920",
  birthPlace: "Erode, Tamil Nadu",
  district: "Erode District",
  parents: "Father: Kuppuswamy Srinivasa Iyengar (Clerk in a sari shop), Mother: Komalatammal (Singer at local temple)",
  schooling: "Town Higher Secondary School, Kumbakonam - Passed primary with highest marks in the district",
  college: "Government Arts College, Kumbakonam (no degree), Pachaiyappa's College, Madras (no degree), Trinity College, Cambridge (B.A. by research, 1916)",
  jobs: "Clerk at Madras Port Trust (1912-1913), Research Scholar at University of Cambridge under G.H. Hardy (1914-1919)",
  achievements: [
    "Self-taught mathematical genius who produced nearly 3,900 results",
    "Groundbreaking contributions to number theory, infinite series, and continued fractions",
    "Hardy-Ramanujan Number (1729) - the first taxicab number",
    "Ramanujan Prime, Ramanujan Theta Function, and Mock Theta Functions",
    "Second Indian to be elected Fellow of the Royal Society (1918)",
    "First Indian to be elected Fellow of Trinity College"
  ],
  impact: "Considered one of the greatest mathematical geniuses in history. Hardy rated his pure talent at 100 on a scale where Hilbert scored 80. His discoveries continue to influence mathematics, physics, string theory, and computer science. December 22 is celebrated as National Mathematics Day in India.",
  awards: ["Fellow of the Royal Society (1918)", "Fellow of Trinity College Cambridge (1918)"]
}
```

### MTH/02 - Dr. T. Vijayaraghavan
```javascript
{
  name: "Dr. Tirukkannapuram Vijayaraghavan",
  shortName: "Dr. T. Vijayaraghavan",
  serial: "MTH/02",
  birth: "November 30, 1902",
  death: "April 20, 1955",
  birthPlace: "Adoor Agaram, Madras Presidency",
  district: "Tamil Nadu",
  parents: "Father: Tirukkannapuram Pattappa Swamy (Famous pandit and Sanskrit/Tamil scholar)",
  schooling: "Hindu Theological High School, Madras; Pachaiyappa's College (1918-1920)",
  college: "Presidency College, Madras - B.A. Honours & M.A. (1920-1924), Trinity College, Cambridge, Oxford University - D.Phil. under G.H. Hardy",
  jobs: "Lecturer at Aligarh Muslim University (1930-1931), Reader at University of Dacca (1931-1946), Professor of Mathematics at University of Madras, Director of Ramanujan Institute",
  achievements: [
    "Worked with G.H. Hardy on Pisot-Vijayaraghavan numbers",
    "Proved special case of Herschfeld's theorem on nested radicals",
    "Pioneering contributions to Diophantine approximation",
    "Foundation Fellow of Indian National Science Academy (1935)",
    "Close collaborator and friend of André Weil",
    "Well-versed in Sanskrit and Tamil literature alongside mathematics"
  ],
  impact: "Established analytical number theory traditions in India. His work on Pisot-Vijayaraghavan numbers remains fundamental in algebraic number theory. Mentored K. Chandrasekharan and influenced generations of Indian mathematicians.",
  awards: ["Fellow of Indian Academy of Sciences (1934)", "Foundation Fellow of INSA (1935)", "Member of London Mathematical Society (1925)"]
}
```

### MTH/03 - Shri Raghava Sasthri
```javascript
{
  name: "Shri Raghava Sasthri",
  shortName: "Shri Raghava Sasthri",
  serial: "MTH/03",
  birth: "Details being researched",
  death: "Details being researched",
  birthPlace: "Tamil Nadu (presumed)",
  district: "Tamil Nadu",
  parents: "Details being researched",
  schooling: "Traditional Gurukul education in Sanskrit and Mathematics",
  college: "Traditional scholarship (pre-modern era)",
  jobs: "Traditional scholar and mathematician",
  achievements: [
    "Traditional Tamil Brahmin mathematician combining Vedic and classical approaches",
    "Preserved and advanced traditional mathematical knowledge systems",
    "Contributed to mathematical scholarship in Tamil Nadu",
    "Note: This profile is under research - if you have biographical information about Shri Raghava Sasthri, please contact the ATATA team"
  ],
  impact: "Contributions being researched and documented.",
  awards: ["Details being researched"]
}
```

### MTH/04 - Prof. V. Ganapathy Iyer
```javascript
{
  name: "Prof. Venkatarama Ganapathy Iyer",
  shortName: "Prof. V. Ganapathy Iyer",
  serial: "MTH/04",
  birth: "1906",
  death: "1987",
  birthPlace: "Tamil Nadu",
  district: "Tamil Nadu",
  parents: "Details being researched",
  schooling: "Details being researched",
  college: "Madras University, Cambridge University",
  jobs: "Professor of Mathematics at Annamalai University, Head of Mathematics Department",
  achievements: [
    "Pioneering contributions to classical analysis and infinite series",
    "Work on summability methods and special functions",
    "Authored 'Lectures on Theory of Functions of a Complex Variable'",
    "Trained many research students who became notable mathematicians",
    "Contributed to mathematical education in South India",
    "Participated in Ramanujan centenary celebrations"
  ],
  impact: "Built a strong school of mathematical analysis at Annamalai University. His textbooks are used across India. Mentored many students who contributed to Indian mathematics.",
  awards: ["Fellow of Indian Academy of Sciences", "Awards from mathematical societies"]
}
```

---

## Technical Features

### 1. Sidebar Functionality
```javascript
function toggleCategory(header) {
  // Toggle the 'active' class on the header
  // Toggle the 'expanded' class on the person-list
  // Animate the chevron icon rotation
  // Show/hide the list of people under that category
}
```

### 2. Profile Display
```javascript
function showProfile(category, index) {
  // Hide welcome screen
  // Show profile card
  // Populate profile card with data from profiles object
  // Update active state in sidebar
  // Scroll to top of content area
}
```

### 3. Save as Image (using html2canvas)
```javascript
async function saveAsImage() {
  // Hide action buttons temporarily
  // Use html2canvas to capture the profile card
  // Download as PNG with filename: ATATA_[Name]_Profile.png
  // Show action buttons again
}
```

### 4. Save as PDF (using jsPDF)
```javascript
async function saveAsPDF() {
  // Hide action buttons temporarily
  // Use html2canvas to capture the profile card
  // Convert to PDF using jsPDF
  // Handle multi-page if content exceeds A4
  // Download as PDF with filename: ATATA_[Name]_Profile.pdf
  // Show action buttons again
}
```

### 5. Share on WhatsApp
```javascript
function shareOnWhatsApp() {
  // Generate formatted text with profile details
  // Include name, serial, dates, birthplace, achievements, awards
  // Add ATATA branding and Tamil tagline
  // Open WhatsApp with encoded text
}
```

### 6. Visitor Counter
```javascript
function updateVisitorCount() {
  // For demo: Use localStorage with random base count
  // For production: Use CountAPI or similar service
  // Display formatted count
}
```

---

## External Libraries Required
```html
<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Source+Sans+Pro:wght@300;400;500;600&family=Noto+Sans+Tamil:wght@400;500;600&display=swap" rel="stylesheet">

<!-- Font Awesome Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<!-- html2canvas for image export -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>

<!-- jsPDF for PDF export -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
```

---

## Responsive Design Requirements

### Desktop (>1024px)
- Full two-panel layout
- Sidebar: 320px fixed width
- Content: Flexible width

### Tablet (768px - 1024px)
- Stack layout vertically
- Sidebar becomes full width, collapsible
- Profile card adjusts

### Mobile (<768px)
- Full stacking
- Simplified header
- Single-column info cards
- Vertically stacked action buttons
- Touch-friendly interactions

---

## CSS Animations

### fadeIn Animation
```css
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
```

### Hover Effects
- Cards lift slightly (translateY(-3px))
- Shadows intensify
- Colors shift subtly
- Smooth 0.3s transitions

### Category Expansion
- Smooth max-height transition
- Chevron rotation animation

---

## Custom Scrollbar Styling
```css
::-webkit-scrollbar { width: 8px; }
::-webkit-scrollbar-track { background: var(--cream); }
::-webkit-scrollbar-thumb {
  background: linear-gradient(180deg, var(--primary-gold), var(--accent-copper));
  border-radius: 4px;
}
```

---

## Print Styles
```css
@media print {
  .sidebar, .action-buttons, header, footer { display: none !important; }
  .content { padding: 0; }
  .profile-card { box-shadow: none; border: 2px solid var(--primary-maroon); }
}
```

---

## File Structure (Recommended)
```
atata/
├── index.html
├── css/
│   └── styles.css
├── js/
│   ├── profiles.js (profile data)
│   └── main.js (functionality)
├── images/
│   └── [profile images]
└── README.md
```

---

## Additional Notes

1. **Profile Images**: Currently using placeholder icons. Add actual images as base64 or URLs.

2. **Data Expansion**: The structure supports adding more categories (Arts, Music, Literature, Medicine, etc.) and more profiles.

3. **Search Feature**: Consider adding a search bar to filter profiles.

4. **Admin Panel**: Future enhancement - add ability to add/edit profiles.

5. **Backend**: For production, consider adding a backend for:
   - Visitor tracking
   - Profile management
   - Image uploads
   - User contributions

6. **SEO**: Add meta tags, structured data, and social sharing tags.

7. **Accessibility**: Ensure ARIA labels, keyboard navigation, and screen reader support.

---

## Credits in Footer

The footer should include:
- © 2026 ATATA - Arun Thondu Attriya Thamizhaga Andhanarkal
- Developed by **Suraja Technologies**
- Powered by **Jignyashika Consulting**
- Under the guidance of **Dr. Sundararaman Chintamani**
- Image attribution disclaimer

---

**End of Prompt**

Create this website as a single HTML file with embedded CSS and JavaScript for easy deployment and testing.
