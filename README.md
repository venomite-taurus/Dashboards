# 🐾 Vet Clinic Dashboard – Power BI Project

A fully interactive **Power BI dashboard** built using real-world style data from a veterinary clinic.  
This project transforms raw Excel data into meaningful insights about **pets, owners, visit patterns, services, and customer communication behavior**.



---

## 📸 Dashboard Preview
![Dashboard Screenshot](./Dashboard.png)  
*(Replace this image with your actual screenshot file name)*

---

## 📁 Dataset Used
**File:** `VetClinic.xlsx`  
The dataset includes details such as:

| Column Name | Description |
|------------|-------------|
| Pet_Name | Name of the pet |
| Breed | Breed category (Bulldog, Labrador, Persian etc.) |
| Pet_Type | Dog / Cat |
| Pet_Age | Age of the pet |
| Owner_Age | Age of the pet owner |
| Visit_Frequency | Number of clinic visits |
| Communication_Channel | Email, SMS, WhatsApp |
| Services_Used | Grooming, Vaccination, Consultation etc. |
| Customer_Cohort | Senior Pets, Young Pets, High-Value Clients, Lapsed Clients etc. |

---

## 🛠 Tools & Technologies
- **Power BI Desktop**
- **Power Query** for data transformations  
- **DAX** for measures & calculated fields  
- **Microsoft Excel** for data preparation  

---

## 📊 Key Insights from Dashboard

### 🐶 1. Pet Demographics  
- Most common breeds visualized using a **pie chart**.  
- Shows top pets like **Bulldog, Labrador, Persian, Husky**, etc.

### 🗓️ 2. Visit Frequency by Breed  
- Highlights which breeds visit the clinic most often.  
- Useful for resource and medical planning.

### 👨‍⚕️ 3. Owner & Pet Age Patterns  
- KPIs summarize **Total Owner Age (9K)** and **Total Pet Age (1.19K)**.  
- Line charts compare age trends across service categories.

### 🐱 4. Pet Type Distribution  
- Donut chart showing **Dogs vs Cats** population split.

### 💬 5. Communication Channel Analysis  
- Displays customer distribution across **Email, SMS, WhatsApp**.

### 🧩 6. Service Usage Across Cohorts  
- Stacked bar charts show which communication channels are most effective for:
  - Senior Pets  
  - Active Young Pets  
  - Mid-Routine Clients  
  - High-Value Clients  
  - Lapsed Returners  
  - Puppy / New Joiners

---

## 📐 Data Modeling
The Power BI data model includes:
- Single table clean structure
- Categorized columns  
- Date and numeric standardization  
- Custom DAX Measures such as:  
  ```DAX
  Total Owner Age = SUM('VetClinic'[Owner_Age])
  Total Pet Age = SUM('VetClinic'[Pet_Age])
