# GIT pre-commit hook for php projects #

This hook check saving code before you save commit.

## Install
- copy files into `.git/hooks/` folder of project
- delete not needed executors from `pre-commit.d` folder 

## Executors
- `php-vardump`   - check for absence in php files `var_dump` and `print_r` functions
- `js-consolelog` - check for absence in js files `console.log` function
- `phpunit`       - run `phpunit` from `vendor/bin` and check for errors
- `phpstan`       - run `phpstan` from `vendor/bin` and check for errors
- `codeception`   - run `codecept` from `vendor/bin` and check for errors
- `robo-parallel` - run `robo` from `vendor/bin` and check for errors

## Ignore checking
If you know what you are doing:

`git commit --no-verify`
