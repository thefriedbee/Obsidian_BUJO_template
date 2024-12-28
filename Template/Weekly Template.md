---
tags:
  - weekly-log
dateStart: <%moment(tp.file.title).startOf("isoWeek").format("YYYY-MM-DD")%>
dateEnd: <%moment(tp.file.title).endOf("isoWeek").format("YYYY-MM-DD")%>
week: <%moment(tp.file.title).format("gggg-[W]ww")%>
memories: 
moods: 
write: 
---

# <%moment(tp.file.title).startOf("isoWeek").format("MM/DD")%> - <%moment(tp.file.title).endOf("isoWeek").format("MM/DD")%>
- [[4.Future log/FutureLog|Future Log]]
- [[5.Yearly Log/<%moment(tp.file.title).format("YYYY")%>|<%moment(tp.file.title).format("YYYY")%>]]/[[3.Monthly Log/<%moment(tp.file.title).format("YYYY-MM")%>|<%moment(tp.file.title).format("MM")%>]]
- [[2.Weekly Log/<%moment(tp.file.title).subtract(1,'week').format("gggg-[W]ww")%>|Previous week]] | [[2.Weekly Log/<%moment(tp.file.title).add(1,'week').format("gggg-[W]ww")%>|Next week]]
- [[1.Daily Log/<%moment(tp.file.title).startOf("isoWeek").add(0, "day").format("YYYY-MM-DD")%>|Mon]] | [[1.Daily Log/<%moment(tp.file.title).startOf("isoWeek").add(1, "day").format("YYYY-MM-DD")%>|Tue]] | [[1.Daily Log/<%moment(tp.file.title).startOf("isoWeek").add(2, "day").format("YYYY-MM-DD")%>|Wed]] | [[1.Daily Log/<%moment(tp.file.title).startOf("isoWeek").add(3, "day").format("YYYY-MM-DD")%>|Thu]] | [[1.Daily Log/<%moment(tp.file.title).startOf("isoWeek").add(4, "day").format("YYYY-MM-DD")%>|Fri]] | [[1.Daily Log/<%moment(tp.file.title).startOf("isoWeek").add(5, "day").format("YYYY-MM-DD")%>|Sat]] | [[1.Daily Log/<%moment(tp.file.title).startOf("isoWeek").add(6, "day").format("YYYY-MM-DD")%>|Sun]]


# Weekly Plan
## Objectives

## Weekly TODOs
- [ ] House maintenance 
- [ ] Grocery

# Weekly Review

### Reminders
- [ ] Review this week (<%* tR+="@"%><%moment(tp.file.title).startOf("isoWeek").add(6, "day").format("YYYY-MM-DD")%> 12:00)

## Habits

```dataview
TABLE
	read AS "📖 read",
	write AS "🖊️ write", 
	log AS "📝 summary",
	workout AS "🏃 workout"
FROM "1.Daily Log" and #daily-log and #<%moment(tp.file.title).format("gggg-[W]ww") %>
SORT date ASC
```


