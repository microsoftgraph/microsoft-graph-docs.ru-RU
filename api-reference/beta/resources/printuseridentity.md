---
title: Тип ресурса Принтусеридентити
description: Представляет удостоверение пользователя в универсальной службе печати. Сопоставление с пользователем Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2899b3ca75660280b797dda62993789f634096
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917618"
---
# <a name="printuseridentity-resource-type"></a>Тип ресурса Принтусеридентити

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение пользователя в универсальной службе печати. Сопоставляется с [пользователем Azure Active Directory (Azure AD)](user.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор Принтусеридентити. Только для чтения.|
|displayName|Строка|Отображаемое имя Принтусеридентити.|
|ipAddress|String|IP-адрес Принтусеридентити. Не заполнено.|
|userPrincipalName|String|Имя участника-пользователя Принтусеридентити (UPN).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUserIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUserIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
