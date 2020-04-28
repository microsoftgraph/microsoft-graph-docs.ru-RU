---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d722beaac54cbd57c227457a0883b856f6eca4bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501831"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>Тип ресурса Едукатионидентитиматчингоптионс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Тег** | string |  Тип роли пользователя, назначаемый лицензии. Возможные значения: `student`, `teacher`, `faculty`.      |
| **саурцепропертинаме** | string |  Имя исходного свойства, которое должно быть именем поля в источнике данных. В этом свойстве учитывается регистр.        |
| **таржетпропертинаме** | string |  Имя целевого свойства, которое должно быть допустимым свойством в Azure AD. В этом свойстве учитывается регистр.     |
| **таржетдомаин** | string |  Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте. Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.        |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
