# travis-notify-geckoboard

Notify Geckoboard widgets with Travis CI build results

![Screenshot of passing build](screenshot-build-passed.png)
![Screenshot of failing build](screenshot-build-failed.png)

## Usage

1. Add a custom text widget to your Geckoboard dashboard
2. Add this to your `.travis.yml`:

``` yaml
before-script: npm install -g travis-notify-geckoboard
after-script: travis-notify-geckoboard -a GECKOBOARD_API_KEY -w GECKOBOARD_WIDGET_KEY
```
