<a id="plannergroup-resource-type" class="xliff"></a>
# Тип ресурса plannerGroup

Ресурс **plannerGroup** предоставляет доступ к ресурсам Планировщика для [группы](group.md). Он не содержит свойства, которые можно использовать.

<a id="methods" class="xliff"></a>
## Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление планов](../api/plannergroup_list_plans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получение коллекции объектов **plannerPlan**.|

<a id="properties" class="xliff"></a>
## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор объекта **plannerGroup**.|

<a id="relationships" class="xliff"></a>
## Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|plans|Коллекция объектов [plannerPlan](plannerplan.md)| Только для чтения. Допускает значение null. Возвращает экземпляры [plannerPlan](plannerplan.md), принадлежащие группе.|

<a id="json-representation" class="xliff"></a>
## Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->