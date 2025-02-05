[![Go Reference][goreference_badge]][goreference_link]
[![Go Report Card][goreportcard_badge]][goreportcard_link]
 
<!-- Code generated by gomarkdoc. DO NOT EDIT -->

# set

```go
import "github.com/bruceesmith/set"
```

Package set is based on public code from [John Arundel](<https://bitfieldconsulting.com/posts/generic-set>), goroutine safety added. It defines goroutine\-safe methods for manipulating a generic [set](<https://en.wikipedia.org/wiki/Set_(abstract_data_type)>) data structure via the standard operations Add, Contains, Intersection, Members, String and Union

## Index

- [type Set](<#Set>)
  - [func New\[E comparable\]\(vals ...E\) \*Set\[E\]](<#New>)
  - [func \(s \*Set\[E\]\) Add\(vals ...E\)](<#Set[E].Add>)
  - [func \(s \*Set\[E\]\) Clear\(\)](<#Set[E].Clear>)
  - [func \(s \*Set\[E\]\) Contains\(v E\) bool](<#Set[E].Contains>)
  - [func \(s \*Set\[E\]\) Delete\(vals ...E\)](<#Set[E].Delete>)
  - [func \(s \*Set\[E\]\) Difference\(s2 \*Set\[E\]\) \*Set\[E\]](<#Set[E].Difference>)
  - [func \(s \*Set\[E\]\) Disjoint\(s2 \*Set\[E\]\) bool](<#Set[E].Disjoint>)
  - [func \(s \*Set\[E\]\) Empty\(\) bool](<#Set[E].Empty>)
  - [func \(s \*Set\[E\]\) Intersection\(s2 \*Set\[E\]\) \*Set\[E\]](<#Set[E].Intersection>)
  - [func \(s \*Set\[E\]\) Members\(\) \[\]E](<#Set[E].Members>)
  - [func \(s \*Set\[E\]\) Size\(\) int](<#Set[E].Size>)
  - [func \(s \*Set\[E\]\) String\(\) string](<#Set[E].String>)
  - [func \(s \*Set\[E\]\) Union\(s2 \*Set\[E\]\) \*Set\[E\]](<#Set[E].Union>)


<a name="Set"></a>
## type Set

Set is a generics implementation of the set data type

```go
type Set[E comparable] struct {
    // contains filtered or unexported fields
}
```

<a name="New"></a>
### func New

```go
func New[E comparable](vals ...E) *Set[E]
```

New creates a new Set

<a name="Set[E].Add"></a>
### func \(\*Set\[E\]\) Add

```go
func (s *Set[E]) Add(vals ...E)
```

Add puts a new value into a Set

<a name="Set[E].Clear"></a>
### func \(\*Set\[E\]\) Clear

```go
func (s *Set[E]) Clear()
```

Clear removes all values from a Set

<a name="Set[E].Contains"></a>
### func \(\*Set\[E\]\) Contains

```go
func (s *Set[E]) Contains(v E) bool
```

Contains checks if a value is in the Set

<a name="Set[E].Delete"></a>
### func \(\*Set\[E\]\) Delete

```go
func (s *Set[E]) Delete(vals ...E)
```

Delete remove values\(s\) from a Set

<a name="Set[E].Difference"></a>
### func \(\*Set\[E\]\) Difference

```go
func (s *Set[E]) Difference(s2 *Set[E]) *Set[E]
```

Difference returns the set of values that are in s \(set A\) but not in s2 \(set B\) ... i.e. A \- B

<a name="Set[E].Disjoint"></a>
### func \(\*Set\[E\]\) Disjoint

```go
func (s *Set[E]) Disjoint(s2 *Set[E]) bool
```

Disjoint returns true if the intersection of s with another set s2 is empty

<a name="Set[E].Empty"></a>
### func \(\*Set\[E\]\) Empty

```go
func (s *Set[E]) Empty() bool
```

Empty returns true if the Set is empty

<a name="Set[E].Intersection"></a>
### func \(\*Set\[E\]\) Intersection

```go
func (s *Set[E]) Intersection(s2 *Set[E]) *Set[E]
```

Intersection returns the logical intersection of 2 Sets

<a name="Set[E].Members"></a>
### func \(\*Set\[E\]\) Members

```go
func (s *Set[E]) Members() []E
```

Members returns a slice of the values in a Set

<a name="Set[E].Size"></a>
### func \(\*Set\[E\]\) Size

```go
func (s *Set[E]) Size() int
```

Size returns the number of values in a Set

<a name="Set[E].String"></a>
### func \(\*Set\[E\]\) String

```go
func (s *Set[E]) String() string
```

String returns a string representation of the Set members

<a name="Set[E].Union"></a>
### func \(\*Set\[E\]\) Union

```go
func (s *Set[E]) Union(s2 *Set[E]) *Set[E]
```

Union returns the logical union of 2 Sets

Generated by [gomarkdoc](<https://github.com/princjef/gomarkdoc>)
 
[goreference_badge]: https://pkg.go.dev/badge/github.com/bruceesmith/set/v3.svg
[goreference_link]: https://pkg.go.dev/github.com/bruceesmith/set
[goreportcard_badge]: https://goreportcard.com/badge/github.com/bruceesmith/set
[goreportcard_link]: https://goreportcard.com/report/github.com/bruceesmith/set
