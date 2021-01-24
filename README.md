![LambdaTest Logo](https://www.lambdatest.com/static/images/logo.svg)
---

# python-lettuce-todo
Lettuce integration with LambdaTest<br/>


### Setup
Install depedencies ```pip install -r requirements.txt```
### Configuration steps
##### Setting locally
- Set LambdaTest username and access key in environment variables. It can be obtained from [LambdaTest dashboard](https://automation.lambdatest.com/)
example:
- For linux/mac
```
   export LT_USERNAME="YOUR_USERNAME"
   export LT_ACCESS_KEY="YOUR ACCESS KEY"
  
```
- For Windows
```
   set LT_USERNAME="YOUR_USERNAME"
   set LT_ACCESS_KEY="YOUR ACCESS KEY"
  
```
For setting capaibilies,Update `config.json`  (List of supported OS platfrom, Browser, resolutions can be found at [LambdaTest capability generator](https://www.lambdatest.com/capabilities-generator/))
 example:
```
   [
     {
        "platform": "win10",
        "browserName": "chrome",
        "version": "67.0",
        "resolution": "1024x768",
        "name": "this is the behave test",
        "build": "behave-test-lambdatest"
     }
   ]
```
##### Setting test through jenkins
Please refer this [url](https://www.lambdatest.com/support/docs/display/TD/Selenium+with+Jenkins)
#####  Routing traffic through your local machine
- Set tunnel value to `true` in test capabilities
> OS specific instructions to download and setup tunnel binary can be found at the following links.
>    - [Windows](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+Windows)
>    - [Mac](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+MacOS)
>    - [Linux](https://www.lambdatest.com/support/docs/display/TD/Local+Testing+For+Linux)

### Run tests
##### Running tests
```bash
paver run 
```

##### Running tests through LambdaTest Jenkins Plugin
```bash
paver run jenkins
```


