## Suite example
```go
package tests

import (
	"testing"

	"github.com/stretchr/testify/assert"
	"github.com/stretchr/testify/mock"
	"github.com/stretchr/testify/suite"
)

type Suite struct {
	suite.Suite
	/*...*/
}
  

func TestSuite(t *testing.T) {
	s := Suite{}
	suite.Run(t, &s)
}
  
// will run only once at the beginning of the suite
func (s Suite) SetupSuite() {
	/*...*/
}

func (s Suite) TestXYZ() {
	assertion := assert.New(s.T())
	/*...*/
}
