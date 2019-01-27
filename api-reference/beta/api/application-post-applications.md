---
title: Создание объекта Application
description: С помощью этого API можно создать объект application.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b86030eede69b85d7b66e4ec5acdd7e2dfef0ce4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515225"
---
# <a name="create-application"></a><span data-ttu-id="7cbed-103">Создание объекта Application</span><span class="sxs-lookup"><span data-stu-id="7cbed-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cbed-104">С помощью этого API можно создать объект application.</span><span class="sxs-lookup"><span data-stu-id="7cbed-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cbed-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cbed-105">Permissions</span></span>
<span data-ttu-id="7cbed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cbed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7cbed-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cbed-108">Permission type</span></span>      | <span data-ttu-id="7cbed-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cbed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cbed-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cbed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7cbed-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7cbed-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7cbed-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cbed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cbed-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cbed-113">Not supported.</span></span>    |
|<span data-ttu-id="7cbed-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cbed-114">Application</span></span> | <span data-ttu-id="7cbed-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cbed-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cbed-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cbed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="7cbed-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cbed-117">Request headers</span></span>
| <span data-ttu-id="7cbed-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7cbed-118">Name</span></span>       | <span data-ttu-id="7cbed-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7cbed-119">Type</span></span> | <span data-ttu-id="7cbed-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7cbed-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7cbed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cbed-121">Authorization</span></span>  | <span data-ttu-id="7cbed-122">string</span><span class="sxs-lookup"><span data-stu-id="7cbed-122">string</span></span>  | <span data-ttu-id="7cbed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cbed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cbed-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cbed-125">Request body</span></span>
<span data-ttu-id="7cbed-126">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cbed-126">In the request body, supply a JSON representation of [plannerBucket](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7cbed-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cbed-127">Response</span></span>

<span data-ttu-id="7cbed-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7cbed-128">If successful, this method returns `201 Created` response code and the [Contact](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cbed-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7cbed-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cbed-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cbed-130">Request</span></span>
<span data-ttu-id="7cbed-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cbed-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="7cbed-132">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cbed-132">In the request body, supply a JSON representation of [plannerBucket](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7cbed-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cbed-133">Response</span></span>
<span data-ttu-id="7cbed-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7cbed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
