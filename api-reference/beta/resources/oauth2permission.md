---
title: Тип ресурса oAuth2Permission
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта application) при вызове ресурса приложения. Свойство **appRoles** servicePrincipal сущности и сущности приложения — это коллекция **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510815"
---
# <a name="oauth2permission-resource-type"></a>Тип ресурса oAuth2Permission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта [application](application.md) ) при вызове ресурса приложения. Свойство **appRoles** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **oAuth2Permission**.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|adminConsentDescription|String|Текст справки разрешение, которое отображается в admin согласия и приложение назначения приемы и способы работы.|
|adminConsentDisplayName|String|Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.|
|id|Guid|Идентификатор уникальные области разрешений внутри семейства oauth2Permissions.|
|isEnabled|Логический|При создании или обновлении разрешение, это свойство должно быть присвоено **значение true** (по умолчанию). Чтобы удалить разрешение, это свойство необходимо сначала задать значение **false**.  На этом этапе в последующих вызовов, могут быть удалены разрешения.|
|type|String|Указывает, является ли это разрешение области можно consented конечным пользователем или, будет ли это разрешение всей клиента, в котором должен быть consented к администратором компании.  Возможные значения: «Пользователь» или «Администратор».|
|userConsentDescription|String|Текст справки разрешение, которое отображается в рабочую среду согласия пользователя.|
|userConsentDisplayName|String|Отображаемое имя для разрешения, которое отображается в рабочую среду согласия пользователя.|
|value|String|Значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
