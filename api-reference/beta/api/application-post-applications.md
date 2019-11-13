---
title: Создание приложения
description: Создайте новое приложение.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b82c816eb9b55086431936b9b033d4e7179317a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934324"
---
# <a name="create-application"></a><span data-ttu-id="a4ada-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="a4ada-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4ada-104">Создайте новый объект [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="a4ada-104">Create a new [](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4ada-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ada-105">Permissions</span></span>
<span data-ttu-id="a4ada-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a4ada-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ada-108">Permission type</span></span>      | <span data-ttu-id="a4ada-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4ada-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4ada-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4ada-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4ada-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4ada-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4ada-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4ada-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4ada-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ada-113">Not supported.</span></span>    |
|<span data-ttu-id="a4ada-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4ada-114">Application</span></span> | <span data-ttu-id="a4ada-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ada-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4ada-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4ada-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="a4ada-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4ada-117">Request headers</span></span>
| <span data-ttu-id="a4ada-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a4ada-118">Name</span></span>       | <span data-ttu-id="a4ada-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ada-119">Type</span></span> | <span data-ttu-id="a4ada-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ada-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a4ada-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4ada-121">Authorization</span></span>  | <span data-ttu-id="a4ada-122">string</span><span class="sxs-lookup"><span data-stu-id="a4ada-122">string</span></span>  | <span data-ttu-id="a4ada-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4ada-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4ada-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4ada-125">Request body</span></span>
<span data-ttu-id="a4ada-126">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4ada-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="a4ada-127">Текст запроса должен включать обязательное свойство **displayName**.</span><span class="sxs-lookup"><span data-stu-id="a4ada-127">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="a4ada-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ada-128">Response</span></span>

<span data-ttu-id="a4ada-129">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4ada-129">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4ada-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4ada-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="a4ada-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4ada-131">Request</span></span>
<span data-ttu-id="a4ada-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4ada-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4ada-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ada-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "displayName": "Display name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4ada-134">C#</span><span class="sxs-lookup"><span data-stu-id="a4ada-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4ada-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4ada-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4ada-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4ada-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a4ada-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ada-137">Response</span></span>
<span data-ttu-id="a4ada-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4ada-138">Here is an example of the response.</span></span> 

> <span data-ttu-id="a4ada-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4ada-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

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
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
