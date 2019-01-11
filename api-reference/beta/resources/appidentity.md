---
title: Тип ресурса appIdentity
description: Указывает идентификатор приложения, выполнившего действия или была изменена. Включает в себя код приложения, имя, идентификатор участника-службы и имя. Этот ресурс вызывается directoryAudit API
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855785"
---
# <a name="appidentity-resource-type"></a>Тип ресурса appIdentity
Указывает идентификатор приложения, выполнившего действия или была изменена. Включает в себя код приложения, имя, идентификатор участника-службы и имя. Этот ресурс вызывается [directoryAudit](../api/directoryaudit-get.md) API


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appId|String|Указывает уникальный идентификатор GUID, представляющий идентификатор приложения в Azure Active Directory.|
|displayName|Строка|Ссылается на имя приложения, отображаемые на портале Azure.|
|servicePrincipalId|Строка|Указывает уникальный идентификатор GUID, указывающее идентификатор участника-службы в Azure Active Directory для соответствующего приложения.|
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
