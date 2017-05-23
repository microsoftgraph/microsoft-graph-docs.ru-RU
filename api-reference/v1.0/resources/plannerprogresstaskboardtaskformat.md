# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>Тип ресурса plannerProgressTaskBoardTaskFormat

Ресурс **plannerProgressTaskBoardTaskFormat** представляет информацию, используемую для правильного отображения задачи в представлении "Ход выполнения" на доске задач (представлении с сортировкой по состоянию поля PercentComplete и столбцами "Не начато", "В процессе" и "Выполнено"). С каждым объектом [task](plannertask.md) связан один объект **plannerProgressTaskBoardTaskFormat**.


### <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat_get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |Чтение свойств и отношений объекта **plannerProgressTaskBoardTaskFormat**.|
|[Обновление](../api/plannerprogresstaskboardtaskformat_update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |Обновление объекта **plannerProgressTaskBoardTaskFormat**. |

### <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Идентификатор ресурса. Идентификатор состоит из 28 символов и чувствителен к регистру. [Проверка формата](planner_identifiers_disclaimer.md) выполняется для службы.|
|orderHint|Строка|Указание, используемое для расположения задачи в представлении "Ход выполнения" на доске задач. Используемый формат описан [здесь](planner_order_hint_format.md).|

### <a name="relationships"></a>Отношения
Нет


### <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->