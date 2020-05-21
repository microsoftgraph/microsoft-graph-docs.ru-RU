---
title: Получение объекта servicePrincipal
description: Получение свойств и связей объекта serviceprincipal.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0cfc71a2cc7c44e05a2f76796940b45dc3513986
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333859"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="bbd96-103">Получение объекта servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="bbd96-103">Get servicePrincipal</span></span>

<span data-ttu-id="bbd96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbd96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbd96-105">Получение свойств и связей объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="bbd96-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbd96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd96-106">Permissions</span></span>
<span data-ttu-id="bbd96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbd96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bbd96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd96-109">Permission type</span></span>      | <span data-ttu-id="bbd96-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbd96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbd96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbd96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bbd96-112">Application. Read. ALL, Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="bbd96-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bbd96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbd96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbd96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd96-114">Not supported.</span></span>    |
|<span data-ttu-id="bbd96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbd96-115">Application</span></span> | <span data-ttu-id="bbd96-116">Application. Read. ALL, Directory. Read. ALL, Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bbd96-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbd96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbd96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bbd96-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bbd96-118">Optional query parameters</span></span>
<span data-ttu-id="bbd96-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bbd96-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbd96-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbd96-120">Request headers</span></span>
| <span data-ttu-id="bbd96-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bbd96-121">Name</span></span>           | <span data-ttu-id="bbd96-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd96-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="bbd96-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbd96-123">Authorization</span></span>  | <span data-ttu-id="bbd96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbd96-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bbd96-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bbd96-126">Request body</span></span>
<span data-ttu-id="bbd96-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbd96-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbd96-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd96-128">Response</span></span>
<span data-ttu-id="bbd96-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bbd96-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbd96-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="bbd96-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="bbd96-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbd96-131">Request</span></span>
<span data-ttu-id="bbd96-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbd96-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bbd96-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbd96-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="bbd96-134">C#</span><span class="sxs-lookup"><span data-stu-id="bbd96-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbd96-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbd96-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbd96-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbd96-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbd96-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd96-137">Response</span></span>
<span data-ttu-id="bbd96-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bbd96-138">Here is an example of the response.</span></span> 

><span data-ttu-id="bbd96-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbd96-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
        "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appDisplayName": "My App",
        "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
        "applicationTemplateId": null,
        "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
        "appRoleAssignmentRequired": false,
        "displayName": "foo",
        "errorUrl": null,
        "homepage": null,
        "loginUrl": null,
        "logoutUrl": null,
        "notificationEmailAddresses": [],
        "preferredSingleSignOnMode": null,
        "preferredTokenSigningKeyEndDateTime": null,
        "preferredTokenSigningKeyThumbprint": null,
        "publisherName": "Contoso",
        "replyUrls": [],
        "samlMetadataUrl": null,
        "samlSingleSignOnSettings": null,
        "servicePrincipalNames": [
            "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
        ],
        "signInAudience": "AzureADandPersonalMicrosoftAccount",
        "tags": [],
        "addIns": [],
        "api": {
            "resourceSpecificApplicationPermissions": []
        },
        "appRoles": [],
        "info": {
            "termsOfServiceUrl": null,
            "supportUrl": null,
            "privacyStatementUrl": null,
            "marketingUrl": null,
            "logoUrl": null
        },
        "keyCredentials": [],
        "publishedPermissionScopes": [],
        "passwordCredentials": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
