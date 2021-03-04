---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration resource type
description: Представляет политику методов проверки подлинности без паролей Microsoft Authenticator Phone.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 054a8c01e0a8ccb1523622fe5df20e8e60831f60
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444065"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type-deprecated"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration resource type (deprecated)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности без паролей Microsoft Authenticator Phone. Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которые могут использовать метод проверки подлинности.

> [!CAUTION]
> API политики метода проверки подлинности без паролей Microsoft Authenticator Phone является обесценен и перестал возвращать результаты 31 декабря 2020 г. Используйте новую политику метода проверки подлинности [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (deprecated)|[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[Обновление](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (неподготовленное) |[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Обновление свойств объекта без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (deprecated)|Нет|Возвращает объект passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration в конфигурацию по умолчанию.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) collection|Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
