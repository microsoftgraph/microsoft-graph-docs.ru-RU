---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для Microsoft Authenticator методов проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db534dfb13e288b82b49005b2b1a923b8bfd5112
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896643"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, с помощью [Microsoft Authenticator методов](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) проверки подлинности в Azure AD.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Объектный ID пользователя или группы Azure AD.|
|authenticationMode|MicrosoftAuthenticatorAuthenticationMode|Определяет, какие типы уведомлений можно использовать для регистрации. Возможные значения: `any` , `deviceBasedPush` (только без паролей), `push` .|
|isRegistrationRequired|Boolean|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности. *Не поддерживается.* |
|numberMatchingRequiredState|advancedConfigState|Требуется совпадение номеров для уведомлений MFA. Значение игнорируется для уведомлений о входе в телефон. Возможные значения: `enabled`, `disabled`, `default`.|
|displayLocationInformationRequiredState|advancedConfigState|Определяет, следует ли показывать пользователю расположение входной записи в теле уведомления. Возможные значения: `enabled`, `disabled`, `default`.|
|displayAppInformationRequiredState|advancedConfigState|Определяет, следует ли показывать пользователю приложение, в которое подписывает пользователь, в теле уведомления. Возможные значения: `enabled`, `disabled`, `default`.|
|targetType|authenticationMethodTargetType| Возможные значения: `null`, `user`, `group`.|

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
  "numberMatchingRequiredState": "String",
  "displayLocationInformationRequiredState": "String",
  "displayAppInformationRequiredState": "String"
}

```
