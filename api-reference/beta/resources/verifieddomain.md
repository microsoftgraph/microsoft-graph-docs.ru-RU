---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство verifiedDomains сущности организации представляет собой коллекцию объектов verifiedDomain.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: e792f30cf77d5199d27cae8d7ca7e6dbc6fc37da
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247037"
---
# <a name="verifieddomain-resource-type"></a>Тип ресурса verifiedDomain

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает домен клиента. Свойство **verifiedDomains** сущности организации представляет [](organization.md) собой коллекцию объектов **verifiedDomain**.


## <a name="properties"></a>Свойства
| Свойство     | Тип    | Описание                                                                          |
|:-------------|:--------|:-------------------------------------------------------------------------------------|
| capabilities | String  | Например: `Email`, `OfficeCommunicationsOnline`.                                  |
| isDefault    | Boolean | `true`Значение , если это домен по умолчанию, связанный с клиентом; в противном случае . `false` |
| isInitial    | Boolean | `true`Значение , если это исходный домен, связанный с клиентом; в противном случае . `false` |
| name         | String  | Доменное имя; Например, `contoso.onmicrosoft.com`.                             |
| type         | String  | Например, `Managed`.                                                              |

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
  "capabilities": "String",
  "isDefault": true,
  "isInitial": true,
  "name": "String",
  "type": "String"
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


