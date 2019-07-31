---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 091bb8e6c1a14f6c173d18acf68679feb6c88eaf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964231"
---
# <a name="verifieddomain-resource-type"></a>Тип ресурса verifiedDomain

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|capabilities|String|Примеры: “Email”, “OfficeCommunicationsOnline”.|
|isDefault|Boolean|                Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.            |
|при инициализации|Boolean|Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.|
|name|String|Доменное имя, например "contoso.onmicrosoft.com"|
|type|String|Пример: "Managed".|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
