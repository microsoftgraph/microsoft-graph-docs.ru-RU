---
title: Тип ресурса permissionScope
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта Application) при вызове ресурса приложения. Свойство **oauth2Permissions** ServicePrincipal сущности и сущности приложения — это коллекция **OAuth2Permission**.
ms.openlocfilehash: b15ee9901632fca113d944000847c953e85be58c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080309"
---
# <a name="permissionscope-resource-type"></a>Тип ресурса permissionScope

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта [Application](application.md) ) при вызове ресурса приложения. Свойство **oauth2Permissions** [ServicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **OAuth2Permission**.

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:---------------|:--------|:----------|
|adminConsentDescription|String| Текст справки разрешение, которое отображается в admin согласия и приложение назначения приемы и способы работы. |
|adminConsentDisplayName|String| Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы. |
|id|Guid| Идентификатор уникальные области разрешений внутри семейства oauth2Permissions. |
|isEnabled|Логический| При создании или обновлении разрешение, это свойство должно быть присвоено **значение true** (по умолчанию). Чтобы удалить разрешение, это свойство необходимо сначала задать значение **false**. На этом этапе в последующих вызовов, могут быть удалены разрешения. |
|Происхождение|String| Для внутреннего использования. |
|type|String| Указывает, является ли это разрешение области можно consented конечным пользователем или, будет ли это разрешение всей клиента, в котором должен быть consented для администратором компании. Возможные значения: *пользователь* или *администратор*. |
|userConsentDescription|String| Текст справки разрешение, которое отображается в разрешения для конечных пользователей. |
|userConsentDisplayName|String| Отображаемое имя для разрешения, которое отображается в разрешения для конечных пользователей. |
|value|String| Значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->