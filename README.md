# Power BI Sales Analysis Dashboard

Bu layihə 2024-2025-ci illər üzrə satış məlumatlarının təhlili üçün hazırlanmış Power BI dashboard-udur.

## Layihə haqqında

Mən bu analizi junior data analyst kimi təcrübə qazanmaq məqsədilə hazırlamışam. Məlumatlar Azərbaycanın müxtəlif regionları üzrə satışları əhatə edir (Bakı, Gəncə, Sumqayıt, Lənkəran, Şəki).

### Əsas göstəricilər (KPIs)
- Ümumi Satış Həcmi
- Ümumi Mənfəət (Sales - Cost)
- Orta Sifariş Dəyəri
- Endirim təsiri
- Region və Kateqoriya üzrə performans

### Dashboard səhifələri
1. **Overview** – Əsas KPI kartları, satış trendi (line chart), region xəritəsi
2. **Product Performance** – Kateqoriya və məhsul üzrə bar chart, top 10 məhsul
3. **Customer Analysis** – Müştəri seqmentasiyası, təkrar alışlar
4. **Regional Deep Dive** – Region filter-ləri ilə detallı baxış

## Quraşdırma

1. `data/sales_data.csv` faylını Power BI Desktop-a import edin
2. Data model-də Date table yaradın (OrderDate əsasında)
3. `measures/` qovluğundakı DAX ölçülərini əlavə edin
4. Visuals-ları documentation-da göstərilən kimi qurun

## Məlumat mənbəyi
- 50 ədəd sifariş qeydi (nümunə data, asanlıqla genişləndirilə bilər)
- Tarix aralığı: Yanvar 2024 – Avqust 2025
- Sahələr: OrderID, OrderDate, Region, Category, Product, Customer, Quantity, UnitPrice, Discount%, SalesAmount, Cost

## Qeyd
Bu layihə təlim məqsədlidir. Real biznes məlumatı deyil. 
Hər hansı sualınız olsa issue açın və ya mənimlə əlaqə saxlayın.

---
Vusal Mammadzade  
Junior Data Analyst  
