---
title: Обновление microsoftAuthenticatorAuthenticationMethodConfiguration
description: Обновление свойств объекта microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6d715e32d2e42a81cf042884ab38d4f06097a3f
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874508"
---
# <a name="update-microsoftauthenticatorauthenticationmethodconfiguration"></a>Обновление microsoftAuthenticatorAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [microsoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности Microsoft Authenticator для клиента Azure AD.


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
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
В теле запроса предоставляем представление объекта [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) в JSON со значениями полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

Список свойств см. в [microsoftAuthenticatorAuthenticationMethodConfiguration.](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)

>**Примечание.** Свойство `@odata.type` со значением должно `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` быть включено в тело.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
Content-Type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "state": "String"
}
```


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "129ae788-e788-129a-88e7-9a1288e79a12",
  "state": "String"
}
```

