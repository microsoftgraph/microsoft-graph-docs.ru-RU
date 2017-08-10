# <a name="update-a-group-setting"></a>Обновление параметра группы

Обновление свойств для указанных объектов параметров группы.

## <a name="prerequisites"></a>Обязательные условия

Для применения этого API требуется одна из указанных ниже **областей**. *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*

> Примечание. Разрешения на выполнение операций создания, обновления и удаления есть только у администраторов клиента.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->

Обновление параметра на уровне клиента или отдельной группы.

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя | Описание |
|:-----------|:-----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В теле запроса укажите значения для соответствующих полей, которые необходимо обновить. 

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| values | settingValue | Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 OK` и обновленный объект [groupSetting](../resources/groupsetting.md) в теле отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->