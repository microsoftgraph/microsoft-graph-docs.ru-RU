---
title: тип ресурсов sectionGroup
description: Группа разделов в OneNote записной книжке. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 575aeb64fbb1f2ffe3df787311704f5fb4f262e6c71808b1d11c901fc2184d0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134954"
---
# <a name="sectiongroup-resource-type"></a>тип ресурсов sectionGroup

Пространство имен: microsoft.graph

Группа разделов в OneNote записной книжке. Группы разделов могут содержать разделы и группы разделов.

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
|createdDateTime|DateTimeOffset|Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|id|String|Уникальный идентификатор группы разделов. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|displayName|String|Имя группы разделов.|
|sectionGroupsUrl|String|URL-адрес `sectionGroups` свойства навигации, который возвращает все группы разделов в группе разделов. Только для чтения.|
|sectionsUrl|String|URL-адрес `sections` свойства навигации, который возвращает все разделы в группе разделов. Только для чтения.|
|self|String|Конечная точка, где можно получить сведения о группе разделов. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Блокнот, содержащий группу разделов. Только для чтения.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Группа разделов, которая содержит группу разделов. Только для чтения.|
|sectionGroups|Коллекция [SectionGroup](sectiongroup.md)|Раздел групп в разделе. Только для чтения. Допускает значение null.|
|sections|Коллекция [OnenoteSection](section.md)|Разделы в группе разделов. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод группы разделов](../api/sectiongroup-get.md) | [SectionGroup](sectiongroup.md) |Ознакомьтесь с свойствами и отношениями группы разделов.|
|[Создание группы разделов](../api/sectiongroup-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Создайте группу разделов, разместив в разделеGroups коллекцию в указанной группе раздела.|
|[Перечисление групп разделов](../api/sectiongroup-list-sectiongroups.md) |Коллекция [SectionGroup](sectiongroup.md)| Получите коллекцию групп разделов в указанной группе раздела.|
|[Создание раздела](../api/sectiongroup-post-sections.md) |[OnenoteSection](section.md)| Создайте раздел, разместив в коллекции разделов в указанной группе разделов.|
|[Перечисление разделов](../api/sectiongroup-list-sections.md) |Коллекция [OnenoteSection](section.md)| Получите коллекцию разделов в указанной группе раздела.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

