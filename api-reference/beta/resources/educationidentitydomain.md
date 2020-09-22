---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b25f935ae404a243826a14c310a17ad80c598380
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095393"
---
# <a name="educationidentitydomain-resource-type"></a>Тип ресурса Едукатионидентитидомаин

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md).

## <a name="properties"></a>Свойства

| Свойство  | Тип   | Описание                                                                                        |
| :-------- | :----- | :------------------------------------------------------------------------------------------------- |
| Тег | String | Тип роли пользователя, назначаемый лицензии. Возможные значения: `student`, `teacher`, `faculty`. |
| name      | String | Представляет домен для учетной записи пользователя.                                                        |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "name": "String"
}
```


