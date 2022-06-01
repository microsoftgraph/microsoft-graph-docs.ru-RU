---
title: Перечисление userRegistrationDetails
description: Получение списка методов проверки подлинности, зарегистрированных для пользователя, как определено в объекте userRegistrationDetails.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: e504bbd4ac4326c68eef1b94ccdde2e6aca68762
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820856"
---
# <a name="list-userregistrationdetails"></a>Перечисление userRegistrationDetails
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка методов проверки подлинности, зарегистрированных для пользователя, как определено в [объекте userRegistrationDetails](../resources/userregistrationdetails.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|UserAuthenticationMethod.Read.All, AuditLog.Read.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|UserAuthenticationMethod.Read.All, AuditLog.Read.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/userRegistrationDetails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает только параметры `$filter` запроса `$orderBy` oData и параметры запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [userRegistrationDetails](../resources/userregistrationdetails.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/userRegistrationDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-userregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-userregistrationdetails-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-userregistrationdetails-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userRegistrationDetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#reports/authenticationMethods/userRegistrationDetails",
    "value": [
        {
            "id": "86462606-fde0-4fc4-9e0c-a20eb73e54c6",
            "userPrincipalName": "AlexW@Contoso.com",
            "userDisplayName": "Alex Wilber",
            "isSsprRegistered": false,
            "isSsprEnabled": false,
            "isSsprCapable": false,
            "isMfaRegistered": true,
            "isMfaCapable": true,
            "isPasswordlessCapable": false,
            "methodsRegistered": [
                "microsoftAuthenticatorPush",
                "softwareOneTimePasscode"
            ],
            "defaultMethod": "microsoftAuthenticatorPush"
        },
        {
            "id": "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f",
            "userPrincipalName": "AllanD@Contoso.com",
            "userDisplayName": "Allan Deyoung",
            "isSsprRegistered": false,
            "isSsprEnabled": false,
            "isSsprCapable": false,
            "isMfaRegistered": false,
            "isMfaCapable": false,
            "isPasswordlessCapable": false,
            "methodsRegistered": [],
            "defaultMethod": ""    
        },
        {
            "id": "c8096958-797c-44fa-8fde-a6fb62567cf0",
            "userPrincipalName": "BiancaP@Contoso.com",
            "userDisplayName": "Bianca Pisani",
            "isSsprRegistered": true,
            "isSsprEnabled": false,
            "isSsprCapable": false,
            "isMfaRegistered": true,
            "isMfaCapable": true,
            "isPasswordlessCapable": false,
            "methodsRegistered": [
                "mobilePhone",
                "microsoftAuthenticatorPush",
                "softwareOneTimePasscode"
            ],
            "defaultMethod": "mobilePhone"
        }
    ]
}
```

