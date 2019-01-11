---
title: Тип ресурса oAuth2Permission
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта application) при вызове ресурса приложения. Свойство **appRoles** servicePrincipal сущности и сущности приложения — это коллекция **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 420a7b181aa2590d3c5bc8eaa7f104251915ae0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829710"
---
# <a name="oauth2permission-resource-type"></a>Тип ресурса oAuth2Permission

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
|adminConsentDescription|Строка|Текст справки разрешение, которое отображается в admin согласия и приложение назначения приемы и способы работы.|
|adminConsentDisplayName|Строка|Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.|
|id|Guid|Идентификатор уникальные области разрешений внутри семейства oauth2Permissions.|
|isEnabled|Логический|При создании или обновлении разрешение, это свойство должно быть присвоено **значение true** (по умолчанию). Чтобы удалить разрешение, это свойство необходимо сначала задать значение **false**.  На этом этапе в последующих вызовов, могут быть удалены разрешения.|
|type|Строка|Указывает, является ли это разрешение области можно consented конечным пользователем или, будет ли это разрешение всей клиента, в котором должен быть consented к администратором компании.  Возможные значения: «Пользователь» или «Администратор».|
|userConsentDescription|Строка|Текст справки разрешение, которое отображается в рабочую среду согласия пользователя.|
|userConsentDisplayName|Строка|Отображаемое имя для разрешения, которое отображается в рабочую среду согласия пользователя.|
|value|Строка|Значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
