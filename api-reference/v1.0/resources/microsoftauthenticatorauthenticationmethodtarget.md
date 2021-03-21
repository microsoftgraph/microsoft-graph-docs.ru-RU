---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 233eed9e49ca25fafbdebc0097b513122bdb9a4b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964935"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
Пространство имен: microsoft.graph

Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Объектный ID пользователя или группы Azure AD.|
|authenticationMode|MicrosoftAuthenticatorAuthenticationMode|Определяет, какие типы уведомлений можно использовать для регистрации. Возможные значения: `any` , `deviceBasedPush` (только без паролей), `push` .|
|featureSettings|authenticatorAppFeatureSettings|Определяет, какие дополнительные параметры следует применить к Microsoft Authenticator. Возможные значения: `null` , `requireNumberMatching` (Требуется совпадение номеров для уведомлений MFA. Значение игнорируется для уведомлений о входе в телефон).|
|isRegistrationRequired|Boolean|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности. *Не поддерживается.* |
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
