---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type
description: Представление метода microsoft Authenticator Passwordless Phone Sign-in, зарегистрированного на пользователя.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0949a92d0adbcfdd53164b550b6d8f8bc07444eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444079"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type-deprecated"></a>passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type (deprecated)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление метода microsoft Authenticator Passwordless Phone Sign-in, зарегистрированного на пользователя.

> [!CAUTION]
> API без пароля Microsoft Authenticator phone is deprecated and will stop returning results on 31 December 2020. Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (неподготовленный)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) collection|Извлечение списка объектов без паролейMicrosoftAuthenticatorAuthenticationMethod и их свойств.|
|[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (deprecated)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Ознакомьтесь с свойствами и отношениями объекта без пароляMicrosoftAuthenticatorAuthenticationMethod.|
|[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (deprecated)|Нет|Удаляет объект без пароляMicrosoftAuthenticatorAuthenticationMethod.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор метода проверки подлинности.|
|displayName|String|Отображающее имя мобильного устройства в качестве данной пользователем.|
|creationDateTime|DateTimeOffset|Время регистрации этого метода пользователем.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

