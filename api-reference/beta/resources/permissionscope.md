---
title: Тип ресурса permissionScope
description: Представляет определение делегирования разрешения, иногда именуемого разрешением OAuth 2.0 или областью OAuth 2.0. После определения делегированная разрешения может запрашиваться клиентской заявкой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0d5d09599108b7753ee60012337e393c6bc79905
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638860"
---
# <a name="permissionscope-resource-type"></a>Тип ресурса permissionScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определение [делегирования разрешения.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)

Делегировать разрешения могут клиентские приложения, которым требуется маркер доступа к API, определяющий разрешения. Делегирование разрешений можно [](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)запрашивать динамически, используя параметр в запросе на авторизацию платформы удостоверений Майкрософт, или статически, через коллекцию `scopes` **requiredResourceAccess на** объекте приложения. [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope) [](application.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|adminConsentDescription|String|Описание делегирования разрешений, которые должен прочитать администратор, дающий разрешение от имени всех пользователей. Этот текст отображается в интерфейсе согласия администратора для всего клиента.|
|adminConsentDisplayName|String|Название разрешения, предназначенное для чтения администратором, дающим разрешение от имени всех пользователей.|
|id|GUID|Уникальный идентификатор делегирования разрешений внутри коллекции делегированных разрешений, определенных для приложения-ресурса.|
|isEnabled|Boolean|При создании или обновлении разрешения это свойство должно быть заданной значение **true** (по умолчанию). Чтобы удалить разрешение, это свойство сначала должно быть настроено **как** false .  В этот момент при последующем вызове разрешение может быть удалено.|
|type|String|Указывает, следует ли считать это делегированное разрешение безопасным для неадминистрирования пользователей, чтобы дать согласие от имени самих себя, или необходимо ли администратору для согласия на разрешения. Это будет поведение по умолчанию, но каждый клиент может настроить поведение в своей организации (разрешив, ограничив или ограничив согласие пользователя этим делегированным разрешением.)|
|userConsentDescription|String|Описание делегирования разрешений, предназначенных для чтения пользователем, выдающим разрешение от своего имени. Этот текст отображается в случаях согласия, когда пользователь соглашается только от имени себя.|
|userConsentDisplayName|String|Название разрешения, предназначенное для чтения пользователем, выдающим разрешение от своего имени. Этот текст отображается в случаях согласия, когда пользователь соглашается только от имени себя.|
|value|String|Указывает значение, необходимое для включаемого `scp` в (область) утверждения в маркерах доступа. Длина не должна превышать 120 символов. Разрешены `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` символы, а также символы в диапазонах `0-9` и `A-Z` `a-z` . Любой другой символ, включая символ пространства, не допускается. Может не `.` начинаться с .|

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
  "id": "guid",
  "adminConsentDisplayName": "string",
  "adminConsentDescription": "string",
  "userConsentDisplayName": "string",
  "userConsentDescription": "string",
  "value": "string",
  "type": "string",
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
