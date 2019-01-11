---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
ms.openlocfilehash: f204c5422eb5f0f2580bfbed82ed28306dd0618f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806309"
---
# <a name="sectiongroup-resource-type"></a>Тип ресурса sectionGroup

Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectionGroup"
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
| Свойство     | Тип   |Описание|
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

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Записная книжка, содержащая группу разделов. Только для чтения.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Группа разделов, содержащая группу разделов. Только для чтения.|
|sectionGroups|Коллекция объектов [SectionGroup](sectiongroup.md)|Группы разделов в разделе. Только для чтения. Допускает значение null.|
|sections|[OnenoteSection](section.md) коллекции|Разделы в группе разделов. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение группы разделов](../api/sectiongroup-get.md) | [SectionGroup](sectiongroup.md) |Чтение свойств и отношений группы разделов.|
|[Создание группы разделов](../api/sectiongroup-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.|
|[Перечисление групп разделов](../api/sectiongroup-list-sectiongroups.md) |Коллекция объектов [SectionGroup](sectiongroup.md)| Получение коллекции групп разделов в указанной группе разделов.|
|[Создание раздела](../api/sectiongroup-post-sections.md) |[OnenoteSection](section.md)| Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.|
|[Перечисление разделов](../api/sectiongroup-list-sections.md) |[OnenoteSection](section.md) коллекции| Получение коллекции разделов в указанной группе разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
