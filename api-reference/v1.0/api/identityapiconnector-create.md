---
title: Создание identityApiConnector
description: Создание нового объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8cdebdaa8ed86e6d6d60ad07c987b2152baf6737
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920366"
---
# <a name="create-identityapiconnector"></a>Создание identityApiConnector

Пространство имен: microsoft.graph

Создание нового [объекта identityApiConnector.](../resources/identityapiconnector.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | APIConnectors.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.  |
| Для приложений                            | APIConnectors.ReadWrite.All |

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор потока внешних пользователей удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [identityApiConnector.](../resources/identityapiconnector.md)

В следующей таблице показаны свойства, необходимые при создании [identityApiConnector.](../resources/identityapiconnector.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка| Имя соединитетеля API. |
|targetUrl|Строка| URL-адрес конечной точки API для вызова. |
|проверка подлинностиКонфигурация|[apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)|Объект, описывая сведения о конфигурации проверки подлинности для вызова API. [Поддерживается базовая](../resources/basicauthentication.md) проверка подлинности и [клиентский сертификат PKCS 12.](../resources/pkcs12certificate.md)|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-create-an-api-connector-with-basic-authentication"></a>Пример 1. Создание соединителя API с базовой проверкой подлинности

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username": "MyUsername",
      "password": "MyPassword"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "MyUsername",
        "password": "******"
    }
}
```

### <a name="example-2-create-an-api-connector-with-client-certificate-authentication"></a>Пример 2. Создание соединителя API с проверкой подлинности сертификата клиента

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

> **Примечание:** `authenticationConfiguration` в запросе имеется тип [microsoft.graph.pkcs12certificate,](../resources/pkcs12certificate.md)который представляет конфигурацию сертификата, необходимого для загрузки или создания.

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type":"#microsoft.graph.pkcs12Certificate",
        "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
        "password": "CertificatePassword"
    }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание:** `authenticationConfiguration` в ответе — тип [microsoft.graph.clientCertificateAuthentication,](../resources/clientcertificateauthentication.md) так как это представляет общедоступные сведения о загруженных сертификатах.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
        "certificateList": [
            {
                "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                "notAfter": 1666350522,
                "notBefore": 1508670522,
                "isActive": true
            }
        ]
    }
}
```
