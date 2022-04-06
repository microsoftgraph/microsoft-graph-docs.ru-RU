---
title: Тип ресурса проверки подлинности
description: Предоставляет отношения, которые представляют методы проверки подлинности, поддерживаемые Azure AD и настроенные для пользователей.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7bf797abcaa2117e603cf7eec69d13d981c5f5ec
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510735"
---
# <a name="authentication-resource-type"></a>Тип ресурса проверки подлинности

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет отношения, которые представляют методы проверки подлинности, поддерживаемые Azure AD и настроенные для пользователей.

Наследует [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|emailMethods|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection|Представляет адреса электронной почты, зарегистрированные пользователем для проверки подлинности. |
|fido2Methods|[коллекция fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Представляет ключи безопасности FIDO2, зарегистрированные пользователю для проверки подлинности.|
|методы|[коллекция authenticationMethod](../resources/authenticationmethod.md)| Представляет все методы проверки подлинности, зарегистрированные пользователем.|
|MicrosoftAuthenticatorMethods|[коллекция microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)| Сведения о приложении Microsoft Authenticator, зарегистрированного пользователем для проверки подлинности. |
|passwordlessMicrosoftAuthenticatorMethods|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) collection|Представляет Microsoft Authenticator методы Телефон, зарегистрированные пользователю для проверки подлинности.|
|passwordMethods|[passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) collection|Представляет сведения о методе проверки подлинности паролей, зарегистрированного пользователем для проверки подлинности.|
|phoneMethods|[коллекция phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)|Представляет телефон, зарегистрированный пользователю для проверки подлинности. |
|temporaryAccessPassMethods|[коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Представляет временный пропуск доступа, зарегистрированный пользователю для проверки подлинности с помощью ограниченных по времени паролей.|
|windowsHelloForBusinessMethods|[коллекция windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Представляет метод Windows Hello для бизнеса проверки подлинности, зарегистрированный пользователем для проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authentication",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authentication"
}
```

