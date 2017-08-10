# <a name="groupsettingtemplate-resource-type"></a>Тип ресурса groupSettingTemplate

Шаблоны параметров группы представляют определенные системой параметры для клиента. Можно на базе доступных объектов **groupSettingTemplate** создавать [параметры группы](groupsetting.md), а также менять предопределенные значения по умолчанию этих параметров. Шаблоны параметров группы невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или отдельной группы. На данный момент доступны только шаблоны, применимые к группам Office 365 и включающие параметры, которые, например, разрешают или запрещают пользователям создавать группы либо приглашать внешних гостей в группу.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Получение groupSettingTemplate](../api/groupsettingtemplate_get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Считывание конкретных свойств одного из определенных системой объектов groupSettingTemplate. |
|[Перечисление groupSettingTemplate](../api/groupsettingtemplate_list.md) | [Коллекция объектов groupSettingTemplate](groupsettingtemplate.md) |Перечисление всех определенных системой объектов groupSettingTemplate.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание шаблона. |
|displayName|String| Отображаемое имя шаблона. |
|id|String| Уникальный идентификатор шаблона. Только для чтения.|
|values|Коллекция объектов [settingTemplateValue](settingtemplatevalue.md)| Коллекция объектов settingTemplateValue, перечисляющих набор доступных параметров, значений по умолчанию и типов, которые составляют шаблон. |

## <a name="relationships"></a>Отношения

Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->