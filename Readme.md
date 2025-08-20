name: 🌞 NoGlassesClasses - A SunSmart Scheduler
description: |
  Optimizing outdoor and indoor school activities using local sunlight data 
  to promote student health, prevent childhood myopia, and improve productivity.

problem_statement: |
  Excessive sun exposure during school hours can increase the risk of 
  UV-related health issues (e.g., sunburn, heat stress), while insufficient 
  outdoor activity contributes to childhood myopia, physical inactivity, and 
  reduced mental wellbeing.

  Schools need a balanced schedule that maximizes safe outdoor learning 
  opportunities while minimizing health risks from overexposure.

solution: |
  The SunSmart Scheduler dynamically generates a **monthly class timetable** 
  for grades 1–5 that ensures:
    - 2 outdoor classes per day, avoiding peak sun hours
    - Fair distribution of indoor classes across remaining time slots
    - Location-based sunrise/sunset adaptation
    - Exportable schedules in CSV format for easy sharing

  This approach promotes healthier student routines, reduces myopia risk, 
  and balances sunlight exposure with academic needs.

tech_stack:
  - Python 3.9+
  - Astral: Sunrise/Sunset & daylight calculation
  - pytz: Timezone support
  - requests: Location → Coordinates lookup
  - timezonefinderL: Auto-detect timezone (optional)

installation: |
  Clone the repo and install dependencies:
    git clone https://github.com/<your-username>/sunsmart-scheduler.git
    cd sunsmart-scheduler
    pip install -r requirements.txt

usage: |
  Run the scheduler:
    python ans.py

  Sample Run:
    📍 Enter city: Amritsar
    🌍 Enter country: India
    🕒 Auto-detected timezone: Asia/Kolkata
    📅 Enter month (1-12): 8
  
  ✅ Schedules exported to schedules.csv

example_output:
  console: |
    🌞 SunSmart Schedule for Grade 1 in August
    Average daylight hours: 13.2
    -------------------------------------
    Day 1: Outdoor, Indoor, Indoor, Outdoor, Indoor, Indoor
    Day 2: Indoor, Outdoor, Indoor, Indoor, Outdoor, Indoor
  csv: |
    Grade,Date,Classes
    1,2025-08-01,Outdoor, Indoor, Indoor, Outdoor, Indoor
    2,2025-08-01,Indoor, Outdoor, Indoor, Indoor, Outdoor
    3,2025-08-01,Outdoor, Indoor, Outdoor, Indoor, Indoor

features:
  - ✅ Location-based sunrise/sunset calculation
  - ✅ Balances outdoor vs indoor activities
  - ✅ Prevents myopia through daily outdoor scheduling
  - ✅ Exports schedules to CSV for record-keeping
  - ✅ Emoji-enhanced console output for readability

future_improvements:
  - 🌤️ Integrate real-time UV index APIs for more accurate risk assessment
  - 📱 Build a mobile/web dashboard for school admins
  - 🧠 Add machine learning to adapt schedules to historical weather/attendance data
  - 🏫 Extend for higher grades and customizable timetables

impact: |
  By aligning student schedules with natural sunlight cycles, this project 
  reduces risks of myopia and UV exposure while promoting mental and physical wellbeing. 
  It has the potential to directly improve public health outcomes in schools globally.

author:
  name: Supreet Kaur
  email: supreetkaur0602@gmail.com
  linkedin: https://www.linkedin.com/in/1supreetkaur/
