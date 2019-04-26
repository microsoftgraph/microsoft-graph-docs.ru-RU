---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1cd9757b0a58afb4183bd917a7a090b14502a36
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343403"
---
# <a name="sectiongroup-resource-type"></a>Тип ресурса sectionGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "keyProperty": "id",
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
|parentNotebook|[записной книжки](notebook.md)|Записная книжка, содержащая группу разделов. Только для чтения.|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|Группа разделов, содержащая группу разделов. Только для чтения.|
|sectionGroups|Коллекция [sectionGroup](sectiongroup.md)|Группы разделов в разделе. Только для чтения. Допускает значение null.|
|sections|Коллекция [оненотесектион](onenotesection.md)|Разделы в группе разделов. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод группы разделов](../api/sectiongroup-get.md) | [sectionGroup](sectiongroup.md) |Прочитайте свойства и связи группы разделов.|
|[Создание группы разделов](../api/sectiongroup-post-sectiongroups.md) |[sectionGroup](sectiongroup.md)| Создание группы разделов путем отправки в коллекцию sectionGroups в указанной группе разделов.|
|[Перечисление групп разделов](../api/sectiongroup-list-sectiongroups.md) |Коллекция [sectionGroup](sectiongroup.md)| Получение коллекции групп разделов в указанной группе разделов.|
|[Создание раздела](../api/sectiongroup-post-sections.md) |[Оненотесектион](onenotesection.md)| Создание раздела путем публикации в коллекции разделов в указанной группе разделов.|
|[Перечисление разделов](../api/sectiongroup-list-sections.md) |Коллекция [оненотесектион](onenotesection.md)| Получение коллекции разделов в указанной группе разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
