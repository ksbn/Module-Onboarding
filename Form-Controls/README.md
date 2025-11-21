# 🧾 Form Controls — T-Shirt Order Form

## 🎯 Learning Objectives

- [x] Interpret requirements and check against a list of criteria  
- [x] Write a valid form using semantic HTML only  
- [x] Test and validate using DevTools  
- [x] Refactor to achieve 100% Accessibility score (Lighthouse)

---

## 🧩 Task Description

We are selling **T-shirts**.  
Your task is to create a form that collects the following information **without using CSS or JavaScript**:

1. **Customer name** — must be valid and contain at least 2 characters.  
2. **Customer email** — must be a valid email address.  
3. **T-shirt colour** — must be selected from **3 predefined options**.  
4. **T-shirt size** — must be selected from **6 predefined options (XS–XXL)**.

All fields are **required**.  
The form **must not** include an `action` attribute.

---

## 🧱 HTML Structure Overview

**Semantic Elements Used:**
- `<form>` — main form container (no action).  
- `<fieldset>` and `<legend>` — for logical grouping and accessibility.  
- `<label>` — properly linked to every input via `for` and `id`.  
- `<input>` — for name, email, and size (radio buttons).  
- `<select>` — for colour selection.  
- `<button type="submit">` — to submit the form.

---

## 🧪 Testing Instructions (DevTools + Lighthouse)

### 1️⃣ Open in Browser
Open `index.html` in Chrome → Right-click → **Inspect** (DevTools).

### 2️⃣ Check the HTML
- All fields are inside a single `<form>` tag.
- Every `<input>` has a matching `<label>`.
- Semantic grouping with `<fieldset>` and `<legend>`.
- There is **no** `action` attribute.

### 3️⃣ Validate the Form
- Try to submit without filling in anything → error should appear.  
- Enter a one-letter name → browser should block submission.  
- Enter invalid email (`test@`) → should be rejected.  
- Don’t choose colour or size → should not submit.

✅ Each field must be validated by the browser.

### 4️⃣ Accessibility Test
1. Open **Lighthouse** tab in DevTools.  
2. Select only **Accessibility**.  
3. Click **Analyze page load**.  
4. Ensure score is **100**.  

If not:
- Check that every `label` is linked to its `input`.
- Ensure all inputs are grouped with a `<fieldset>` and `<legend>`.

### 5️⃣ Keyboard Navigation
- Press **Tab** → focus should move through all form fields in order.  
- Pressing **Space/Enter** on radio buttons should toggle them.  
- Pressing **Enter** on “Submit” should trigger validation.

