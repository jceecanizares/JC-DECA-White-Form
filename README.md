# Deca Homes Urdaneta — Principal Beneficiary White Form Assistant

An interactive, mobile-first web assistant for homebuyers of **Deca Homes Urdaneta (Expanded 4PH Program)** to easily fill out their **Principal Beneficiary Details (White Form / Information Slip)** with digital signature capture, instant validation, and high-resolution document generation.

Exclusively branded and locked to **Sales Consultant John Edcee T. Cañizares** and **Agency Manager Rowena Comilang** (Cassia DECA / North Forbes Realty / Deca Gold).

---

## 🌟 Key Features

1. **Step-by-Step Guided Form:**
   - **Step 1:** Principal Beneficiary Details (Personal info, Pag-IBIG MID formatting, birthday & age checks).
   - **Step 2:** Employment & Income Details (Employer, designation, category, monthly income).
   - **Step 3 (Smart Conditional):** Spouse Details — **Automatically skippable** if the applicant is Single, Widowed, or Legally Separated; required only if Married.
   - **Step 4:** Touch/Mouse **Digital Signature Pad** with ink simulation.

2. **100% Authentic White Form Replication:**
   - Hardcoded background matching `assets/verified/White Form.jfif` at **1792 x 2400** high-definition resolution.
   - Exact coordinate alignment on all underlines, checkmarks, and signature lines.
   - Authentic ballpen navy blue ink typography.

3. **Agency & Consultant Lock (Exclusive):**
   - The generated form permanently includes:
     * **Group Name:** `Cassia DECA/North Forbes Realty`
     * **Seller / Realty Name:** `JOHN EDCEE T. CAÑIZARES (SC) / ROWENA COMILANG (AM) / NORTH FORBES REALTY`
     * Direct Messenger routing to `https://m.me/DecaHomeUrda`.

4. **Multi-Export Options & Official Vector PDFs:**
   - **Download High-Res JPG:** Saves directly to the buyer's phone or computer.
   - **Print / Save as PDF:** One-click print preview scaled for standard Letter/A4 portrait.
   - **Copy Summary for Messenger:** Formats an executive summary ready to paste directly into JC's Facebook Messenger.
   - **Official Fillable PDF (`Deca_Gold_Principal_Beneficiary_Form_Fillable.pdf`):** Interactive digital PDF with 32 AcroForm fields (can be typed directly in Acrobat/Chrome/Brave) with locked attribution.
   - **Pre-printed Official PDF (`Deca_Gold_Principal_Beneficiary_Form_JC_Canizares.pdf`):** Vector-grade official PDF with pre-stamped group and seller attribution ready for instant hardcopy printing.

5. **Anti-Phishing & Trust Verification Shield:**
   - **Official Deca Homes Logo:** Displays authentic `logo-deca-homes-square.jpg` directly in the header and trust cards.
   - **Zero-Storage Privacy Architecture:** Runs 100% inside the buyer's browser. Zero database, zero passwords, zero payment collection online (RA 10173 Compliant).
   - **Interactive Security Modal ("Ligtas Ba Ito?"):** Explains consultant credentials, office location (San Vicente East), site location (Brgy. Nancayasan), and provides one-tap Messenger verification (`m.me/DecaHomeUrda`).
   - **Integrated Field Guides:** Contextual tooltips explaining where to find the 12-digit Pag-IBIG MID, civil status rules, and OFW income ceiling exemption.

---

## 🔒 Zero-Leakage Architecture & Complete Separation from Buyer Database

> [!IMPORTANT]
> **Strict Separation of Concerns:**
> - **White Form Assistant (`white-form-assistant`):** This is a 100% standalone, public-facing tool meant for prospective homebuyers. It runs entirely client-side inside the buyer's own mobile browser. It has **NO database connection**, **NO links to internal CRM records**, and **NO storage of other clients' data**.
> - **Buyer Database CRM (`buyer-database`):** This is John Edcee Cañizares's **private, internal-only CRM vault**. It resides exclusively on his local machine (and private Google Sheet sync) and must **NEVER** be uploaded to GitHub or shared publicly.
> - The two tools are kept strictly isolated to guarantee 100% client data privacy and prevent any exposure of confidential buyer leads.

---

## 🚀 How to Run Locally

You can test and run this tool right now on your computer:
1. Navigate to: `C:\Users\jceec\workspaces\decahome-urdaneta\tools\white-form-assistant\`
2. Double-click `index.html` (it will open directly in Brave or Chrome).
3. Try filling out the form, drawing a signature, and clicking **"Generate Official White Form"**!

---

## 🌐 How to Publish to GitHub Pages (Live Online Link for Buyers)

To give buyers a public link they can open from Facebook Messenger, follow these 3 quick steps:

### Option A: Create a Dedicated Free Repository on GitHub (Recommended)
1. Go to [github.com/new](https://github.com/new) and log in.
2. Set **Repository name** to: `white-form` (or `deca-whiteform`).
3. Set visibility to **Public** and click **Create repository**.
4. Click **"uploading an existing file"** and drag all 3 files from this folder:
   - `index.html`
   - `template-b64.js`
   - `white-form-template.jpg`
5. Click **Commit changes**.
6. Go to repository **Settings** ➔ **Pages** (on the left menu).
7. Under **Branch**, select `main` (or `master`) and click **Save**.
8. In ~1 minute, your live link will be ready:
   `https://<your-github-username>.github.io/white-form/`

Now, whenever a buyer asks for the White Form or pre-screening, simply send them your link!

---

## 📁 File Structure

```text
tools/white-form-assistant/
├── index.html              # Complete client-side web application (UI, logic, canvas renderer)
├── template-b64.js         # Base64 encoded high-res template (zero CORS/offline capability)
├── white-form-template.jpg # 1792x2400 JPG backup asset
└── README.md               # User guide & deployment instructions
```
