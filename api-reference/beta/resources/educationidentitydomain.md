---
title: Тип ресурса Едукатионидентитидомаин
description: 'Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a21d4d3005be8a776ae8bb9f9e3c1027be48de72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501929"
---
# <a name="educationidentitydomain-resource-type"></a>Тип ресурса Едукатионидентитидомаин

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сопоставление между типом пользователя "образование" и доменом, к которому принадлежит учетная запись пользователя. Ресурс Domain является частью [конфигурации создания удостоверений](educationidentitycreationconfiguration.md). 

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Тег** | string |  Тип роли пользователя, назначаемый лицензии. Возможные значения: `student`, `teacher`, `faculty`.      |
| **name** | string |  Представляет домен для учетной записи пользователя.         |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
