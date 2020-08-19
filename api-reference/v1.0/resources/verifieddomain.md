---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 656e4a4c8fc40c86eea3b3e167adae22a9580081
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807698"
---
# <a name="verifieddomain-resource-type"></a>Тип ресурса verifiedDomain

Пространство имен: microsoft.graph

Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|capabilities|String|Примеры: “Email”, “OfficeCommunicationsOnline”.|
|isDefault|Boolean|                Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.            |
|при инициализации|Boolean|Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.|
|name|String|Доменное имя, например "contoso.onmicrosoft.com"|
|type|String|Пример: "Managed".|

## <a name="json-representation"></a>Представление в формате JSON

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
