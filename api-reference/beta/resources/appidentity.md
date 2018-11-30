---
title: Тип ресурса appIdentity
description: Указывает идентификатор приложения, выполнившего действия или была изменена. Включает в себя код приложения, имя, идентификатор участника-службы и имя. Этот ресурс вызывается directoryAudit API
ms.openlocfilehash: 6fcbe8dbb1e17139111c5f1fa9e8681cd1b996a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078630"
---
# <a name="appidentity-resource-type"></a>Тип ресурса appIdentity
Указывает идентификатор приложения, выполнившего действия или была изменена. Включает в себя код приложения, имя, идентификатор участника-службы и имя. Этот ресурс вызывается [directoryAudit](../api/directoryaudit-get.md) API


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|appId|String|Указывает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|displayName|String|Ссылается на имя приложения, отображаемые на портале Azure.|
|servicePrincipalId|String|Указывает уникальный идентификатор GUID, указывающее идентификатор участника-службы в Azure Active Directory для соответствующего приложения.|
|servicePrincipalName|String|Ссылается на имя участника-службы — это имя приложения в клиентов. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->