# Makefile

## Print help

```Makefile
help: ## this help
  @grep -hE '^[a-zA-Z_-]+.*?:.*?## .*$$' ${MAKEFILE_LIST} | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'

goal1: ## goal1 the goal#
  echo goal1
  
goal2: goal1 ## goal2 the goal#
  echo goal2
```
