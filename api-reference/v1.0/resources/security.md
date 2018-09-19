# <a name="security-resource-type"></a>тип ресурса безопасности

Ресурс безопасности — это точка входа для объектной модели Security. Она выводит одноэлементный ресурс безопасности. Не содержит свойства, которые можно использовать.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [|||UNTRANSLATED_CONTENT_START|||List alerts|||UNTRANSLATED_CONTENT_END|||](../api/alert_list.md) | коллекция [alert](alert.md) | Получение коллекции объектов alert. |
| [получить оповещения](../api/alert_get.md) | коллекция [alert](alert.md) | Получить объект alert. |
| [Обновление оповещений](../api/alert_update.md) | коллекция [alert](alert.md) | Получить объект alert. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|оповещения|коллекция [alert](alert.md)| Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>Пример

Ресурс**безопасности** доступен в корневом каталоге Graph.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->