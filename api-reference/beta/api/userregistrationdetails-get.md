---
title: Get userRegistrationDetails
description: Ознакомьтесь с свойствами и отношениями объекта userRegistrationDetails.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: b70b2557ca5ec9b0af2d0a7d5d9f714777b385f1
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201792"
---
# <a name="get-userregistrationdetails"></a>Get userRegistrationDetails
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями [объекта userRegistrationDetails.](../resources/userregistrationdetails.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|UserAuthenticationMethod.Read.All, AuditLog.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|UserAuthenticationMethod.Read.All, AuditLog.Read.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/userRegistrationDetails/{userRegistrationDetailsId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не поддерживает параметры запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа и `200 OK` [объект userRegistrationDetails](../resources/userregistrationdetails.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_userregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/userRegistrationDetails/{userRegistrationDetailsId}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.userRegistrationDetails",
    "id": "6832a83d-2ef9-c5f5-9a2d-f2761d7ff317",
    "userDisplayName": "Abbe Smith",
    "userPrincipalName": "abbe@contoso.com",
    "isMfaRegistered": "true",
    "isMfaCapable": "true",
    "isSsprRegistered": "true",
    "isSsprEnabled": "false",
    "isSsprCapable": "false",
    "isPasswordlessCapable": "false",
    "methodsRegistered": [
      "mobilePhone",
      "email"
    ]
  }
}
```

