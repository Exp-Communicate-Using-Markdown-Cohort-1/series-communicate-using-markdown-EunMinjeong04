# Head1:Learning Markdown from scratch
This is the first file.
A new figure ![figure|400](https://telepic.yuukidev.me/file/193de1e74d20e54ea169e.png)

# Pseudocode 
```
begin
	shedule <- initSolution()
	savingTalbe <- initSavingTable()
	nextRouteFlag <- False
	u,v,saving <- findMaxSaving(savingTable)
	savingTalbe <- updateSavingTable()
	currentRoute = [u,v]
	while len(notVisted) > 0
		if not nextRouteFlag
			head <- currentRoute[0]
			tail <- currentRoute[-1]
			nextArc,saving <- findMaxSaving(head,tail,savingTable)
			if saving < terminalThresh
				nextRouteFlag <-True
				shedule <- addToSchedule(currentRoute)
			else
				currentRoute <- bestMerge(currentRoute,nextArc)
				shedule <- removeFromSchedule(nextArc.Route)
				savingTalbe <- updateSavingTable()
			end if
		else
			u,v,saving <- findMaxSaving(savingTable)
			currentRoute = [u,v]
			savingTalbe <- updateSavingTable()
			nextRouteFlag <- False
		end if 
	end while
end
```
# Task list 
- [x] Merge Algorithm
- [ ] Split method
