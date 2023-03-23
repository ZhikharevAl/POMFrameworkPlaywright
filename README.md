# 🎭Automate web browsers with [Python](https://www.python.org/) and [Playwright](https://playwright.dev/python/).
|               | Linux | Windows | macOS |
|---------------|-------|---------|-------|
| **Chromium**  | ✅     | ✅       | ✅     |
| **WebKit**    | ✅     | ✅       | ✅     |
| **Firefox**   | ✅     | ✅       | ✅     |

## ❓What is Playwright

>Playwright was created specifically to accommodate the needs of end-to-end testing. Playwright supports all modern rendering engines including Chromium, WebKit, and Firefox. Test on Windows, Linux, and macOS, locally or on CI, headless or headed with native mobile emulation.


## 📖 Documentation:

https://playwright.dev/python/docs/intro

## ❕Requirements:
* To run this testing framework, you will need:

  * [Python](https://www.python.org/) 3.7 or higher
  * [Docker](https://www.docker.com/) (if you want to run the tests in a container)
  * [Docker-compose](https://docs.docker.com/compose/) (if you want to run the tests in a container)
  * [Allure](https://github.com/allure-framework) (if you want to generate test reports)

## 🔧 Installation: 

- Install the [Pytest plugin](https://pypi.org/project/pytest-playwright/):
```sh
pip install pytest-playwright
```
- Install the required browsers:
```sh
playwright install
```


## 🚀 Running:
Follow these steps to install the necessary packages:
1. Clone the repository:
```sh
git clone https://github.com/ZhikharevAl/python-playwright-demo-project.git
```

2. Create and activate a virtual environment:
```sh
python3 -m venv venv
source venv/bin/activate
```
3. To install dependencies from the requirements.txt file, run the following command:
```sh
pip install -r requirements.txt
```
4. To run the example test, use the following command:
```sh
pytest -s --headed --slowmo 800 -k test_homepage_has_Playwright_in_title_and_get_started_link_linking_to_the_intro_page
```
## 🐳 [Docker](https://www.docker.com/):
>Docker is a platform for developing, delivering, and running applications in containers. In the context of testing, Docker can be used to run tests in isolated containers to ensure environment consistency and avoid conflicts between dependencies. In this example, if you want to run tests in a Docker container, you need to install Docker and Docker-compose. Then, to run tests in a container, use the following command:
```sh
docker build -t <Container name> .
docker run -it <Container name>
docker-compose up
```
## 📈 [Allure Framework](https://github.com/allure-framework):
>Allure is a framework and report generator that can be used to create beautiful and informative reports on test results. In this example, Allure is used to generate reports on test execution results. If you want to generate reports, you need to install Allure and run tests with the --alluredir parameter, as shown below:
```sh
pytest --alluredir=allure-results
```
>After running tests, you can generate Allure reports using the command:

```sh
allure serve allure-results
```
## 📝 License:
This project is licensed under the MIT License - see the [LICENSE](https://ru.wikipedia.org/wiki/Лицензия_MIT) file for details.
## ![Jokes Card](https://readme-jokes.vercel.app/api)