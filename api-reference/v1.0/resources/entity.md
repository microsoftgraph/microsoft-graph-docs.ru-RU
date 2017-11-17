# <a name="entity-resource-type"></a>Тип ресурса entity


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение сущности](../api/entity_get.md) | [entity](entity.md) |Чтение свойств и связей объекта сущности.|
|[Удаление](../api/entity_delete.md) | Нет |Удаление объекта сущности. |

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|

## <a name="relationships"></a>Отношения
Нет





## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entity"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->