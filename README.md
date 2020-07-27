# igeAutoTest

C++ extension Firebase Auto Test Lab for 3D and 2D games.

### Before running this tutorial, you have to install igeAutoTest
	[pip install igeAutoTest]

### Functions
- First, you need to impor the module
	```
	import igeAutoTest
	```
- Helper function
	- Check if the game is running with Auto Test or not
		```
		auto_test = igeAutoTest.isLoopTest()
		```
	- Capture the screenshot, the image will be saved under **.jpg** format with the name based on the system time
		```
		igeAutoTest.screenshots()
		```
	- Write message information to a results file, in string format
		```
		igeAutoTest.writeResultsTest(message)
		```
	- Finish the auto test loop, all the result information and screenshot will be upload to **Test Lab** firebase console
		```
		igeAutoTest.finishLoopTest()
		```
	- The default test loop result should be (**result.json**)
		```json
		{
			"Adjust": {
				"adid": "ff96ad57fa7e09cbf776a768dceca0f7",
				"debug": true,
				"event": [],
				"secret": "(1, 1665077278, 978761167, 1927431060, 1766817079)",
				"token": "hpqyvx4aumm8"
			},
			"Applovin": {
				"banner": "543b53f89be58d39",
				"interstitial": "ded4ed1fe2aa54e0",
				"rewarded": "3602eab376c95aa3"
			},
			"GameAnalytics": {
				"debug": true,
				"event": {
				"complete": [
					"world01"
				],
				"fail": [],
				"start": [
					"world01",
					"world02",
					"world03",
					"world04"
				]
				},
				"game_key": "5382b405e69fa73d7c0464c768b57a5f",
				"secret_key": "9951c60e96346307c889484cd76bece4ae833ee2"
			},
			"Result": "Success"
		}
	```
### Reference
- https://firebase.google.com/docs/test-lab

