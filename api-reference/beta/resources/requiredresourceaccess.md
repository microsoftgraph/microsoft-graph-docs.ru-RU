---
title: Тип ресурса requiredResourceAccess
description: Задает набор области разрешений OAuth 2.0 и роли приложения в разделе указанного ресурса, доступ к приложению. Указанной области разрешений OAuth 2.0 может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** ) при вызове ресурса приложения. Свойство **requiredResourceAccess** объекта приложения — это коллекция **ReqiredResourceAccess**.
ms.openlocfilehash: 937557f2f078ade1b336cfd00cd128d428d59cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080857"
---
# <a name="requiredresourceaccess-resource-type"></a>Тип ресурса requiredResourceAccess

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Задает набор области разрешений OAuth 2.0 и роли приложения в разделе указанного ресурса, доступ к приложению. Указанной области разрешений OAuth 2.0 может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** ) при вызове ресурса приложения. Свойство **requiredResourceAccess** объекта [приложения](application.md) — это коллекция **ReqiredResourceAccess**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|resourceAccess|[ResourceAccess](resourceaccess.md) коллекции|Список области разрешений OAuth2.0 и роли приложения, необходимых приложению из указанного ресурса.|
|resourceAppId|String|Уникальный идентификатор для ресурса, доступ к приложению.  Это должен быть равен **appId** , объявлен ресурсов для конечного приложения.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
