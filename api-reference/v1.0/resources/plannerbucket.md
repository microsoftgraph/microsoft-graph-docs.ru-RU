# <a name="plannerbucket-resource-type"></a>Тип ресурса plannerBucket

Ресурс **plannerBucket** представляет сегмент (или "специальный столбец") для задач плана в Office 365. Он содержится в объекте [plannerPlan](plannerPlan.md) и может содержать коллекцию объектов [plannerTasks](plannerTask.md).



### <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerBucket](../api/plannerbucket_get.md) | [plannerBucket](plannerbucket.md) |Чтение свойств и отношений объекта **plannerBucket**.|
|[Перечисление объектов plannerTasks](../api/plannerbucket_list_tasks.md) |Коллекция объектов [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Создание](../api/planner_post_buckets.md) | [plannerBucket](plannerbucket.md)    | Создание объекта **plannerBucket**. |
|[Обновление](../api/plannerbucket_update.md) | [plannerBucket](plannerbucket.md)    |Обновление объекта **plannerBucket**. |
|[Удаление](../api/plannerbucket_delete.md) | Нет |Удаление объекта **plannerBucket**. |

### <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор сегмента. Идентификатор состоит из 28 символов и чувствителен к регистру. [Проверка формата](planner_identifiers_disclaimer.md) выполняется для службы.|
|name|Строка|Имя сегмента.|
|orderHint|Строка|Указание, используемое для упорядочивания элементов этого типа в списке. Используемый формат описан [здесь](planner_order_hint_format.md).|
|planId|Строка|Идентификатор плана, к которому относится сегмент.|

### <a name="relationships"></a>Отношения
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Коллекция задач в сегменте.|

### <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->