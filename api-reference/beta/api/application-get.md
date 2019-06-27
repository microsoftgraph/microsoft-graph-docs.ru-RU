---
title: Получение объекта application
description: Получение свойств и связей объекта application.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 78a68dadda832d54e96163faa14a2fbbfd9668df
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258487"
---
# <a name="get-application"></a><span data-ttu-id="48b56-103">Получение объекта application</span><span class="sxs-lookup"><span data-stu-id="48b56-103">Get application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48b56-104">Получение свойств и связей объекта application.</span><span class="sxs-lookup"><span data-stu-id="48b56-104">Retrieve the properties and relationships of application object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48b56-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48b56-105">Permissions</span></span>
<span data-ttu-id="48b56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48b56-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48b56-108">Permission type</span></span>      | <span data-ttu-id="48b56-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48b56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48b56-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48b56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48b56-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48b56-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48b56-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48b56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48b56-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48b56-113">Not supported.</span></span>    |
|<span data-ttu-id="48b56-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48b56-114">Application</span></span> | <span data-ttu-id="48b56-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="48b56-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48b56-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48b56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="48b56-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48b56-117">Optional query parameters</span></span>
<span data-ttu-id="48b56-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48b56-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48b56-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48b56-119">Request headers</span></span>
| <span data-ttu-id="48b56-120">Имя</span><span class="sxs-lookup"><span data-stu-id="48b56-120">Name</span></span>       | <span data-ttu-id="48b56-121">Тип</span><span class="sxs-lookup"><span data-stu-id="48b56-121">Type</span></span> | <span data-ttu-id="48b56-122">Описание</span><span class="sxs-lookup"><span data-stu-id="48b56-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="48b56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48b56-123">Authorization</span></span>  | <span data-ttu-id="48b56-124">string</span><span class="sxs-lookup"><span data-stu-id="48b56-124">string</span></span>  | <span data-ttu-id="48b56-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48b56-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48b56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48b56-127">Request body</span></span>
<span data-ttu-id="48b56-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48b56-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48b56-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="48b56-129">Response</span></span>

<span data-ttu-id="48b56-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48b56-130">If successful, this method returns a `200 OK` response code and [application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48b56-131">Пример</span><span class="sxs-lookup"><span data-stu-id="48b56-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48b56-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="48b56-132">Request</span></span>
<span data-ttu-id="48b56-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48b56-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="48b56-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="48b56-134">Response</span></span>
<span data-ttu-id="48b56-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48b56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "api": {
    "acceptedAccessTokenVersion": 1,
    "publishedPermissionScopes": [
      {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
      }
    ]
  },
  "allowPublicClient": true,
  "applicationAliases": [
    "applicationAliases-value"
  ],
  "createdDateTime": "datetime-value",
  "installedClients": {
    "redirectUrls": [
      "redirectUrls-value"
    ]
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="48b56-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="48b56-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="48b56-139">C#</span><span class="sxs-lookup"><span data-stu-id="48b56-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48b56-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48b56-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_application-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="48b56-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48b56-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_application-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/application-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/application-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
