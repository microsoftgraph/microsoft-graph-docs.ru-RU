---
title: Создание приложения
description: Создайте новое приложение.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d6fbb458a66f31a53917d4a0a328f399cb2593
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441489"
---
# <a name="create-application"></a><span data-ttu-id="73468-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="73468-103">Create application</span></span>

<span data-ttu-id="73468-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73468-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73468-105">Создайте новый объект [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="73468-105">Create a new [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73468-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73468-106">Permissions</span></span>
<span data-ttu-id="73468-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="73468-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73468-109">Permission type</span></span>      | <span data-ttu-id="73468-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73468-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73468-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73468-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73468-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73468-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73468-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73468-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73468-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73468-114">Not supported.</span></span>    |
|<span data-ttu-id="73468-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73468-115">Application</span></span> | <span data-ttu-id="73468-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73468-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73468-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73468-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="73468-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73468-118">Request headers</span></span>
| <span data-ttu-id="73468-119">Имя</span><span class="sxs-lookup"><span data-stu-id="73468-119">Name</span></span>       | <span data-ttu-id="73468-120">Тип</span><span class="sxs-lookup"><span data-stu-id="73468-120">Type</span></span> | <span data-ttu-id="73468-121">Описание</span><span class="sxs-lookup"><span data-stu-id="73468-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73468-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73468-122">Authorization</span></span>  | <span data-ttu-id="73468-123">string</span><span class="sxs-lookup"><span data-stu-id="73468-123">string</span></span>  | <span data-ttu-id="73468-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73468-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73468-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73468-126">Request body</span></span>
<span data-ttu-id="73468-127">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73468-127">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="73468-128">Текст запроса должен включать обязательное свойство **displayName**.</span><span class="sxs-lookup"><span data-stu-id="73468-128">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="73468-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="73468-129">Response</span></span>

<span data-ttu-id="73468-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73468-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73468-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="73468-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="73468-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73468-132">Request</span></span>
<span data-ttu-id="73468-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73468-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73468-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="73468-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="73468-135">C#</span><span class="sxs-lookup"><span data-stu-id="73468-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73468-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73468-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73468-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73468-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="73468-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="73468-138">Response</span></span>
<span data-ttu-id="73468-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73468-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="73468-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73468-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
