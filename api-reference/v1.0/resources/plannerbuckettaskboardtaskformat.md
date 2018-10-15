# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>Тип ресурса plannerBucketTaskBoardTaskFormat

Ресурс **plannerBucketTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении Buckets на доске задач (представление, предусматривающее упорядочивание по задачам в сегментах, которым назначены). С каждым объектом [task](plannertask.md) связан один объект **plannerBucketTaskBoardTaskFormat**.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat_get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |Считывание свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.|
|[Обновление](../api/plannerbuckettaskboardtaskformat_update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |Обновление объекта **plannerBucketTaskBoardTaskFormat**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Только для чтения. Идентификатор ресурса. Длина — 28 знаков с учетом регистра. [Проверка формата](planner_identifiers_disclaimer.md) выполняется на службе.|
|orderHint|Строка|Указание, используемое для расположения задач в представлении сегментов на доске задач. Используемый формат описан [здесь](planner_order_hint_format.md).|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->