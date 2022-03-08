---
title: Тип ресурса appIdentity
description: Указывает удостоверение приложения, которое выполнило действие или было изменено. Включает id приложения, имя, главный ИД службы и имя. Этот ресурс называется API directoryAudit
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: sureshja
ms.openlocfilehash: 66a830d5a030a6b3247e3265aaeaa66452a7c577
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336930"
---
# <a name="appidentity-resource-type"></a>Тип ресурса appIdentity

Пространство имен: microsoft.graph

Указывает удостоверение приложения, которое выполнило действие или было изменено. Этот ресурс называется API [directoryAudit](../api/directoryaudit-get.md) .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|appId|String|Ссылается на уникальный идентификатор, представляющий идентификатор приложения в Azure Active Directory.|
|displayName|String|Ссылается на имя приложения, отображаемую на портале Azure.|
|servicePrincipalId|String|Ссылается на уникальный идентификатор, указывающий идентификатор директора службы в Azure Active Directory для соответствующего приложения.|
|servicePrincipalName|String|Ссылается на имя главного клиента службы — имя приложения в клиенте. |

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


