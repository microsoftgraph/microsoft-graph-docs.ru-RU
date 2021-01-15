---
title: Удаление microsoftAuthenticatorAuthenticationMethodConfiguration
description: Удаляет объект microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 740bba96925e6393ce8b8c4dee517da3461b6b7c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874488"
---
# <a name="delete-microsoftauthenticatorauthenticationmethodconfiguration"></a>Удаление microsoftAuthenticatorAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удалите изменения, внесенные в политику метода проверки подлинности [Microsoft Authenticator,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) вернув политику к конфигурации по умолчанию.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Policy.ReadWrite.AuthenticationMethod|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Policy.ReadWrite.AuthenticationMethod|

Для делегирования сценариев администратору требуется роль глобального администратора. Дополнительные сведения см. в [сведениях о роли.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

