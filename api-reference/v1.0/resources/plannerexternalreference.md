---
title: тип ресурса plannerExternalReference
description: Ресурс **plannerExternalReference представляет** метаданные ссылки (вложения, такие как файл, URL-адрес). Это значение пар значения свойства в объекте externalReferences.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 225a4fb53875629eab093586193bf569d31693c4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019274"
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
|previewPriority|Строка|Используется для задания порядка относительного приоритета, в котором ссылка будет показана в качестве предварительного просмотра задачи.|
|type|Строка|Используется для описания типа ссылки. Типы включают: `PowerPoint` `Word` , , , `Excel` `Other` .|

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

