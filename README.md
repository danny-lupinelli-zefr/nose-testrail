# nose-testrail

This plugin is designed to work with DDT in updating test rails.

For example:

prefix your test case with the follwing lines:

#1_test:1_case_id Mapping
@case_id([10, 300, 400])
@data(200,800,4040)
test_some_function(self, input, expexted)

For input 200 the test_case_id = 10 will be updated in test rails, for 800 will update test_case_id=800 and 4040 updates test_case_id = 400.


or

#1_test:many_case_ids Mapping

case_id('[100,444,33]')
@data(888)
test_some_function(self, input, expexted)

For test run using 888, all three test_case_id will be updated for the one test run.
