---
title: Удаление x509CertificateAuthenticationMethodConfiguration
description: Удаление объекта x509CertificateAuthenticationMethodConfiguration и восстановление всех остальных свойств в их параметрах по умолчанию
author: charlenezheng
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="delete-x509certificateauthenticationmethodconfiguration"></a>Удаление x509CertificateAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Восстановление [объекта x509CertificateAuthenticationMethodConfiguration](../resources/x509certificateauthenticationmethodconfiguration.md) в конфигурации по умолчанию.

## <a name="permissions"></a>Разрешения:
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Policy.ReadWrite.AuthenticationMethod|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

Для делегирования сценариев администратору требуется одна из следующих ролей [Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Администратор политики проверки подлинности
* Глобальный администратор

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "delete_x509certificateauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

