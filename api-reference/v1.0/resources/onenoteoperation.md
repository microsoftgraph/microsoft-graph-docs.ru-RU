# <a name="onenoteoperation-resource-type"></a>Тип ресурса onenoteOperation

Состояние определенных операций OneNote, выполняющихся в течение длительного времени.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |Время начала операции.|
|error|[onenoteOperationError](onenoteoperationerror.md)|Ошибка при выполнении операции.|
|id|string|Идентификатор операции. Только для чтения.|
|lastActionDateTime| DateTimeOffset |Время последнего действия операции.|
|resourceId|string|Идентификатор ресурса.|
|resourceLocation|string|URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела. |
|status|string|Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`. |
|percentComplete|string|Процент завершения операции, если операция в состоянии `running`.

## <a name="relationships"></a>Связи
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение операции](../api/onenoteoperation_get.md) | [onenoteOperation](onenoteoperation.md) |Получение состояния операции. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
