---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ce68460e8dfd0ff3e58b51d0007278aa6c9426e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334245"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>Тип ресурса Едукатионидентитиматчингоптионс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **Тег** | string |  Тип роли пользователя, назначаемый лицензии. Возможные значения: `student`, `teacher`.      |
| **Саурцепропертинаме** | string |  Имя исходного свойства, которое должно быть именем поля в источнике данных. В этом свойстве учитывается регистр.        |
| **Таржетпропертинаме** | string |  Имя целевого свойства, которое должно быть допустимым свойством в Azure AD. В этом свойстве учитывается регистр.     |
| **Таржетдомаин** | string |  Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте. Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством.        |

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
