# <a name="plannerplan-resource-type"></a>Тип ресурса plannerPlan

Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать [группе](group.md). Он содержит коллекцию объектов [plannerTask](plannerTask.md). Кроме того, он может содержать коллекцию объектов [plannerBucket](plannerBucket.md). Каждый объект plan имеет объект [details](plannerPlanDetails.md), который может содержать дополнительные сведения о плане. Дополнительную информацию о связях между группами, планами и задачами см. в статье с [общими сведениями](planner_overview.md).



### <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение plannerPlan](../api/plannerplan_get.md) | [plannerPlan](plannerplan.md) |Считывание свойств и связей объекта **plannerPlan**.|
|[Перечисление контейнеров](../api/plannerplan_list_buckets.md) |Коллекция [plannerBucket](plannerbucket.md)| Получение коллекции объектов **plannerBucket**.|
|[Перечисление задач](../api/plannerplan_list_tasks.md) |Коллекция [plannerTask](plannertask.md)| Получение коллекции объектов **plannerTask**.|
|[Обновление](../api/plannerplan_update.md) | [plannerPlan](plannerplan.md)    |Обновление объекта **plannerPlan**. |

### <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Только для чтения. Идентификатор плана. Содержит 28 знаков, учитывается регистр. [Проверка формата](planner_identifiers_disclaimer.md) выполняется в службе.|
|owner|String|Идентификатор [группы](group.md), которая является владельцем плана. В этом поле можно указать только идентификатор существующей группы, которая допустима. После задания значения его сможет обновить только владелец.|
|title|String|Обязательный. Название плана.|
|createdBy|[identitySet](identityset.md)|Только для чтения. Пользователь, создавший план.|

### <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция [plannerBucket](plannerbucket.md)| Только для чтения. Допускает значение null. Коллекция контейнеров в плане.|
|details|[plannerPlanDetails](plannerplandetails.md)| Только для чтения. Допускает значение null. Дополнительные сведения о плане.|
|tasks|Коллекция [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Коллекция задач в плане.|

### <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->