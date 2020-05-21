---
title: Создание serviceprincipal
description: Создание нового объекта serviceprincipal.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ec647e98f7c7810f560e454acf0eaccfbe5990af
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335850"
---
# <a name="create-serviceprincipal"></a>Создание servicePrincipal

Пространство имен: microsoft.graph

Создание нового объекта [servicePrincipal](../resources/serviceprincipal.md) .

> [!IMPORTANT]
> Добавление [**пассвордкредентиал**](../resources/passwordcredential.md) при создании сервицепринЦипалс не поддерживается. Используйте метод [аддпассворд](serviceprincipal-addpassword.md) , чтобы добавить пароли для объекта servicePrincipal.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /serviceprincipals
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Основной текст запроса
В тексте запроса добавьте представление объекта [serviceprincipal](../resources/serviceprincipal.md) в формате JSON. Текст запроса должен содержать **AppID**.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [serviceprincipal](../resources/serviceprincipal.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}-->
```http
POST https://graph.microsoft.com/v1.0/serviceprincipals
Content-type: application/json

{
  "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-from-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-from-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-from-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-serviceprincipal-from-serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals/$entity",
    "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appDisplayName": "My App",
    "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
    "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
    "appRoleAssignmentRequired": false,
    "displayName": "foo",
    "homepage": null,
    "logoutUrl": null,
    "publisherName": "Contoso",
    "replyUrls": [],
    "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
    ],
    "tags": [],
    "addIns": [],
    "appRoles": [],
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [],
    "passwordCredentials": []
}
```
