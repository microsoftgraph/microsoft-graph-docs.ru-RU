---
title: тип ресурса plannerExternalReference
description: Ресурс **plannerExternalReference представляет** метаданные ссылки (вложения, такие как файл, URL-адрес). Это значение пар значения свойства в объекте externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: cb856a9d147874428ab7e4d3e4169eba8bf1c028a80df4d0b6a459dc8bd1f430
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251873"
---
# <a name="plannerexternalreference-resource-type"></a>тип ресурса plannerExternalReference

Пространство имен: microsoft.graph

Ресурс **plannerExternalReference представляет** метаданные ссылки (вложения, такие как файл, URL-адрес). Это значение пар свойств-значений в [объекте externalReferences.](plannerexternalreferences.md)



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|alias|String|Псевдоним имени для описания ссылки.|
|lastModifiedBy|[identitySet](identityset.md)|Только для чтения. Пользовательский ID, с помощью которого он был изменен в последний раз.|
|lastModifiedDateTime|DateTimeOffset|Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|previewPriority|String|Используется для задания порядка относительного приоритета, в котором ссылка будет показана в качестве предварительного просмотра задачи.|
|type|String|Используется для описания типа ссылки. Типы включают: `PowerPoint` `Word` , , , `Excel` `Other` .|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

