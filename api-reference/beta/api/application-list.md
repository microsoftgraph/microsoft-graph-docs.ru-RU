---
title: Список приложений
description: Получение списка приложений в организации.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45bd17b5f855db16d8e3716d7df8cae5b35c41eb
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41233958"
---
# <a name="list-applications"></a><span data-ttu-id="ad2ab-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="ad2ab-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad2ab-104">Получение списка [приложений](../resources/application.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-104">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad2ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad2ab-105">Permissions</span></span>
<span data-ttu-id="ad2ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad2ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad2ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad2ab-108">Permission type</span></span>      | <span data-ttu-id="ad2ab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad2ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad2ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad2ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad2ab-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad2ab-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad2ab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad2ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad2ab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-113">Not supported.</span></span>    |
|<span data-ttu-id="ad2ab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad2ab-114">Application</span></span> | <span data-ttu-id="ad2ab-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad2ab-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad2ab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad2ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ad2ab-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad2ab-117">Optional query parameters</span></span>
<span data-ttu-id="ad2ab-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad2ab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad2ab-119">Request headers</span></span>
| <span data-ttu-id="ad2ab-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ad2ab-120">Name</span></span>       | <span data-ttu-id="ad2ab-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ad2ab-121">Type</span></span> | <span data-ttu-id="ad2ab-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ad2ab-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ad2ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad2ab-123">Authorization</span></span>  | <span data-ttu-id="ad2ab-124">string</span><span class="sxs-lookup"><span data-stu-id="ad2ab-124">string</span></span>  | <span data-ttu-id="ad2ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad2ab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad2ab-127">Request body</span></span>
<span data-ttu-id="ad2ab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad2ab-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad2ab-129">Response</span></span>

<span data-ttu-id="ad2ab-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-130">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="ad2ab-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ad2ab-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="ad2ab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad2ab-132">Request</span></span>
<span data-ttu-id="ad2ab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad2ab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad2ab-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad2ab-135">C#</span><span class="sxs-lookup"><span data-stu-id="ad2ab-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad2ab-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad2ab-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad2ab-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad2ab-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ad2ab-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad2ab-138">Response</span></span>
<span data-ttu-id="ad2ab-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="ad2ab-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad2ab-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications",
    "value": [
        {
            "id": "00af5dfb-85da-4b41-a677-0c6b86dd34f8",
            "deletedDateTime": null,
            "isFallbackPublicClient": false,
            "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
            "applicationTemplateId": null,
            "identifierUris": [
                "http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"
            ],
            "createdDateTime": "2019-09-15T05:23:08Z",
            "displayName": "My app",
            "isDeviceOnlyAuthSupported": null,
            "groupMembershipClaims": null,
            "optionalClaims": null,
            "orgRestrictions": [],
            "publisherDomain": "contoso.onmicrosoft.com",
            "signInAudience": "AzureADMyOrg",
            "tags": [],
            "tokenEncryptionKeyId": null,
            "api": {
                "requestedAccessTokenVersion": null,
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
                "redirectUris": [
                    "https://127.0.0.1:444/applications/default.aspx"
                ],
                "homePageUrl": "http://www.contoso.com/landingPage",
                "logoutUrl": null,
                "implicitGrantSettings": {
                    "enableIdTokenIssuance": true,
                    "enableAccessTokenIssuance": false
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
