---
title: Тип ресурса educationLinkResource
description: Подкласс educationResource.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1dbf39593f4e76aadd714b9a8989e25944f1c2d0
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684482"
---
# <a name="educationlinkresource-resource-type"></a>Тип ресурса educationLinkResource

Пространство имен: microsoft.graph

Подкласс [educationResource](educationresource.md). 

Этот ресурс является ссылкой и не содержит дополнительных данных, связанных с ним.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ссылка|String|URL-адрес ресурса.|
|createdBy|String|Отображаемое имя пользователя, создавшего этот объект.|
|createdDateTime|DateTimeOffset|Дата, когда была добавлена повторная ошибка.|
|displayName|string|Отображаемое имя ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменяет ресурс.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения ресурса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String",
  "createdBy": "String (User)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": "String (User)",
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


