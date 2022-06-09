---
title: Тип ресурса проверки подлинности
description: Предоставляет связи, которые представляют методы проверки подлинности, поддерживаемые Azure AD и настроенные для пользователей.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 34a7877f8b88e319cfb4ff0e710b064f56365eae
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971380"
---
# <a name="authentication-resource-type"></a>Тип ресурса проверки подлинности

Пространство имен: microsoft.graph

Предоставляет связи, которые представляют методы проверки подлинности, поддерживаемые Azure AD и настроенные для пользователей.

Наследует [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|fido2Methods|[Коллекция fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)|Представляет ключи безопасности FIDO2, зарегистрированные для пользователя для проверки подлинности.|
|Методы|[Коллекция authenticationMethod](../resources/authenticationmethod.md)| Представляет все методы проверки подлинности, зарегистрированные для пользователя.|
|microsoftAuthenticatorMethods|[Коллекция microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)| Сведения о приложении Microsoft Authenticator, зарегистрированном для пользователя для проверки подлинности. |
|temporaryAccessPassMethods|[Коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Представляет временный секретный код, зарегистрированный пользователю для проверки подлинности с помощью секретных кодов с ограниченным временем.|
|windowsHelloForBusinessMethods|[Коллекция windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Представляет метод проверки подлинности Windows Hello для бизнеса, зарегистрированный для пользователя для проверки подлинности.|

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
