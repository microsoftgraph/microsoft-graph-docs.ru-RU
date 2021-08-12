---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для Microsoft Authenticator методов проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5fc1f6dfd2d28e6a0e6e4643b239ed50ba41309dce90448e373f8851040a1478
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249169"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
Пространство имен: microsoft.graph

Коллекция пользователей или групп, с помощью [Microsoft Authenticator методов](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) проверки подлинности в Azure AD.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Объектный ID пользователя или группы Azure AD.|
|authenticationMode|MicrosoftAuthenticatorAuthenticationMode|Определяет, какие типы уведомлений можно использовать для регистрации. Возможные значения: `any` , `deviceBasedPush` (только без паролей), `push` .|
|featureSettings|authenticatorAppFeatureSettings|Определяет, какие дополнительные параметры следует применить к Microsoft Authenticator. Возможные значения: `null` , `requireNumberMatching` (Требуется совпадение номеров для уведомлений MFA. Значение игнорируется для уведомлений о входе в телефон).|
|isRegistrationRequired|Логический|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности. *Не поддерживается.* |
|shownContext|authenticatorAppContextType|(Частный предварительный просмотр) Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления. Возможные значения: `location`, `app`.|
|targetType|authenticationMethodTargetType| Возможные значения: `user`, `group`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "authenticationMode": "String",
  "shownContext": "String",
  "featureSettings": "String"
}
```
