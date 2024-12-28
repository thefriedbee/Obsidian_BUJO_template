Monthly log creates dashboards for me to view the status...

# Links
- [[5.Yearly Log/<%moment(tp.file.title).format("YYYY")%>| Yearly Log]]

# Review/Summary
Things I did this month:





# Dashboards (trackers)

## weekly summary
```dataview
TABLE
	dateformat(dateStart, "MM-dd") AS "start",
	dateformat(dateEnd, "MM-dd") AS "end",
	memories AS "🖼️", 
	moods AS "♥️"
FROM "2.Weekly Log" and #weekly-log
WHERE contains(file.name,"2024") AND dateStart >= date(<% 
tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD") %>) AND dateStart <= date(<% 
tp.date.now("YYYY-MM-DD", +31, tp.file.title, "YYYY-MM-DD") %>)
SORT dateStart ASC
```


## daily summary
```dataview
TABLE
	read AS "📖 read",
	write AS "🖊️ write", 
	log AS "📝 summary",
	workout AS "🏃 workout"
FROM "1.Daily Log" AND #daily-log 
WHERE date >= date(<% 
tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD") %>) AND date <= date(<% 
tp.date.now("YYYY-MM-DD", +31, tp.file.title, "YYYY-MM-DD") %>)

SORT date ASC
```




















