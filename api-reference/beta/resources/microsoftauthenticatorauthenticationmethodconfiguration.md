---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5af441d32c02f2c6b8be45ef3f3ab401b10d12da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444149"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности Microsoft Authenticator. Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которые могут использовать метод проверки подлинности.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[получение](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md);|[MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[Обновление](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|Обновление свойств объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[удаление](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md);|Нет|Возвращает объект MicrosoftAuthenticatorAuthenticationMethodConfiguration к конфигурации по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[коллекция microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)|Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

