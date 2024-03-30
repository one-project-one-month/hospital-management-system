## Hospital-Management-System

> Hospital Management System မှာ အဓိက ရည်ရွယ်ချက်က ဆေးရုံမှာပြသ‌ချင်တဲ့ လူနာက ကြိုတင် ရက်ချိန်းယူလို့ရအောင် Hospital ဘက်က ဖုန်းနဲ့ လက်ခံပြီး ရက်ချိန်းတွေကို မှတ်သားနိုင်ဖို့ ဒီ System ကိုရေးသားထားခြင်းဖြစ်ပါတယ်

 ---------------------------------

Tech Stack
Frontend - React, Vite, shadcn/ui
backend - Node.js, Express.js, PostgreSQL

Frontend Repository ကို ဒီ [Link](https://github.com/sannlynnhtun-coding/hospital_management_system_frontend) မှာ ကြည့်လို့ရပါတယ်
Backend Repository ကို ဒီ [Link](https://github.com/sannlynnhtun-coding/hospital_management_system_backend) ကနေ စမ်းလို့ရပါတယ်

---------------------------------

ပါ၀င်တဲ့ Table တွေကတော့
1. Doctor
2. Patient
3. Appointment
4. Medical Record
5. Disease
6. Specialist
7. Room

## Contributors

### Frontend
<table>
 <thead>
  <tr>
   <th colspan="12">Contributors</th>
  </tr>
 </thead>
    <tbody>
        <tr>
            <td><a href="https://github.com/Aung-myat-min"><img src="https://github.com/Aung-myat-min.png" width="60px;"/></a></td>
            <td><a href="https://github.com/Kha-10"><img src="https://github.com/Kha-10.png" width="60px;"/></a></td>
            <td><a href="https://github.com/Arkar08"><img src="https://github.com/Arkar08.png" width="60px;"/></a></td>
            <td><a href="https://github.com/CraziiIvan"><img src="https://github.com/CraziiIvan.png" width="60px;"/></a></td>
           <td><a href="https://github.com/htooa2014"><img src="https://github.com/htooa2014.png" width="60px;"/></a></td>
           <td><a href="https://github.com/mr-kmh"><img src="https://github.com/mr-kmh.png" width="60px;"/></a></td>
          <td><a href="https://github.com/htetahyan"><img src="https://github.com/htetahyan.png" width="60px;"/></a></td>
           <td><a href="https://github.com/Kaung-Myat-Hun"><img src="https://github.com/Kaung-Myat-Hun.png" width="60px;"/></a></td>
        </tr>
    </tbody>
</table>

### Backend
<table>
 <thead>
  <tr>
   <th colspan="12">Contributors</th>
  </tr>
 </thead>
    <tbody>
        <tr>
           <td><a href="https://github.com/mr-kmh"><img src="https://github.com/mr-kmh.png" width="60px;"/></a></td>
           <td><a href="https://github.com/GerVaf"><img src="https://github.com/GerVaf.png" width="60px;"/></a></td>
           <td><a href="https://github.com/Kaung-Myat-Hun"><img src="https://github.com/Kaung-Myat-Hun.png" width="60px;"/></a></td>
        </tr>
    </tbody>
</table>

**Description**

Hospital Management System ကို ကိုလင်းရဲ့ ဦးဆောင်မှုဖြင့် စတင်ခဲ့ပြီး တစ်လအတွင်းပြီးနိုင်‌‌လောက်သည်အထိ scope သတ်မှတ်ခဲ့ပါတယ်။ HMS က ဆေးရုံရဲ့ လုပ်ငန်းဆောင်တာအချို့ကို လုပ်ဆောင်ရမှာ လွယ်ကူစေရန် ရည်ရွယ်ခဲ့ပါတယ်။ HMS တွင် လူနာတွေရဲ့ အချက်အလက်တွေ၊ ဆရာဝန်‌တွေရဲ့ အချက်အလက်‌ တွေ၊ သိမ်းဆည်းထားနိုင်ပြီး လျှင်မြန်စွာ ရှာဖွေကြည့်ရှုနိုင်ပါတယ်။ HMS တွင် လူနာအချက်အသစ်လုပ်ခြင်း၊ လူနာအချက်အလက်ပြင်ဆင်ခြင်းစတဲ့ patient management ကို လွယ်ကူစွာလုပ်ဆောင်နိုင်ပါတယ်။ ဆရာဝန်နှင့် ပြသလိုလျှင်လည်း ရက်ချိန်းများလည်း လုပ်ဆောင်နိုင်ပါသည်။

### Doctor
> ဆရာဝန်ရဲ့ အချက်အလက်များ သိမ်းရန်၊ Patient နဲ့ Appointment ချိတ်ဆက်ပေးရန်

```
 Id Int
 DoctorName    String
 Email         String
 MobileNumber  String
 SpecialistId  Int            
 StartDuty     String
 EndDuty       String
```

### Patient
> လူနာတွေရဲ့ အချက်အလက်များသိမ်းရန်၊ Doctor နဲ့ Appointment ချိတ်ဆက်ပေးရန်

```
  Id            Int    
  Name          String   
  Gender        String 
  PhoneNumber   String   
  Email         String   
  BloodType     String  
  BirthDate     DateTime  
  Address       String
```

### Appointment
> Appointment data သိမ်းရန်၊ Doctor နဲ့ Patient ချိတ်ဆက်ပေးရန်

```
  Id              Int  
  PatientId       Int
  DoctorId        Int
  AppointmentDate DateTime
  RoomId          Int
  TokenId         String 
  Status          String  
  IsCancel        Boolean
```

### Medical Record
> လူနာရဲ့ ဆေးအချက်အလက်မှတ်တမ်းသိမ်းဆည်းရန်၊ Disease နဲ့ Patient ချိတ်ဆက်ပေးရန် 
```
  Id        Int   
  Patient   Patient 
  PatientID Int   
  StartDate DateTime
  EndDate   DateTime
  Diagnosis String
  Note      String
  Treatment String
```

### Disease
> ရောဂါ အချက်အလက်သိမ်းဆည်းရန်၊ Medical Record တွင် Patient နဲ့ ချိတ်ဆက်ရန်
```
  Id             Int   
  Name           String
 ```

### Specialist
> အထူးပြု ရောဂါကုသသော အချက်လက်ကိုသိမ်းဆည်းရန်၊ Doctor နဲ့ ချိတ်ဆက်ရန်
```
  Id    Int   
  Name  String
  Description String
```

### Room
> အခန်းသိမ်းဆည်းရန်၊ Appointment တွင် Doctor နဲ့ Patient အားချိတ်ရန်
```
  Id    Int   
  Name  String
```
