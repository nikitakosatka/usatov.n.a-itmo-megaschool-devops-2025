# usatov.n.a-itmo-megaschool-devops-2025

## Helm-чарты

Подготовлены Helm-чарты для Time-Server (ifilyaninitmo/time-server-mega-itmo:main) и Auth-Server
(ifilyaninitmo/auth-server-mega-itmo:main).

## GitHub Workflow

Подготовлен GitHub-Workflow для проверки Helm-чартов (helm-check-action).

## Развертывание

1) Установить MongoDB на Minikube, используя Helm-чарт из [репозитория](https://github.com/mongodb/helm-charts)

2) Установить Time Server и Auth Server
```sh
helm install time-server ./charts/time-server

helm install auth-server ./charts/auth-server
```

### Try it out

Swagger для Auth Server доступен по endpoint'у `/docs`