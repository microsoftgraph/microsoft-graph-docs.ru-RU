---
title: Список применяетсяTo
description: Список ресурсов, присвоенных политике управления приложениями.
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5ada4a6c98f8568fe4761898f92d7c34d1bc7f65
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688375"
---
# <a name="list-appliesto"></a>Список применяетсяTo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список основных объектов приложения и службы, задав объект [политики appManagementPolicy.](../resources/appManagementPolicy.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                             |
| :------------------------------------- | :--------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Application.Read.All и Policy.Read.All, Application.Read.All и Policy.ReadWrite.ApplicationConfiguration |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                             |
| Application                            | Application.Read.All и Policy.Read.All, Application.Read.All и Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /policies/appManagementPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры `$select` `$filter` запроса OData и OData для настройки `$top` ответа. Вы можете применить `$filter` к свойствам [поддерживаемых объектов](../resources/application.md) приложения или [servicePrincipal.](../resources/serviceprincipal.md) `$filter` Например, в следующем запросе извлекаем **appId** и **displayName** приложений или директоров служб, которые назначены политике.

``` http

https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}/appliesTo?$select=appId,displayName
```

Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [appManagementPolicy](../resources/appManagementPolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-get-applications-and-service-principal-objects-applied-to-an-app-management-policy"></a>Пример 1. Применение приложений и основных объектов службы к политике управления приложениями

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appManagementPolicyAppliesTo"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}/appliesTo
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appmanagementpolicyappliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appmanagementpolicyappliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appmanagementpolicyappliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appmanagementpolicyappliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "0d77e011-2fc6-438f-8b93-decb4f926929",
      "appId": "8f527de6-05c9-4032-bca9-b2b56ab2358a",
      "displayName": "TestApp1",
      "createdDateTime": "2018-01-24T05:55:37Z"
    }
  ]
}
```

### <a name="example-2-get-specific-properties-of-applications-and-service-principal-objects-applied-to-an-app-management-policy-using-select-query-option"></a>Пример 2. Получение определенных свойств приложений и основных объектов службы, применяемых к политике управления приложениями с $select запроса

#### <a name="request"></a>Запрос

Ниже приводится пример запроса с помощью $select запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appManagementPolicyAppliesTo_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}/appliesTo?$select=id,appId,displayName,createdDateTime
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appmanagementpolicyappliesto-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appmanagementpolicyappliesto-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appmanagementpolicyappliesto-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appmanagementpolicyappliesto-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приводится пример возвращаемого ответа, а также приложений и директоров служб, в которых `id` `appId` применяется `displayName` `createdDateTime` политика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects(id,appId,displayName,createdDateTime)",
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "0d77e011-2fc6-438f-8b93-decb4f926929",
      "appId": "8f527de6-05c9-4032-bca9-b2b56ab2358a",
      "displayName": "TestApp1",
      "createdDateTime": "2018-01-24T05:55:37Z"
    },
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "0e1fa067-dcc1-4d85-9b4c-e69145dd3efb",
      "appId": "255912cb-e31d-4dee-bee4-3fa5d774d6b9",
      "displayName": "TestApp2",
      "createdDateTime": "2018-01-24T05:55:37Z"
    }
  ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "list resources for appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
