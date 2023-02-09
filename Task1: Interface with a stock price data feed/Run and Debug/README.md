## Output from Terminal

Initially we have an output from client.py as Ratio 1 , In order to get the Output 

First, Run server.py and client.py (in that order) and take a look at the output. You should notice two things:
○ The Ratio in the client output is always 1
○ The price of each stock is always the same as its bid

Before you run the client.py file , run the server.py

<img width="830" alt="server" src="https://user-images.githubusercontent.com/104922257/217687158-d8368b2d-0be8-49bd-a2ff-545f13f2e667.png">

After running server.py, Run client.py

<img width="760" alt="client py output" src="https://user-images.githubusercontent.com/104922257/217687177-2d8c8e31-f197-420d-98e8-a9f75bd89940.png">

When Query received the server keeps running and is as below: 

<img width="795" alt="Query server" src="https://user-images.githubusercontent.com/104922257/217687196-b149fef6-48ae-47f9-9ccf-641d0c07be89.png">

Before passing the test. We make the test fail called as Test Driven Development ( TDD ).


```
import unittest

class TestClass(unittest.TestCase):
  def test1(self)
      self.fail
      
  def test2(self)
      self.fail
      
if '__name__' == '__main__'
   unittest.main() 
   
   ```
   
Example : ![image](https://user-images.githubusercontent.com/104922257/217695234-56bf1b66-58b1-4bfb-8407-521086063791.png)
   
#### Test passed

<img width="935" alt="test output" src="https://user-images.githubusercontent.com/104922257/217687201-c81d731b-fc33-4c98-ac81-92db36b09518.png">
