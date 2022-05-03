---
title: Тип ресурса printUserIdentity
description: Представляет удостоверение пользователя в службе универсальной печати. Карты к Azure AD пользователя.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 50a73a6f08448d50ac616e82d15c046d52d63b83
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176305"
---
# <a name="printuseridentity-resource-type"></a>Тип ресурса printUserIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение пользователя в службе универсальной печати. Карты пользователю Azure Active Directory [(Azure AD).](user.md)

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор printUserIdentity. Только для чтения.|
|displayName|Строка|Отображаемое имя printUserIdentity.|
|ipAddress|String|IP-адрес printUserIdentity. Не заполнено.|
|userPrincipalName|String|Имя участника-пользователя (UPN) printUserIdentity.|

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


