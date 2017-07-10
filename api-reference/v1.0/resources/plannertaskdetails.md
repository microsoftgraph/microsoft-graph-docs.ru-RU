<a id="plannertaskdetails-resource-type" class="xliff"></a>
# Тип ресурса plannerTaskDetails

Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. С каждым объектом [task](plannertask.md) связан объект details.


<a id="methods" class="xliff"></a>
## Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerTaskDetails](../api/plannertaskdetails_get.md) | [plannerTaskDetails](plannertaskdetails.md) |Чтение свойств и отношений объекта **plannerTaskDetails**.|
|[Обновление](../api/plannertaskdetails_update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Обновление объекта **plannerTaskDetails**. |


<a id="properties" class="xliff"></a>
## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|Коллекция элементов контрольного списка задачи.|
|description|Строка|Описание задачи.|
|id|String| Только для чтения. Идентификатор сведений о задаче. Идентификатор состоит из 28 символов и чувствителен к регистру. [Проверка формата](planner_identifiers_disclaimer.md) выполняется для службы.|
|previewType|string|Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.|
|references|[plannerExternalReferences](plannerexternalreferences.md)|Коллекция ссылок на задачу.|

<a id="relationships" class="xliff"></a>
## Отношения
Нет


<a id="json-representation" class="xliff"></a>
## Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->