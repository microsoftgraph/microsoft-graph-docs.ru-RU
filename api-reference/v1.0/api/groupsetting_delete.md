# <a name="delete-a-group-setting"></a>Удаление параметра группы

Удаление параметра группы.

## <a name="prerequisites"></a>Обязательные условия

Для применения этого API требуется одна из указанных ниже **областей**. *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*

> Примечание. Разрешения на выполнение операций создания, обновления и удаления есть только у администраторов клиента.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.


## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает никакие данные в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->