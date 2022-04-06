---
title: Тип ресурса проверки подлинности
description: Предоставляет отношения, которые представляют методы проверки подлинности, поддерживаемые Azure AD и настроенные для пользователей.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c098cc1b813a3805c1afc3956d93b6a416aa239
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510721"
---
# <a name="authentication-resource-type"></a>Тип ресурса проверки подлинности

Пространство имен: microsoft.graph

Предоставляет отношения, которые представляют методы проверки подлинности, поддерживаемые Azure AD и настроенные для пользователей.

Наследует [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|fido2Methods|[коллекция fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Представляет ключи безопасности FIDO2, зарегистрированные пользователю для проверки подлинности.|
|методы|[коллекция authenticationMethod](../resources/authenticationmethod.md)| Представляет все методы проверки подлинности, зарегистрированные пользователем.|
|MicrosoftAuthenticatorMethods|[коллекция microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)| Сведения о приложении Microsoft Authenticator, зарегистрированного пользователем для проверки подлинности. |
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

