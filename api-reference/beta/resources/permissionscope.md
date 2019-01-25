---
title: Тип ресурса permissionScope
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта Application) при вызове ресурса приложения. Свойство **oauth2Permissions** ServicePrincipal сущности и сущности приложения — это коллекция **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517080"
---
# <a name="permissionscope-resource-type"></a>Тип ресурса permissionScope

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта [Application](application.md) ) при вызове ресурса приложения. Свойство **oauth2Permissions** [ServicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **OAuth2Permission**.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
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
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
