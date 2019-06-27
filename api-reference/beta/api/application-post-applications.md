---
title: Создание объекта Application
description: С помощью этого API можно создать объект application.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a9cf7f8888ee8026a3a98d2816c64c82c8f45b1e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258445"
---
# <a name="create-application"></a><span data-ttu-id="e2ea0-103">Создание объекта Application</span><span class="sxs-lookup"><span data-stu-id="e2ea0-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2ea0-104">С помощью этого API можно создать объект application.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2ea0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ea0-105">Permissions</span></span>
<span data-ttu-id="e2ea0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e2ea0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2ea0-108">Permission type</span></span>      | <span data-ttu-id="e2ea0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2ea0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2ea0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2ea0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2ea0-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2ea0-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2ea0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2ea0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2ea0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-113">Not supported.</span></span>    |
|<span data-ttu-id="e2ea0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2ea0-114">Application</span></span> | <span data-ttu-id="e2ea0-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2ea0-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2ea0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2ea0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="e2ea0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2ea0-117">Request headers</span></span>
| <span data-ttu-id="e2ea0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e2ea0-118">Name</span></span>       | <span data-ttu-id="e2ea0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e2ea0-119">Type</span></span> | <span data-ttu-id="e2ea0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ea0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2ea0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2ea0-121">Authorization</span></span>  | <span data-ttu-id="e2ea0-122">string</span><span class="sxs-lookup"><span data-stu-id="e2ea0-122">string</span></span>  | <span data-ttu-id="e2ea0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2ea0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2ea0-125">Request body</span></span>
<span data-ttu-id="e2ea0-126">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2ea0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2ea0-127">Response</span></span>

<span data-ttu-id="e2ea0-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2ea0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e2ea0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2ea0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2ea0-130">Request</span></span>
<span data-ttu-id="e2ea0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "allowPublicClient": true,
  "displayName": "Display name"
}
```
<span data-ttu-id="e2ea0-132">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e2ea0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2ea0-133">Response</span></span>
<span data-ttu-id="e2ea0-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2ea0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "id": "b5b2920e-a47c-43b7-91ef-25ae96fddddd",
    "deletedDateTime": null,
    "api": {
        "acceptedAccessTokenVersion": 2,
        "publishedPermissionScopes": []
    },
    "allowPublicClient": true,
    "applicationAliases": [],
    "appRoles": [],
    "createdDateTime": "2017-05-25T16:33:04.3646617Z",
    "installedClients": {
        "redirectUrls": []
    },
    "displayName": "Display name",
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "orgRestrictions": [],
    "passwordCredentials": [],
    "preAuthorizedApplications": [],
    "requiredResourceAccess": [],
    "tags": [],
    "web": {
        "redirectUrls": [],
        "logoutUrl": null,
        "oauth2AllowImplicitFlow": null
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e2ea0-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e2ea0-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e2ea0-138">C#</span><span class="sxs-lookup"><span data-stu-id="e2ea0-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_application_from_applications-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2ea0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2ea0-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_application_from_applications-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e2ea0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2ea0-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_application_from_applications-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
