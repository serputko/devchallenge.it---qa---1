# devchallenge.it---qa---1

This project was created for api testing of http://petstore.swagger.io/ service.
Prerequisites:
- install JDK8+
- install git

Clone and navigate to repo:
- Clone this repo:
```
git clone https://github.com/ololololololololol/devchallenge.it---qa---1.git
```
- open project directory
```
cd devchallenge.it---qa---1
```
To run test execute next steps accordinly to your OS:
# Mac/Linux
Open test with jmeter GUI(for detailed results)
```
sh apache-jmeter-4.0/bin/jmeter.sh -t scenarios/pets_api_testing.jmx
```

Run test in non GUI mode(Preferable)
```
rm -rf Report/
sh apache-jmeter-4.0/bin/jmeter.sh -nt scenarios/pets_api_testing.jmx -eo Report/ -fl report.csv
```

# Windows
Open test with jmeter GUI(for detailed results)
```
cd apache-jmeter-4.0\
.\bin\jmeter.bat -t ..\scenarios\pets_api_testing.jmx
```

Run test in non GUI mode(Preferable)
```
rmdir .\Report\ /s /q
cd apache-jmeter-4.0\
.\bin\jmeter.bat -nt ..\scenarios\pets_api_testing.jmx -eo ..\Report\ -fl report.csv
```

To view test results please open index.html file in Report/ directory
