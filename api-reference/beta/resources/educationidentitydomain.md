---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4e23a9111d2515234d1aa665f4847d732dc563
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435042"
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
