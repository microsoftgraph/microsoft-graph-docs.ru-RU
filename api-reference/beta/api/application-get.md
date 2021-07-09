---
title: Получение объекта application
description: Получение свойств и связей объекта application.
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1fbfebb6a889ffae5ae6052cc1b774d335f9fb50
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350879"
---
# <a name="get-application"></a><span data-ttu-id="63086-103">Получение объекта application</span><span class="sxs-lookup"><span data-stu-id="63086-103">Get application</span></span>

<span data-ttu-id="63086-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63086-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63086-105">Получение свойств и связей объекта [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="63086-105">Get the properties and relationships of an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63086-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63086-106">Permissions</span></span>
<span data-ttu-id="63086-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63086-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63086-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63086-109">Permission type</span></span>      | <span data-ttu-id="63086-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63086-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63086-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63086-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63086-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63086-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63086-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63086-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63086-114">Application.Read.All, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63086-114">Application.Read.All, Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="63086-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="63086-115">Application</span></span> | <span data-ttu-id="63086-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy,  Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63086-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy,  Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63086-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63086-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="63086-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="63086-118">Optional query parameters</span></span>
<span data-ttu-id="63086-119">Этот метод поддерживает [параметр запроса OData](/graph/query-parameters) `$select` для получения конкретных свойств приложения.</span><span class="sxs-lookup"><span data-stu-id="63086-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to retrieve specific application properties.</span></span> 
## <a name="request-headers"></a><span data-ttu-id="63086-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63086-120">Request headers</span></span>
| <span data-ttu-id="63086-121">Имя</span><span class="sxs-lookup"><span data-stu-id="63086-121">Name</span></span>           | <span data-ttu-id="63086-122">Описание</span><span class="sxs-lookup"><span data-stu-id="63086-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="63086-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63086-123">Authorization</span></span>  | <span data-ttu-id="63086-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63086-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63086-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63086-126">Request body</span></span>
<span data-ttu-id="63086-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63086-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63086-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="63086-128">Response</span></span>

<span data-ttu-id="63086-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63086-129">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="63086-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="63086-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="63086-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="63086-131">Request</span></span>
<span data-ttu-id="63086-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63086-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63086-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="63086-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="63086-134">C#</span><span class="sxs-lookup"><span data-stu-id="63086-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63086-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63086-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63086-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63086-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63086-137">Java</span><span class="sxs-lookup"><span data-stu-id="63086-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="63086-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="63086-138">Response</span></span>
<span data-ttu-id="63086-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63086-139">Here is an example of the response.</span></span> 

><span data-ttu-id="63086-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63086-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
    "disabledByMicrosoftStatus": null,
    "displayName": "Display name",
    "isDeviceOnlyAuthSupported": null,
    "groupMembershipClaims": null,
    "optionalClaims": null,
    "addIns": [],
    "publisherDomain": "contoso.onmicrosoft.com",
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "api": {
        "requestedAccessTokenVersion": 2,
        "acceptMappedClaims": null,
        "knownClientApplications": [],
        "oauth2PermissionScopes": [],
        "preAuthorizedApplications": []
    },
    "appRoles": [],
    "publicClient": {
        "redirectUris": []
    },
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
        "countriesBlockedForMinors": [],
        "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "requiredResourceAccess": [],
    "uniqueName": null,
    "web": {
        "redirectUris": [],
        "homePageUrl": null,
        "logoutUrl": null,
        "implicitGrantSettings": {
            "enableIdTokenIssuance": false,
            "enableAccessTokenIssuance": false
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



