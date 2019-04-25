---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ec27343121ba20ef65703f3df1d53e6c62ccc8e4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579144"
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
|id|String|Уникальный идентификатор группы разделов. Только для чтения.|
|lastModifiedBy|[identitySet](identityset.md)|Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|displayName|String|Имя группы разделов.|
|Сектионграупсурл|String|URL-адрес для `sectionGroups` свойства навигации, который возвращает все группы разделов в группе разделов. Только для чтения.|
|Сектионсурл|String|URL-адрес для `sections` свойства навигации, который возвращает все разделы в группе разделов. Только для чтения.|
|Self|String|Конечная точка, где можно получить сведения о группе разделов. Только для чтения.|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|Записная книжка, содержащая группу разделов. Только для чтения.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|Группа разделов, содержащая группу разделов. Только для чтения.|
|sectionGroups|Коллекция [sectionGroup](sectiongroup.md)|Группы разделов в разделе. Только для чтения. Допускается значение null.|
|sections|Коллекция [оненотесектион](section.md)|Разделы в группе разделов. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод группы разделов](../api/sectiongroup-get.md) | [SectionGroup](sectiongroup.md) |Прочитайте свойства и связи группы разделов.|
|[Создание группы разделов](../api/sectiongroup-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Создание группы разделов путем отправки в коллекцию sectionGroups в указанной группе разделов.|
|[Список групп разделов](../api/sectiongroup-list-sectiongroups.md) |Коллекция [sectionGroup](sectiongroup.md)| Получение коллекции групп разделов в указанной группе разделов.|
|[Создание раздела](../api/sectiongroup-post-sections.md) |[Оненотесектион](section.md)| Создание раздела путем публикации в коллекции разделов в указанной группе разделов.|
|[Вывод списка разделов](../api/sectiongroup-list-sections.md) |Коллекция [оненотесектион](section.md)| Получение коллекции разделов в указанной группе разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
