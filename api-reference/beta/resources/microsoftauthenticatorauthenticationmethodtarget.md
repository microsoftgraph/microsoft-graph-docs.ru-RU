---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для Microsoft Authenticator методов проверки подлинности.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8276f01bca86025c11eddeef21d5cce28263c379
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493482"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, с помощью [Microsoft Authenticator методов](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) проверки подлинности в Azure AD.  Наследует от [проверки подлинностиMethodTarget](authenticationMethodTarget.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authenticationMode|MicrosoftAuthenticatorAuthenticationMode|Определяет, какие типы уведомлений можно использовать для регистрации. Возможные значения: `deviceBasedPush` (только без паролей) `push` и `any` .|
|id|String|Идентификатор объекта пользователя или группы Azure AD. Унаследованный от [проверки подлинностиMethodTarget](authenticationmethodtarget.md).|
|isRegistrationRequired|Логический|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности. Унаследованный от [проверки подлинностиMethodTarget](authenticationmethodtarget.md). *Не поддерживается.* |
|targetType|authenticationMethodTargetType| Возможные значения: `user`, `group` и `unknownFutureValue`. Унаследованный от [проверки подлинностиMethodTarget](authenticationMethodTarget.md).|
|numberMatchingRequiredState|advancedConfigState|Требуется совпадение номеров для уведомлений MFA. Значение игнорируется для уведомлений о входе в телефон. Возможные значения: `enabled`, `disabled`, `default`.|
|displayAppInformationRequiredState|advancedConfigState|Определяет, отображается ли пользователю дополнительный контекст в уведомлении Authenticator приложения. В теле уведомления Authenticator пользователю будет показано приложение, в которое они подписываются, а также место, из которое исходил запрос на проверку подлинности. Возможные значения: `enabled`, `disabled`, `default`.|

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
  "displayAppInformationRequiredState": "String"
}

```
