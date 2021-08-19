---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для Microsoft Authenticator методов проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4baf2713789a54707c65fe8c2b94fe60ac275626
ms.sourcegitcommit: b7e01a1331abe5f5c9aa2828d93dad08229573f1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58336672"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, с помощью [Microsoft Authenticator методов](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) проверки подлинности в Azure AD.  Наследует от [проверки подлинностиMethodTarget](authenticationMethodTarget.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authenticationMode|MicrosoftAuthenticatorAuthenticationMode|Определяет, какие типы уведомлений можно использовать для регистрации. Возможные значения: `deviceBasedPush` (только без паролей) `push` и `any` .|
|featureSettings|authenticatorAppFeatureSettings|Определяет, какие дополнительные параметры следует применить к Microsoft Authenticator. Возможные значения: `requireNumberMatching` (Требуется совпадение номеров для уведомлений MFA. Значение игнорируется для уведомлений о входе в телефон). Допускает значение null.|
|id|Строка|Идентификатор объекта пользователя или группы Azure AD. Унаследованный от [проверки подлинностиMethodTarget](authenticationmethodtarget.md).|
|isRegistrationRequired|Логический|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности. Унаследованный от [проверки подлинностиMethodTarget](authenticationmethodtarget.md). *Не поддерживается.* |
|targetType|authenticationMethodTargetType| Возможные значения: `user`, `group` и `unknownFutureValue`. Унаследованный от [проверки подлинностиMethodTarget](authenticationMethodTarget.md).|
<!--
|numberMatchingRequiredState|advancedConfigState|Requires number matching for MFA notifications. Value is ignored for phone sign-in notifications. Possible values are: `enabled`, `disabled`, `default`.|
|displayLocationInformationRequiredState|advancedConfigState|Determines whether the location of the sign-in should be shown to the user in the body of the notification. Possible values are: `enabled`, `disabled`, `default`.|
|displayAppInformationRequiredState|advancedConfigState|Determines whether the app the user is signing into should be shown to the user in the body of the notification. Possible values are: `enabled`, `disabled`, `default`.|
-->

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
  "featureSettings": "String"
}

```
