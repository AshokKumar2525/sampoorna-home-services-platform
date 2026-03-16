# 🏠 Sampoorna Home Services

> **One platform. Verified vendors. Fixed pricing.**  
> A one-stop digital platform that coordinates moving, repairs, cleaning, and maintenance — making urban relocation stress-free.

Built as part of the **Venture Viability Analysis** at IIIT RGUKT RK Valley, Kadapa, Andhra Pradesh.  
Supported by **Wadhwani Foundation**.

---

## 📸 Preview

| Section | Description |
|---|---|
| Hero | UVP, trust badges, real photo background |
| Stats | Animated counters — relocations, satisfaction, vendors |
| Services | 4 service cards with real images |
| How It Works | Visual infographic with 4-step flow |
| Demo | Embedded YouTube demo video |
| Pricing | 3-tier pricing cards |
| Testimonials | Customer reviews with avatars |
| Contact | Booking form + Contact form + Newsletter |

---

## 🗂️ Project Structure

```
sampoorna-home-services/
├── sampoorna-v2.html        # React frontend (single file, no build needed)
├── sampoorna-backend.py     # FastAPI backend
├── requirements.txt         # Python dependencies
└── README.md                # You are here
```

---

## ⚙️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 18 (CDN, no build step), CSS Variables |
| Backend | FastAPI (Python) |
| Fonts | Cormorant Garamond + Outfit (Google Fonts) |
| Images | Unsplash (free, no API key needed) |
| Video | YouTube embed |
| Notifications | SMTP Email (Gmail) + Twilio (WhatsApp/SMS) |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/sampoorna-home-services.git
cd sampoorna-home-services
```

### 2. Set Up Python Environment

```bash
# Create virtual environment
python -m venv venv

# Activate it
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### 3. Run the Backend

```bash
uvicorn sampoorna-backend:app --reload --port 8000
```

Backend will be live at: `http://localhost:8000`  
API docs (auto-generated): `http://localhost:8000/docs`

### 4. Open the Frontend

Just open `sampoorna-v2.html` in your browser — no build step needed.

> ⚠️ Make sure the backend is running on port 8000 before opening the frontend, otherwise the forms won't submit.

---

## 📡 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/booking` | Submit a booking enquiry |
| `POST` | `/api/contact` | Submit a contact message |
| `POST` | `/api/newsletter` | Subscribe to newsletter |
| `GET` | `/admin/bookings` | View all bookings |
| `GET` | `/admin/contacts` | View all contact submissions |
| `GET` | `/admin/subscribers` | View all newsletter subscribers |

### Example Booking Request

```json
POST /api/booking
{
  "name": "Priya Sharma",
  "email": "priya@email.com",
  "phone": "+91 98765 43210",
  "service_type": "full-relocation",
  "preferred_date": "2025-08-15",
  "city": "Hyderabad",
  "notes": "3 BHK, 2nd floor, no lift"
}
```

---

## 🔔 Setting Up Notifications (Optional)

To enable real email/WhatsApp alerts, configure these in `sampoorna-backend.py`:

### Gmail SMTP (Email)
1. Go to your Google Account → **Security** → **2-Step Verification** → **App Passwords**
2. Generate a password for "Mail"
3. Fill in the config at the top of `sampoorna-backend.py`:

```python
GMAIL_USER     = "yourname@gmail.com"
GMAIL_PASSWORD = "your-app-password"
TEAM_EMAIL     = "team@sampoorna.in"
```

### Twilio (WhatsApp / SMS)
1. Sign up at https://twilio.com (free trial available)
2. Get your Account SID, Auth Token, and WhatsApp number
3. Fill in:

```python
TWILIO_ACCOUNT_SID  = "ACxxxxxxxxxxxxxxxx"
TWILIO_AUTH_TOKEN   = "your_auth_token"
TWILIO_WHATSAPP_FROM = "whatsapp:+14155238886"
```

---

## 🎬 Replacing the Demo Video

In `sampoorna-v2.html`, find this line and replace the video ID:

```js
const VIDEO_ID = "dQw4w9WgXcQ"; // ← Replace with your YouTube video ID
```

Your YouTube video URL looks like:  
`https://www.youtube.com/watch?v=`**`ABC123xyz`**  
The bold part is your Video ID.

---

## 👥 Venture Team

| Name | Role | Skills |
|---|---|---|
| P. Mounisha | Marketing | Digital Marketing |
| C. Sowmya | Customer Outreach | Presenting & Communication |
| M. Ashok Kumar | Product Development | UI Design, Problem Solving |

**Mentor:** Kalyan Chakravarthy  
**Mentors Needed:** Product, GTM strategy, vendor onboarding, pricing, scaling

---

## 📊 Financial Snapshot

| Year | Revenue | Expenses | Profit |
|---|---|---|---|
| Year 1 | ₹46,00,000 | ₹40,50,000 | ₹5,50,000 |
| Year 2 | ₹60,00,000 | ₹45,00,000 | ₹15,00,000 |
| Year 3 | ₹1,20,00,000 | ₹80,00,000 | ₹40,00,000 |

- **Break-even:** Month 7
- **Pricing:** ₹5,000 per relocation booking
- **Model:** Marketplace + Pay-per-Use

---

## 🗺️ Roadmap

| Timeline | Goal |
|---|---|
| Months 1–3 | MVP build & user validation |
| Months 4–6 | Beta launch & vendor onboarding |
| Months 7–9 | Expand users & partnerships |
| Months 10–12 | Scale ops & funding readiness |

---

## 📄 License

This project is for educational and entrepreneurship purposes under the **Wadhwani Foundation NEN Program**.

---

<p align="center">Made with ♦ for India's urban movers · Sampoorna Home Services © 2025</p>
