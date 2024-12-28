---
tags:
  - daily-log
  - <%moment(tp.file.title).format("YYYY-MM-DD")%>
  - <%moment(tp.file.title).format("gggg-[W]ww")%>
date: <%moment(tp.file.title).format("YYYY-MM-DD")%>
week: <%moment(tp.file.title).format("gggg-[W]ww") %>
read: 
write: 
log: 
workout: 
---

## Links
- [[5.Yearly Log/<%moment(tp.file.title).format("YYYY")%>|Yearly Log]]
- [[1.Daily Log/<%tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD")%>|<%tp.date.now("MM-DD", -1, tp.file.title, "YYYY-MM-DD")%>]]<--<%moment(tp.file.title).format("MM-DD")%>-->[[1.Daily Log/<%tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD")%>|<%tp.date.now("MM-DD", 1, tp.file.title, "YYYY-MM-DD")%>]]
- [[5.Yearly Log/<%moment(tp.file.title).format("YYYY")%>|<%moment(tp.file.title).format("YYYY")%>]]/[[3.Monthly Log/<%moment(tp.file.title).format("gggg-MM")%>|<%moment(tp.file.title).format("MM")%>]], [[2.Weekly Log/<%moment(tp.file.title).format("gggg-[W]ww") %>|W<%moment(tp.file.title).format("ww") %>]]
- [[4.Future log/FutureLog|Future Log]]

## 1. Major Work TODOs
- [ ] Task 1

## 2. Events/Deadlines/Commitments
- [ ] An Event
<%*
const weekdayStr = tp.date.now("dddd", 0, tp.file.title, "YYYY-MM-DD");
if (weekdayStr === "Sunday" || weekdayStr === "星期日") {
	tR += "- [ ] Plan new week"
}
%>
<%*
const dateString = tp.file.title; // Assuming the file title is in "YYYY-MM-DD" format
const dateParts = dateString.split("-");
const year = parseInt(dateParts[0], 10);
const month = parseInt(dateParts[1], 10) - 1; // Month is 0-indexed
const day = parseInt(dateParts[2], 10);
const date = new Date(year, month, day);
const lastDayOfMonth = new Date(year, month + 1, 0).getDate(); // Get the last day of the month

if (day === lastDayOfMonth) {
	tR += "- [ ] Review the month";
}
%>

## 3. Notes & ideas


## 4. Time Blocks
### Day Block Planner
- [ ] 9:00 - 10:00 Morning
- [ ] 10:00 - 11:00 Deep activity
- [ ] 11:00 - 12:00 workout
- [ ] 12:00 - 13:30 Deep activity
- [ ] 13:30 - 15:00 Deep activity
- [ ] 15:00 - 16:30 Deep activity
- [ ] 16:30 - 17:30 Dinner
- [ ] 17:30 - 18:30 Rest
- [ ] 18:30 - 19:30 Shallow activity
- [ ] 19:30 - 21:00 Shallow activity
- [ ] 21:00 - 22:00 Shallow activity
- [ ] 22:00 - 23:00 Shallow activity
- [ ] 23:00 - 24:00 Tear down

### Reminders
- [ ] Plan next day (<%* tR+="@"%><%tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD")%> 19:30)
- [ ] Review today (<%* tR+="@"%><%tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD")%> 22:30)


**Bullet Formats**
- Basic bullets
	- [ ] todo (- [ ])
	- [/] incomplete (half completed) (- [/])
	- [x] done (- [x])
	- [-] canceled (- [-])
	 - [I] idea (- [I])
	 - [*] Events (- [\*])
- Migration bullets
	 - [>] forward (to Future Log) (- [>])
	 - [<] re-scheduling (reschedule to the next day's Daily Log) (- [<])
- Extended bullets
	- [i] important (- [i])
	- [u] up (- [u])
	- [d] down (- [d])
	- ["] quote (- ["])
	- [l] location (- [l])



