# <a name="planner-resource-type"></a>Тип ресурса planner

Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.


### <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание объекта plannerBucket](../api/planner_post_buckets.md) |[plannerBucket](plannerbucket.md)| Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.|
|[Создание объекта plannerPlan](../api/planner_post_plans.md) |[plannerPlan](plannerplan.md)| Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.|
|[Создание объекта plannerTask](../api/planner_post_tasks.md) |[plannerTask](plannertask.md)| Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.|

### <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор ресурса **planner**.|

### <a name="relationships"></a>Отношения
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|buckets|Коллекция объектов [plannerBucket](plannerbucket.md)| Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.|
|plans|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.|
|tasks|Коллекция объектов [plannerTask](plannertask.md)| Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.|

### <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->