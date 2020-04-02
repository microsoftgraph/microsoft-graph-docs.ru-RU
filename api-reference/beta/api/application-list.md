---
title: Список приложений
description: Получение списка приложений в организации.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2655cfe15589d7df22fb4c41339696e8a6266fa5
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107187"
---
# <a name="list-applications"></a><span data-ttu-id="bb8ad-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="bb8ad-103">List applications</span></span>

<span data-ttu-id="bb8ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb8ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb8ad-105">Получение списка [приложений](../resources/application.md) в организации.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-105">Get the list of [applications](../resources/application.md) in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb8ad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb8ad-106">Permissions</span></span>
<span data-ttu-id="bb8ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb8ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bb8ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb8ad-109">Permission type</span></span>      | <span data-ttu-id="bb8ad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb8ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb8ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb8ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb8ad-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb8ad-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb8ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb8ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb8ad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-114">Not supported.</span></span>    |
|<span data-ttu-id="bb8ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb8ad-115">Application</span></span> | <span data-ttu-id="bb8ad-116">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb8ad-116">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb8ad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb8ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb8ad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb8ad-118">Optional query parameters</span></span>
<span data-ttu-id="bb8ad-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb8ad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb8ad-120">Request headers</span></span>
| <span data-ttu-id="bb8ad-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bb8ad-121">Name</span></span>       | <span data-ttu-id="bb8ad-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bb8ad-122">Type</span></span> | <span data-ttu-id="bb8ad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bb8ad-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb8ad-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb8ad-124">Authorization</span></span>  | <span data-ttu-id="bb8ad-125">string</span><span class="sxs-lookup"><span data-stu-id="bb8ad-125">string</span></span>  | <span data-ttu-id="bb8ad-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb8ad-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb8ad-128">Request body</span></span>
<span data-ttu-id="bb8ad-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb8ad-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb8ad-130">Response</span></span>

<span data-ttu-id="bb8ad-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-131">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="bb8ad-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="bb8ad-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="bb8ad-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb8ad-133">Request</span></span>
<span data-ttu-id="bb8ad-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb8ad-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb8ad-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="c"></a>[<span data-ttu-id="bb8ad-136">C#</span><span class="sxs-lookup"><span data-stu-id="bb8ad-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb8ad-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb8ad-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb8ad-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb8ad-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bb8ad-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb8ad-139">Response</span></span>
<span data-ttu-id="bb8ad-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="bb8ad-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb8ad-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
