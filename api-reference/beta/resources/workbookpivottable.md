<a id="pivottable-resource-type" class="xliff"></a>
# Тип ресурсов pivotTable

Представляет сводную таблицу Excel.

<a id="methods" class="xliff"></a>
## Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение workbookPivotTable](../api/workbookpivottable_get.md) | [workbookPivotTable](workbookpivottable.md) |Чтение свойств и связей объекта workbookPivotTable.|
|[Refresh](../api/workbookpivottable_refresh.md)|Нет|Обновляет сводную таблицу. |
|[Refreshall](../api/workbookpivottable_refreshall.md)|Нет|Обновляет все таблицы на заданном листе. Обратите внимание, что это действие доступно только в коллекции сводных таблиц.|

<a id="properties" class="xliff"></a>
## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Идентификатор сводной таблицы.   Только для чтения.|
|name|String|Имя сводной таблицы.    |

<a id="relationships" class="xliff"></a>
## Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|worksheet|[worksheet](worksheet.md)| Лист, содержащий текущую сводную таблицу. Только для чтения.   |

<a id="json-representation" class="xliff"></a>
## Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
