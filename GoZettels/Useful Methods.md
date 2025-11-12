***
***
# strings
***
```Go 
ReplaceAll(s, old, new string) string
```
Returns a copy of the string *s* with all 
non-overlapping instances of *old* replaced by *new*.
***
***
# time
***
```Go
Tick(d Duration) <-chan Time
```
***
```Go
After(d Duration) <-chan Time
```
It waits for the duration to elapse and then sends the current time on the returned channel. 
***
```Go
Sleep(d Duration)
```
It blocks the current *goroutine* for the specified duration of time.