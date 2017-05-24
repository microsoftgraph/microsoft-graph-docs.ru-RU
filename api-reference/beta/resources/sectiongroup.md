# <a name="sectiongroup-resource-type"></a>Тип ресурса sectionGroup

Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|createdDateTime|DateTimeOffset|Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|id|Строка|Уникальный идентификатор группы разделов. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.| 
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|displayName|Строка|Имя группы разделов.|
|sectionGroupsUrl|Строка|URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в группе разделов. Только для чтения.| 
|sectionsUrl|Строка|URL-адрес для свойства навигации `sections`, который возвращает все разделы в группе разделов. Только для чтения.|
|self|Строка|Конечная точка, в которой можно получить сведения о группе разделов. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Записная книжка, содержащая группу разделов. Только для чтения.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Группа разделов, содержащая группу разделов. Только для чтения.|
|sectionGroups|Коллекция объектов [SectionGroup](sectiongroup.md)|Группы разделов в разделе. Только для чтения. Допускает значение null.|
|sections|Коллекция объектов [Section](section.md)|Разделы в группе разделов. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение группы разделов](../api/sectiongroup_get.md) | [SectionGroup](sectiongroup.md) |Чтение свойств и отношений группы разделов.|
|[Создание группы разделов](../api/sectiongroup_post_sectiongroups.md) |[SectionGroup](sectiongroup.md)| Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.|
|[Перечисление групп разделов](../api/sectiongroup_list_sectiongroups.md) |Коллекция объектов [SectionGroup](sectiongroup.md)| Получение коллекции групп разделов в указанной группе разделов.|
|[Создание раздела](../api/sectiongroup_post_sections.md) |[Section](section.md)| Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.|
|[Перечисление разделов](../api/sectiongroup_list_sections.md) |Коллекция объектов [Section](section.md)| Получение коллекции разделов в указанной группе разделов.|


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
