# **Cervical Cancer Analysis**  

## **Overview**  
This project aims to analyze cervical cancer data to identify risk factors and improve early detection strategies. The analysis is motivated by both personal experience and a deep interest in understanding the variables that contribute to the diagnosis and progression of cervical cancer.  

By leveraging machine learning and statistical analysis, this study seeks to uncover patterns that may enhance awareness and prevention of the disease.  

## **Dataset**  
- **Source**: Collected at *Hospital Universitario de Caracas* in Caracas, Venezuela.  
- **Size**: Contains information on **858 patients**.  
- **Features**: Includes **demographic details, lifestyle habits, and medical history records**.  
- **Missing Data**: Some patients chose not to answer certain questions due to privacy concerns.  

## **Project Structure**  
📂 cervical-cancer-analysis
│-- 📂 data
│ │-- 📂 raw (Contains the original dataset in ZIP format)
│ │-- 📂 processed (Preprocessed dataset ready for analysis)
│ │-- 📂 interim (Intermediate transformations, if any)
│
│-- 📂 models (Trained machine learning models will be stored here)
│-- 📂 src
│ │-- app.py (Main script for running predictions)
│ │-- explore.ipynb (Exploratory Data Analysis notebook)
│ │-- utils.py (Helper functions for data preprocessing and analysis)
│
│-- .gitignore
│-- README.md
│-- requirements.txt (List of dependencies needed to run the project)


## **Variables in the Dataset**  
The dataset includes multiple features related to cervical cancer risk factors:  

### **General Variables**  
- **`Age`**: *The person's age.*  
- **`Number of sexual partners`**: *The number of sexual partners the person has had.*  
- **`First sexual intercourse (age)`**: *Age at first sexual intercourse.*  
- **`Num of pregnancies`**: *Number of pregnancies the person has had.*  

### **Risk Habits**  
- **`Smokes`**: *Whether the person smokes (Yes/No).*  
- **`Smokes (years)`**: *Number of years the person has been smoking.*  
- **`Smokes (packs/year)`**: *Number of cigarette packs smoked per year.*  

### **Use of Contraceptives**  
- **`Hormonal Contraceptives`**: *Whether the person uses hormonal contraceptives (Yes/No).*  
- **`Hormonal Contraceptives (years)`**: *Number of years the person has been using hormonal contraceptives.*  
- **`IUD`**: *Whether the person has used an intrauterine device (IUD) (Yes/No).*  
- **`IUD (years)`**: *Number of years with an IUD.*  

### **Sexually Transmitted Diseases (STDs)**  
- **`STDs`**: *Whether the person has had any sexually transmitted disease (Yes/No).*  
- **`STDs (number)`**: *Number of STDs the person has had.*  
- **`STDs:condylomatosis`**, **`STDs:cervical condylomatosis`**, **`STDs:vaginal condylomatosis`**, **`STDs:vulvo-perineal condylomatosis`**: *Different types of condylomas (genital warts caused by HPV).*  
- **`STDs:syphilis`**, **`STDs:pelvic inflammatory disease`**, **`STDs:genital herpes`**, **`STDs:molluscum contagiosum`**, **`STDs:AIDS`**, **`STDs:HIV`**, **`STDs:Hepatitis B`**, **`STDs:HPV`**: *Indicators of whether the person has had these specific diseases.*  

### **STD Diagnosis History**  
- **`STDs: Number of diagnosis`**: *Total number of STD diagnoses received.*  
- **`STDs: Time since first diagnosis`**: *Time in years since the first STD diagnosis.*  
- **`STDs: Time since last diagnosis`**: *Time in years since the last STD diagnosis.*  

### **Medical Diagnoses**  
- **`Dx:Cancer`**: *Whether the person has been diagnosed with cancer.*  
- **`Dx:CIN`**: *Whether the person has been diagnosed with Cervical Intraepithelial Neoplasia (CIN), a precancerous cervical lesion.*  
- **`Dx:HPV`**: *Whether the person has been diagnosed with human papillomavirus (HPV).*  
- **`Dx`**: *General positive diagnosis of a related medical condition.*  

### **Target Variables**  
These variables are likely used to predict cervical cancer:  
- **`Hinselmann: target variable`**: *Result of the Hinselmann test (colposcopy with acetic acid).*  
- **`Schiller: target variable`**: *Result of the Schiller test (colposcopy with Lugol's iodine).*  
- **`Cytology: target variable`**: *Result of the cytology test (Pap smear).*  
- **`Biopsy: target variable`**: *Result of the biopsy test (definitive confirmation of cancer or precancerous lesions).*  

## **Installation and Setup**  
To run this project locally, follow these steps:  

1. **Clone the repository**  
   ```bash
   git clone https://github.com/Elisag28/Cervical_Cancer.git
   cd Cervical_Cancer
