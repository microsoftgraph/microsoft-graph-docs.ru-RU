---
title: Тип ресурса Едукатионидентитиматчингоптионс
description: Обеспечивает сопоставление между свойством Source и целевым свойством для сопоставления учетных записей пользователей. Исходное свойство должно существовать в исходных данных. Свойство Target должно быть допустимым свойством в Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b17ca8548d7a70b8f652ad2d54455fb6040677d
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435028"
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
