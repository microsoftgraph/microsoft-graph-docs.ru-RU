---
title: Тип ресурса permissionScope
description: Представляет определение делегирования разрешения, иногда именуемого разрешением OAuth 2.0 или областью OAuth 2.0. После определения делегированная разрешения может запрашиваться клиентской заявкой.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: e06af959ffa280256489912e3e3df3dd2490cf74
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335222"
---
# <a name="permissionscope-resource-type"></a>Тип ресурса permissionScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определение [делегирования разрешения](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).

Делегировать разрешения могут клиентские приложения, которым требуется маркер доступа к API, определяющий разрешения. Делегирование разрешений можно запрашивать [динамически,](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)`scopes` используя параметр в запросе на авторизацию в платформа удостоверений Майкрософт или статически [через](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope) коллекцию **requiredResourceAccess на** объекте [приложения.](application.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|adminConsentDescription|Строка|Описание делегирования разрешений, которые должен прочитать администратор, дающий разрешение от имени всех пользователей. Этот текст отображается в интерфейсе согласия администратора для всего клиента.|
|adminConsentDisplayName|String|Название разрешения, предназначенное для чтения администратором, дающим разрешение от имени всех пользователей.|
|id|GUID|Уникальный идентификатор делегирования разрешений внутри коллекции делегированных разрешений, определенных для приложения-ресурса.|
|isEnabled|Boolean|При создании или обновлении разрешения это свойство должно быть заданной значение **true** (по умолчанию). Чтобы удалить разрешение, это свойство сначала должно быть настроено как **ложное**.  В этот момент при последующем вызове разрешение может быть удалено.|
|type|String| Возможные значения: `User` и `Admin`. Указывает, следует ли считать это делегированное разрешение безопасным для неадминистрных пользователей, чтобы дать согласие от имени самих себя, или требуется ли всегда согласие администратора. Хотя microsoft Graph для каждого разрешения определяет требование о согласии по умолчанию, администратор клиента может переопределять поведение в организации (разрешив, ограничив или ограничив согласие пользователя этим делегированным разрешением). Дополнительные сведения см. в [приложении Configure how users consent to applications](/azure/active-directory/manage-apps/configure-user-consent). |
|userConsentDescription|Строка|Описание делегирования разрешений, предназначенных для чтения пользователем, выдающим разрешение от своего имени. Этот текст отображается в случаях согласия, когда пользователь соглашается только от имени себя.|
|userConsentDisplayName|Строка|Название разрешения, предназначенное для чтения пользователем, выдающим разрешение от своего имени. Этот текст отображается в случаях согласия, когда пользователь соглашается только от имени себя.|
|value|String|Указывает значение, необходимое для включаемого `scp` в (область) утверждения в маркерах доступа. Длина не должна превышать 120 символов. Разрешены символы `:` <code>&#96;</code> `]` `@` `^` `'` `&` `(` `%` `$` `#` `!` <code>&gt;</code> `?` `[` `;` `~`<code>&lt;</code> `}` `+` `*` `,` `-` `.` `)` `/` `_` <code>&#124;</code> `=` `{` `:` `+`, а также символы в диапазонах `0-9`и .`a-z``A-Z` Любой другой символ, включая символ пространства, не допускается. Может не начинаться с `.`.|

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
  "id": "Guid",
  "adminConsentDisplayName": "String",
  "adminConsentDescription": "String",
  "userConsentDisplayName": "String",
  "userConsentDescription": "String",
  "value": "String",
  "type": "String",
  "isEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
