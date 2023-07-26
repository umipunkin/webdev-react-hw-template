# Skypro.Music API

API для музыкального плеера, позволяет получает разные плейлисты с музыкой и управлять избранными треками пользователя.

Документация в swagger:
https://painassasin.online/swagger/

## Пользователи и авторизация

- [Документация API «Пользователи и авторизация»](./docs/AuthAPI.md)

## Плейлисты и треки

Api для управления плейлистами пользователя и получения треков.

Документация в swagger:
https://painassasin.online/swagger/

| Описание запроса                    | Тип запроса | Пример запроса                                           |
| ----------------------------------- | ----------- | -------------------------------------------------------- |
| Получить все треки                  | GET         | https://painassasin.online/catalog/track/all/            |
| Получить трек по id                 | GET         | https://painassasin.online/catalog/track/<id\>           |
| Посмотреть подборки                 | GET         | https://painassasin.online/catalog/selection/            |
| Посмотреть подборку по id           | GET         | https://painassasin.online/catalog/selection/<id\>/      |
| Добавить трек в избранное по id \*  | POST        | https://painassasin.online/catalog/track/<id\>/favorite/ |
| Удалить трек из избранного по id \* | DELETE      | https://painassasin.online/catalog/track/<id\>/favorite/ |
| Получить все избранные треки \*     | GET         | https://painassasin.online/catalog/track/favorite/all/   |

Запросы отмеченные \* требуют авторизацию.
