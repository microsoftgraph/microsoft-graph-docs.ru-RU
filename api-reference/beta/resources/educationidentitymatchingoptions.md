---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 73c97b0e9c23c455b3e15ed656060eca7f8a3e4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095382"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>Тип ресурса Едукатионидентитиматчингоптионс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).

## <a name="properties"></a>Свойства

| Свойство           | Тип   | Описание                                                                                                                                                    |
| :----------------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Тег          | String | Тип роли пользователя, назначаемый лицензии. Возможные значения: `student`, `teacher`, `faculty`.                                                             |
| саурцепропертинаме | Строка | Имя исходного свойства, которое должно быть именем поля в источнике данных. В этом свойстве учитывается регистр.                                             |
| таржетпропертинаме | Строка | Имя целевого свойства, которое должно быть допустимым свойством в Azure AD. В этом свойстве учитывается регистр.                                                |
| таржетдомаин       | Строка | Домен в суффикс с исходным свойством, который необходимо найти в целевом объекте. Если задано значение null, свойство Source будет использоваться для сравнения с целевым свойством. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "sourcePropertyName": "String",
  "targetPropertyName": "String",
  "targetDomain": "String"
}
```


