***
***
# strings
***
```Go 
ReplaceAll(s, old, new string) string
```
Returns a copy of the string *s* with all 
non-overlapping instances of *old* replaced by *new*.

```Go
Split(s string, sep string) []string
```


```Go
NewReader(s string) *Reader
```
It converts a *string* into an implementation of the *io.Reader* interface.

```Go
TrimSpace(s string) string
```
Returns a new *string* with all leading and trailing whitespace characters removed. 
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

***

# log

```Go
func SetFlags(log.Lshortfile)

func SetOutput(w io.Writer)
func Print(v ...any)
func Printf(v ...any)
func Fatalf(v ...any)
```

***
# os 

```Go
func (*File) Read(b []byte) (n int, err error)
func Open(name string) (*File, error)
func Copy(dst io.Writer, src io.Reader) (written int64, err error)
```
***
# io
***
```Go
type Writer interface {
	Write(p []byte) (n int, err error)
}
```
If defines the contract for writing data to a destination
***

***
# bytes
***
```Go
bytes.Buffer // implements the io.Writer interface

func (b *Buffer) WriteString(s string) (n int, err error) // n is the number of bytes written
```


***
# fmt
***
```Go
func Fprintf(w io.Writer, format string, a ...any) (n int, err error)
```
***