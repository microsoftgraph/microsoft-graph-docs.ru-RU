---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для Microsoft Authenticator методов проверки подлинности.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 810403eff5801ebcbafd56cf3de6252fe1f68bf8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067082"
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
|isRegistrationRequired|Boolean|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности. *Не поддерживается.* |
|shownContext|authenticatorAppContextType|(Частный предварительный просмотр) Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления. Возможные значения: `location`, `app`.|
|targetType|authenticationMethodTargetType| Возможные значения: `user`, `group`.|

## <a name="relationships"></a>Отношения
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
