---
title: Создание объекта Application
description: С помощью этого API можно создать объект application.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 775f7d59ba19ed015b7af5d66e9d52ae817ec65c
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908322"
---
# <a name="create-application"></a><span data-ttu-id="ad4c3-103">Создание объекта Application</span><span class="sxs-lookup"><span data-stu-id="ad4c3-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad4c3-104">С помощью этого API можно создать объект application.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad4c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad4c3-105">Permissions</span></span>
<span data-ttu-id="ad4c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad4c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad4c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad4c3-108">Permission type</span></span>      | <span data-ttu-id="ad4c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad4c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad4c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad4c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad4c3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad4c3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad4c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad4c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad4c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-113">Not supported.</span></span>    |
|<span data-ttu-id="ad4c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad4c3-114">Application</span></span> | <span data-ttu-id="ad4c3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad4c3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad4c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad4c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="ad4c3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad4c3-117">Request headers</span></span>
| <span data-ttu-id="ad4c3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ad4c3-118">Name</span></span>       | <span data-ttu-id="ad4c3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ad4c3-119">Type</span></span> | <span data-ttu-id="ad4c3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad4c3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad4c3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad4c3-121">Authorization</span></span>  | <span data-ttu-id="ad4c3-122">string</span><span class="sxs-lookup"><span data-stu-id="ad4c3-122">string</span></span>  | <span data-ttu-id="ad4c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad4c3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad4c3-125">Request body</span></span>
<span data-ttu-id="ad4c3-126">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ad4c3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad4c3-127">Response</span></span>

<span data-ttu-id="ad4c3-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad4c3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ad4c3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad4c3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad4c3-130">Request</span></span>
<span data-ttu-id="ad4c3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad4c3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad4c3-132">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad4c3-133">C#</span><span class="sxs-lookup"><span data-stu-id="ad4c3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad4c3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad4c3-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad4c3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad4c3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ad4c3-136">Java</span><span class="sxs-lookup"><span data-stu-id="ad4c3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ad4c3-137">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-137">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ad4c3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad4c3-138">Response</span></span>
<span data-ttu-id="ad4c3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad4c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
