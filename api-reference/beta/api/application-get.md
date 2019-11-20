---
title: Получение объекта application
description: Получение свойств и связей объекта application.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5a2fd02e7cf078aee3898b881d4754169ef0d6a
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747631"
---
# <a name="get-application"></a><span data-ttu-id="f6c48-103">Получение объекта application</span><span class="sxs-lookup"><span data-stu-id="f6c48-103">Get application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6c48-104">Получение свойств и связей объекта [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="f6c48-104">Get the properties and relationships of an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c48-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6c48-105">Permissions</span></span>
<span data-ttu-id="f6c48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6c48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6c48-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6c48-108">Permission type</span></span>      | <span data-ttu-id="f6c48-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6c48-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6c48-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6c48-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6c48-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6c48-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6c48-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6c48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c48-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6c48-113">Not supported.</span></span>    |
|<span data-ttu-id="f6c48-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6c48-114">Application</span></span> | <span data-ttu-id="f6c48-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6c48-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6c48-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6c48-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6c48-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6c48-117">Optional query parameters</span></span>
<span data-ttu-id="f6c48-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f6c48-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6c48-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6c48-119">Request headers</span></span>
| <span data-ttu-id="f6c48-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f6c48-120">Name</span></span>       | <span data-ttu-id="f6c48-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f6c48-121">Type</span></span> | <span data-ttu-id="f6c48-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c48-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6c48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c48-123">Authorization</span></span>  | <span data-ttu-id="f6c48-124">string</span><span class="sxs-lookup"><span data-stu-id="f6c48-124">string</span></span>  | <span data-ttu-id="f6c48-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6c48-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f6c48-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6c48-127">Content-type</span></span> | <span data-ttu-id="f6c48-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6c48-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6c48-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6c48-130">Request body</span></span>
<span data-ttu-id="f6c48-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6c48-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6c48-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6c48-132">Response</span></span>

<span data-ttu-id="f6c48-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6c48-133">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="f6c48-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6c48-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f6c48-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6c48-135">Request</span></span>
<span data-ttu-id="f6c48-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6c48-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6c48-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6c48-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6c48-138">C#</span><span class="sxs-lookup"><span data-stu-id="f6c48-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6c48-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6c48-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6c48-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6c48-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f6c48-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6c48-141">Response</span></span>
<span data-ttu-id="f6c48-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6c48-142">Here is an example of the response.</span></span> 

><span data-ttu-id="f6c48-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6c48-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
