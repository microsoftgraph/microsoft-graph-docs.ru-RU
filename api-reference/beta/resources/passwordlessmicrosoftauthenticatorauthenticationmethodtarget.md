---
title: Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику проверки подлинности на телефоне без пароля Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d3dd874b96a54dc7e764200800e85b445abd50ee
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137657"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a>Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget (неподготовлен)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, которые могут использовать политику проверки подлинности на телефоне без пароля Microsoft Authenticator](.. /resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.

> [!CAUTION]
> API политики проверки подлинности для телефона без пароля Microsoft Authenticator является неподготовленным и больше не возвращает результаты 31 декабря 2020 г. Используйте новую политику метода [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ИД объекта пользователя или группы Azure AD.|
|isRegistrationRequired|Boolean|Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности.|
|shownContext|authenticatorAppContextType|Возможные значения: `location`, `app`.|
|targetType|authenticationMethodTargetType|Возможные значения: `user`, `group`.|
|useForSignIn|Boolean|Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
