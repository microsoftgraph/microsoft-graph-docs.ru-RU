---
title: Получение Онпремисесажент
description: Получение свойств и связей объекта Онпремисесажент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8b789810c7a95264f8f8b48af3d0671194a34b4
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726178"
---
# <a name="get-onpremisesagent"></a><span data-ttu-id="09855-103">Получение Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="09855-103">Get onPremisesAgent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09855-104">Получение свойств и связей объекта [онпремисесажент](../resources/onpremisesagent.md) .</span><span class="sxs-lookup"><span data-stu-id="09855-104">Retrieve the properties and relationships of an [onPremisesAgent](../resources/onpremisesagent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09855-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09855-105">Permissions</span></span>

<span data-ttu-id="09855-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09855-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09855-108">Permission type</span></span>                        | <span data-ttu-id="09855-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09855-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="09855-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09855-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="09855-111">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09855-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="09855-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09855-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09855-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09855-113">Not supported.</span></span> |
| <span data-ttu-id="09855-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09855-114">Application</span></span>                            | <span data-ttu-id="09855-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09855-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09855-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09855-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/?$expand=agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09855-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="09855-117">Optional query parameters</span></span>

<span data-ttu-id="09855-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="09855-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09855-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09855-119">Request headers</span></span>

| <span data-ttu-id="09855-120">Имя</span><span class="sxs-lookup"><span data-stu-id="09855-120">Name</span></span>      |<span data-ttu-id="09855-121">Описание</span><span class="sxs-lookup"><span data-stu-id="09855-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09855-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09855-122">Authorization</span></span> | <span data-ttu-id="09855-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="09855-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="09855-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09855-124">Request body</span></span>

<span data-ttu-id="09855-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09855-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09855-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="09855-126">Response</span></span>

<span data-ttu-id="09855-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [онпремисесажент](../resources/onpremisesagent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09855-127">If successful, this method returns a `200 OK` response code and an [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09855-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="09855-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09855-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="09855-129">Request</span></span>

<span data-ttu-id="09855-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09855-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="09855-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="09855-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="09855-132">C#</span><span class="sxs-lookup"><span data-stu-id="09855-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09855-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09855-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="09855-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09855-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09855-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="09855-135">Response</span></span>

<span data-ttu-id="09855-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="09855-136">The following is an example of the response.</span></span>

> <span data-ttu-id="09855-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09855-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
    "status": "Active",
    "machineName": "server1.local1.contoso.com",
    "externalIp": "153.69.23.122",
    "agentGroups": [
         {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1"
         }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
