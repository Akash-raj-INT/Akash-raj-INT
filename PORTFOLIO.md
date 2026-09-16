````markdown
---

# **AKASH RAJ**
**Full-Stack Web Developer | Frontend Specialist | AI/ML Enthusiast**

📧 Email: akashraj848114@gmail.com | 🔗 GitHub: [Akash-raj-INT](https://github.com/Akash-raj-INT)  
🌍 Portfolio: [https://akashrajportfolio.netlify.app/](https://akashrajportfolio.netlify.app/)  
📍 Location: New Delhi | 🔗 LinkedIn: [Connect](#)

---

## **PROFESSIONAL SUMMARY**

Full-stack developer with 2+ years of experience building scalable, feature-rich web applications. Specialized in vanilla JavaScript architecture, responsive design, AI-powered UX, and backend services with Django/Python. Passionate about creating production-grade prototypes that solve real business problems. Strong foundation in component-driven development, state management patterns, and clean architecture principles.

---

## **KEY COMPETENCIES**

| **Frontend** | **Backend** | **Architecture** | **Tools & Tech** |
|---|---|---|---|
| Vanilla JavaScript (ES6+) | Django & Python | Repository Pattern | Vercel & Git |
| React & Angular | REST APIs | Client-side State Mgmt | localStorage APIs |
| HTML5 & CSS3 | Node.js/Express | Data Normalization | Web Speech API |
| Component Architecture | SQL & SQLite | Hash-based Routing | Machine Learning |
| DOM Manipulation | Database Design | Mock Layers | PyTorch & TensorFlow |
| Responsive Design | Web Scraping | API Abstraction | Web Audio/Voice |

---

---

# **🌟 FEATURED PROJECTS**

---

## **1. HANDLOOM — B2B Textile Marketplace**

### **High-Performance Marketplace Prototype** ⭐⭐⭐
*A fully-functional, feature-rich B2B marketplace built for a hackathon brief*

**Project Duration:** 6 weeks | **Status:** Production-ready prototype  
**Live Demo:** [https://handloom-theta.vercel.app](https://handloom-theta.vercel.app)  
**Repository:** [GitHub](https://github.com/Akash-raj-INT/Handloom)

---

### **Technical Overview**

**Architecture & Stack:**
- **Frontend:** Vanilla JavaScript (ES6+), HTML5, CSS3 (zero frameworks)
- **State Management:** localStorage-backed mock database with repository pattern
- **Routing:** Hash-based client-side router
- **AI Component:** Rule-based NLU engine for product discovery
- **Deployment:** Vercel (serverless)

**Why This Approach:**
This intentional framework-free design demonstrates:
- Zero external dependencies running entirely in-browser
- localStorage as simulated database for complete isolation
- Clean repository pattern for seamless API migration
- Full-stack thinking without complexity
- 2,500 lines of production-grade JavaScript

---

### **Core Features Delivered**

#### **🔐 Role-Based Authentication System**
- Dual-role support (Buyer & Supplier) with session persistence
- Secure login/register with form validation
- Conversational & traditional onboarding flows (user choice)
- Demo accounts: `buyer@demo.com` / `supplier@demo.com` (both: `demo1234`)

#### **🤖 AI-Powered Marketplace Assistant ("Weave")**
*Standout feature demonstrating advanced UX patterns*

**Capabilities:**
- 🔍 **Natural Language Search** → Keyword extraction + attribute scoring
- 💡 **Smart Recommendations** → Rule-based NLU with price/category/fabric filtering
- 🔄 **Product Comparison** → Side-by-side spec tables
- ❓ **Contextual Q&A** → Answer product questions (MOQ, stock, composition)
- 🎙️ **Voice Input** → Web Speech API integration
- 💬 **Conversational Chat** → Interactive flow with quick-reply suggestions

**Implementation:**
```javascript
// Transparent NLU ready for LLM swap
function scoreProduct(product, intent) {
  let score = 0;
  
  // Category matching
  intent.categories.forEach(c => {
    if (product.haystack.includes(c)) score += 4;
  });
  
  // Price ceiling filtering
  if (intent.priceCeiling && product.price <= intent.priceCeiling) 
    score += 3;
  
  // Budget language detection
  if (intent.wantsCheap) 
    score += Math.max(0, 3 - product.price / 5);
  
  return score;
}
```

#### **🛍️ Complete Buyer Experience**
- Marketplace browsing with advanced filters (category, fabric, price, stock)
- Product detail pages with gallery & color swatches
- Shopping cart with persistent state
- Multi-step checkout (shipping → review → confirmation)
- Buyer dashboard with order history

#### **📊 Full Supplier Portal**
- Dashboard with product stats & low-stock alerts
- Inventory management (add/edit/delete products)
- Order management with status progression
- Business profile management
- Conversational onboarding option

---

### **Project Statistics**

| Metric | Value |
|---|---|
| **Total LoC** | ~2,500 |
| **JavaScript** | 80.4% |
| **CSS** | 18.3% |
| **HTML** | 1.3% |
| **Core Modules** | 8 (auth, store, router, AI, components, pages) |
| **Features** | 15+ major features |
| **Demo Accounts** | 2 pre-seeded |

---

---

## **2. EXTROVERTS SIGNUP WIZARD — High-Fidelity App Replication**

### **Advanced Onboarding UI/UX** 🎉⭐⭐
*Progressive 4-step signup wizard replicating an Android party app*

**Live Demo:** [https://extroverts-signup-wizard.vercel.app/](https://extroverts-signup-wizard.vercel.app/)  
**Repository:** [GitHub](https://github.com/Akash-raj-INT/Extroverts-Signup-Wizard)  
**Tech Stack:** React 19 + Vite + Vanilla CSS

---

### **Key Features & UX Innovations**

#### **🎨 Landing Page & Terms Modal**
- Dark party vibe theme (`#090A0F`) with neon glowing accents
- Glassmorphic cards showcasing party categories
- Live stats ticker (participants, hosts, ratings)
- Community terms modal with safety policies & 18+ restriction

#### **🧙‍♂️ Progressive 4-Step Signup Wizard**

**Step 1: Contact & Enhanced OTP Verification**
- Email or Mobile Phone toggle with country code selector
- Real-time validation for emails/phones
- 6 individual digit input boxes with:
  - Auto-focus & backspace navigation
  - Paste support
  - 30-second countdown timer
  - ⚡ Demo fill button (`123456`)

**Step 2: Profile Essentials & Age Restriction UX**
- Full Name input (2–50 chars, trim validation)
- DOB date selector with **Real-Time Age Calculation**
- **Under 18 Alert Banner** → Glowing red warning with "Extroverts is 18+ only"
- Gender identity & Pronouns selection pills

**Step 3: Campus & Location (Cross-Field Filtering)**
- **Dynamic Cascading:** State → Cities → Colleges
- State selector (California, New York, Texas, Maharashtra, Delhi NCR, Karnataka)
- City filter based on selected state
- College/University population based on city
- **Smart Logic:** Prevents invalid combinations

**Step 4: Party Vibes, Photo & Bio**
- Party Vibe interest tags (minimum 3 required)
- Photo file uploader with preview
- 6 preset party avatar gallery
- Bio textarea with live counter (`0/150`)
- Quick prompt insertion pills

#### **🎉 VIP Extrovert Party Pass & Confetti**
- Canvas confetti celebratory blast
- Interactive VIP ticket with:
  - User photo & name
  - Age, city/state, campus
  - Selected vibes
  - Serial barcode (`EX-2026-XXXXXX`)

#### **📱 Device View Simulator**
- Toggle between Desktop & Mobile phone frame
- Easy responsive testing

---

### **Technical Highlights**

```javascript
// Smart age calculation & real-time validation
const calculateAge = (dob) => {
  const today = new Date();
  let age = today.getFullYear() - dob.getFullYear();
  const monthDiff = today.getMonth() - dob.getMonth();
  
  if (monthDiff < 0 || (monthDiff === 0 && today.getDate() < dob.getDate())) {
    age--;
  }
  
  return age;
};

// Under-18 restriction with visual feedback
if (age < 18) {
  showRestrictedBanner(); // Glowing red banner
  disableNextButton();    // Prevent progression
} else {
  hideRestrictedBanner();
  enableNextButton();
}
```

**Cross-Field Filtering Logic:**
```javascript
// Dynamic city population based on state
const citiesByState = {
  'California': ['Los Angeles', 'San Francisco', 'San Diego'],
  'Maharashtra': ['Mumbai', 'Pune', 'Nagpur'],
  // ...
};

// College population based on city
const collegesByCity = {
  'Los Angeles': ['UCLA', 'USC', 'LMU'],
  'Mumbai': ['IIT Bombay', 'NMIMS', 'Amity'],
  // ...
};
```

---

### **Tech Stack**
- React 19 + Vite
- Vanilla CSS (Glassmorphism, Neon effects, Micro-animations)
- Lucide React icons
- Canvas Confetti
- Vercel deployment

---

---

## **3. SOLAR COMPANY — Full-Stack Web Application**

### **Enterprise-Grade Django Web App** ⚡⭐⭐
*High-performance solar energy company website with interactive features*

**Live Demo:** [https://solar-company-smoky.vercel.app/](https://solar-company-smoky.vercel.app/)  
**Repository:** [GitHub](https://github.com/Akash-raj-INT/Solar-Company)

---

### **Technology Stack**

| Layer | Technology |
|---|---|
| **Backend** | Python 3.12, Django 4.2 |
| **Frontend** | HTML5 Semantic, Vanilla CSS, ES6 JavaScript |
| **Database** | SQLite3 + Django ORM |
| **Deployment** | Vercel Serverless Functions |
| **Fonts & Icons** | Google Fonts (Outfit, Plus Jakarta Sans), Custom SVG |

---

### **Key Features & Sections**

#### **⚡ Sticky Glassmorphic Navigation Bar**
- Responsive nav with brand logo
- Section scrolling links
- Mobile drawer menu
- Quick CTA button

#### **🌅 Dynamic Hero Section**
- High-impact headline
- Live generation metric card
- Solar panel illustration
- Achievement badges:
  - 15,000+ Installations
  - 25-Year Performance Warranty
  - $24M+ Customer Savings

#### **🛠️ Solar Services Grid**
Four interactive service modules:
1. **Photovoltaic Installation** — Panel placement & grid connection
2. **Panel Maintenance & Cleaning** — Performance optimization
3. **3D LiDAR Energy Audit** — Site analysis
4. **Smart Battery Backup Storage** — Energy storage solutions

Each with technical spec modals and detailed information.

#### **🧮 Interactive Solar ROI Calculator**
Real-time sliders calculating:
- 25-year financial savings
- Reduced monthly bill
- Investment payback timeline
- Annual CO₂ reduction (tons)

**Implementation:**
```javascript
// Real-time ROI calculation
function calculateROI(systemSize, location, panelCount) {
  const annualGeneration = systemSize * 1.3 * locationFactors[location];
  const savings25Year = annualGeneration * 25 * electricityRate * escalation;
  const paybackYears = systemCost / (savings25Year / 25);
  const co2Reduction = annualGeneration * 0.4; // tons/year
  
  return {
    savings25Year,
    paybackYears,
    co2Reduction,
    monthlyBillReduction: (annualGeneration / 12) * electricityRate
  };
}
```

#### **🏆 Why Choose Us & Utility Comparison**
- Key differentiators
- Interactive comparison table (Solaria vs. Standard Grid)
- Feature matrix highlighting advantages

#### **📜 About Us, Testimonials & FAQs**
- Mission & company background
- 5-star verified customer reviews
- Interactive accordion FAQs with smooth expand/collapse

#### **📩 Asynchronous Quote Request Form**
- Real-time form validation
- AJAX JSON submit processing
- Inline success/error alerts
- Toast notifications
- Submissions stored in SQLite

#### **⚙️ Django Admin Panel**
- Full `/admin/` portal
- Manage services, inquiries, testimonials
- Edit testimonials & contact submissions

---

### **Project Structure**

```
Solar-Company/
├── manage.py
├── requirements.txt
├── vercel.json               # Serverless config
├── api/
│   └── index.py              # Serverless entry
├── solar_project/
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── core/
│   ├── models.py             # SolarService, Testimonial, FAQ, ContactSubmission
│   ├── views.py              # Home render + AJAX handlers
│   ├── admin.py              # Admin registrations
│   └── management/commands/
│       └── seed_data.py      # Auto-populate database
├── templates/
│   ├── base.html
│   ├── index.html
│   └── includes/             # navbar, hero, services, calculator, etc.
└── static/
    ├── css/style.css         # Complete design system
    └── js/main.js            # Calculator, modals, AJAX
```

---

### **Key Technical Achievements**

✅ **Serverless Django Deployment** on Vercel with `@vercel/python`  
✅ **Real-time ROI Calculator** with dynamic financial projections  
✅ **Responsive Design** from mobile to desktop  
✅ **AJAX Form Submission** with client-side validation  
✅ **SQLite + Django ORM** for persistence  
✅ **Admin Panel** for content management  
✅ **Zero Frontend Build Step** — pure HTML/CSS/JS  

---

---

## **4. PAGE PULSE — SEO & Accessibility Audit Tool**

### **Python/Django Backend Tool** 🔍⭐
*Lightweight URL analyzer for SEO vitals & accessibility checks*

**Live Demo:** [https://page-pulse-rz01.onrender.com](https://page-pulse-rz01.onrender.com)  
**Repository:** [GitHub](https://github.com/Akash-raj-INT/Page-Pulse)

---

### **What It Does**

Audits any public URL and returns a comprehensive report:
- ✅ HTTP status & response time
- ✅ Page title & meta description
- ✅ H1 count validation
- ✅ Images missing alt text (accessibility)
- ✅ Approximate word count
- ✅ Content type detection
- ✅ Truncation warnings for large responses

---

### **Technical Architecture**

**Backend:**
- Django 4.2 + Python 3
- Stateless request design (no database persistence)
- Comprehensive error handling & recovery
- Security: blocks localhost/internal hosts

**Frontend:**
- Single-page HTML/CSS/JS interface
- No build step
- Real-time validation feedback
- Toast notifications

**API Endpoint:**

```bash
POST /api/audit/
Content-Type: application/json

Request:
{ "url": "example.com" }

Response (200 OK):
{
  "requested_url": "https://example.com",
  "final_url": "https://example.com/",
  "status_code": 200,
  "response_time_ms": 184,
  "content_type": "text/html; charset=UTF-8",
  "title": "Example Domain",
  "meta_description": null,
  "h1_count": 1,
  "images_total": 0,
  "images_missing_alt": 0,
  "word_count": 28,
  "truncated": false
}
```

---

### **Design Choices**

| Feature | Implementation |
|---|---|
| **No Database** | Stateless; only SQLite for Django defaults |
| **Response Size Cap** | 5 MB limit prevents worker overload |
| **Timeouts** | 5s connect / 12s read prevents hanging |
| **Security** | Blocks localhost/internal IPs |
| **Word Count** | Regex-based (approximate) over visible text |
| **Error Handling** | Every failure mode → structured JSON |

---

### **Deployment Options**

**Recommended: Render.com**
```bash
Build command: ./build.sh
Start command: gunicorn pagepulse.wsgi
Environment vars: SECRET_KEY, DEBUG=False, ALLOWED_HOSTS
```

**Also works on:**
- Railway
- Heroku
- PythonAnywhere

---

### **Code Quality**

**Clean Service Layer:**
```python
# services.py - reusable, testable
def audit_url(raw_url) -> dict:
    """
    Fetch URL, parse, extract vitals.
    Raises ValidationError or AuditError.
    """
    validated_url = validate_url(raw_url)
    response = fetch_with_timeout(validated_url)
    return parse_response(response)
```

This design allows:
- ✅ Unit testing without Django
- ✅ Reuse in management commands
- ✅ Celery task integration
- ✅ CLI usage

---

---

## **5. E-COMMERCE STORE — Angular Application**

### **Full-Featured Shopping Platform** 🛒⭐
*Modern e-commerce application with routing, search, and cart*

**Live Demo:** [https://e-commerce-store-6b1o.onrender.com](https://e-commerce-store-6b1o.onrender.com)  
**Repository:** [GitHub](https://github.com/Akash-raj-INT/E-Commerce-Store)

---

### **Technology Stack**

- **Framework:** Angular + TypeScript
- **Styling:** Responsive CSS
- **Data:** JSON-based product catalog
- **Deployment:** Render.com

---

### **Core Features**

#### **📦 Product Management**
- Product listing with grid view
- Detailed product pages
- Responsive image galleries
- Stock indicators

#### **🔍 Search & Filtering**
- Real-time search functionality
- Category filtering
- Price range filters
- Sort options (name, price, rating)

#### **🛒 Shopping Cart**
- Add/remove items
- Quantity management
- Persistent cart (localStorage)
- Cart summary with totals

#### **🔀 Client-Side Routing**
- Angular Router for seamless navigation
- Lazy-loaded product modules
- Deep linking support

#### **📱 Responsive Design**
- Mobile-first approach
- Tablet & desktop optimization
- Touch-friendly interface

---

### **Project Structure**

```
E-Commerce-Store/
├── src/
│   ├── app/
│   │   ├── components/
│   │   │   ├── product-list/
│   │   │   ├── product-detail/
│   │   │   └── cart/
│   │   ├── services/
│   │   │   └── product.service.ts
│   │   └── app.routing.ts
│   ├── assets/
│   │   └── products.json
│   └── styles.css
└── angular.json
```

---

---

## **TECHNICAL SKILLS DEMONSTRATED**

### **Vanilla JavaScript**
✅ ES6+ modules, async/await, Promises  
✅ DOM manipulation & event handling  
✅ Array methods (map, filter, reduce)  
✅ localStorage & sessionStorage APIs  
✅ Regular expressions  
✅ Web Audio/Speech APIs  

### **Frontend Frameworks**
✅ React 19 + Vite  
✅ Angular with TypeScript  
✅ Component-driven architecture  
✅ State management patterns  

### **Backend & Full-Stack**
✅ Django 4.2 + Python 3  
✅ Node.js/Express basics  
✅ RESTful API design  
✅ Database modeling (SQLite, basic SQL)  
✅ Serverless deployment  

### **CSS & Design**
✅ Responsive design (mobile-first)  
✅ CSS Grid & Flexbox  
✅ Glassmorphism & modern effects  
✅ Design systems & tokens  
✅ Accessibility (WCAG 2.1)  
✅ Animation & transitions  

### **DevOps & Deployment**
✅ Vercel serverless  
✅ Render.com cloud platform  
✅ Git & GitHub  
✅ Build tools (Vite, npm)  
✅ Environment configuration  

### **Advanced Features**
✅ Web Speech API (voice input)  
✅ Real-time data validation  
✅ AJAX form submission  
✅ Progressive enhancement  
✅ Offline-first patterns (localStorage)  

---

---

## **KEY ACHIEVEMENTS**

✅ **Built 5+ production-grade prototypes** demonstrating full-stack expertise  
✅ **Zero-dependency architecture** (Handloom) proving vanilla JavaScript mastery  
✅ **AI-powered UX** with rule-based NLU for intelligent recommendations  
✅ **Responsive design** working seamlessly across mobile/tablet/desktop  
✅ **Accessible interfaces** following WCAG 2.1 guidelines  
✅ **Clean architecture** with separation of concerns & easy backend migration  
✅ **Serverless deployment** on Vercel, Render, and PythonAnywhere  
✅ **Real-world features**: authentication, payments flow, admin panels, analytics  

---

---

## **PROFESSIONAL EXPERIENCE & ACHIEVEMENTS**

### **Skills Summary**

**Languages:** JavaScript (Expert), Python (Advanced), TypeScript (Intermediate), SQL (Intermediate)  
**Frontend:** React, Angular, Vanilla JS, HTML5, CSS3, Responsive Design  
**Backend:** Django, Node.js/Express, REST APIs, Database Design  
**DevOps:** Vercel, Render, Git, CI/CD basics  
**Tools:** VS Code, Git, npm/pip, Figma (design collaboration)  
**Soft Skills:** Problem-solving, rapid prototyping, user-centric design, documentation  

---

---

## **LEARNING & GROWTH**

🎓 **Currently exploring:**
- Advanced React patterns & Next.js  
- FastAPI for high-performance Python backends  
- Machine learning with TensorFlow/PyTorch  
- System design & scalability  
- Web3 & blockchain basics  

📚 **Strong foundation in:**
- Data Structures & Algorithms (DSA)  
- Object-Oriented & Functional Programming  
- Web standards & best practices  
- Performance optimization  

---

---

## **GITHUB STATS**

- 60+ repositories showcasing diverse projects
- Full-stack examples (frontend, backend, ML)
- Active contributor & open-source enthusiast
- Consistent commit history demonstrating dedication

---

---

## **HOW I WORK**

### **My Development Philosophy**

1. **User-First Design** → Features solve real problems
2. **Clean Code** → Readable, maintainable, testable
3. **Progressive Enhancement** → Start simple, add complexity when needed
4. **Documentation** → Every project has clear READMEs & comments
5. **Performance** → Optimize for speed & accessibility
6. **Collaboration** → Clear commits, comments, and communication

### **Project Approach**

- 📋 Requirement analysis & planning
- 🎨 Responsive design mockups
- 💻 Modular, testable code
- 🧪 Manual testing + edge cases
- 📦 Deployment & monitoring
- 📝 Documentation & handoff

---

---

## **WHAT'S NEXT**

🚀 **Building:** Advanced full-stack applications with real-time features  
🤖 **Exploring:** AI-powered features & intelligent recommendations  
💼 **Seeking:** Opportunities to impact user experience at scale  
🌍 **Goal:** Contribute to open-source & mentor junior developers  

---

---

## **GET IN TOUCH**

💌 **Email:** [akashraj848114@gmail.com](mailto:akashraj848114@gmail.com)  
🔗 **GitHub:** [github.com/Akash-raj-INT](https://github.com/Akash-raj-INT)  
🌐 **Portfolio:** [akashrajportfolio.netlify.app](https://akashrajportfolio.netlify.app)  
💼 **LinkedIn:** [Connect on LinkedIn](#)  

---

## **PROJECT LINKS**

| Project | Type | Live Demo | Repo |
|---------|------|-----------|------|
| **Handloom** | B2B Marketplace | [Live](https://handloom-theta.vercel.app) | [GitHub](https://github.com/Akash-raj-INT/Handloom) |
| **Extroverts** | Signup Wizard | [Live](https://extroverts-signup-wizard.vercel.app/) | [GitHub](https://github.com/Akash-raj-INT/Extroverts-Signup-Wizard) |
| **Solar Company** | Django App | [Live](https://solar-company-smoky.vercel.app/) | [GitHub](https://github.com/Akash-raj-INT/Solar-Company) |
| **Page Pulse** | SEO Audit Tool | [Live](https://page-pulse-rz01.onrender.com) | [GitHub](https://github.com/Akash-raj-INT/Page-Pulse) |
| **E-Commerce** | Angular Store | [Live](https://e-commerce-store-6b1o.onrender.com) | [GitHub](https://github.com/Akash-raj-INT/E-Commerce-Store) |

---

*Document created: September 2026*  
*Last updated: September 16, 2026*  
*For inquiries or collaboration, please reach out via email or GitHub.*

````
