# Formulas Reference

# 📘 Formulas Reference – Hospital ER Dashboard (Excel)

### 🧮 Age Group Formula
```excel
=IF([@[Patient Age]]>=70,"70-79",
IF([@[Patient Age]]>=60,"60-69",
IF([@[Patient Age]]>=45,"45-59",
IF([@[Patient Age]]>=30,"30-44",
IF([@[Patient Age]]>=15,"15-29",
IF([@[Patient Age]]>=5,"05-14","0-4"))))))


### ⏱ Timeliness KPI Formula

=IF([@[Wait Time]]<30,"Within Time","Delayed")



📊 Admission Ratio

Use COUNTIF or Pivot Table calculation:

=COUNTIF([Admission Status],"Admitted") / COUNTA([Admission Status])