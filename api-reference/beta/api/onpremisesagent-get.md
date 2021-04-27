---
title: Get onPremisesAgent
description: Извлечение свойств и связей объекта onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 034ab82730afe99ef547d496d7addca1b503387d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038219"
---
# <a name="get-onpremisesagent"></a><span data-ttu-id="77979-103">Get onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="77979-103">Get onPremisesAgent</span></span>

<span data-ttu-id="77979-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77979-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77979-105">Извлечение свойств и связей [объекта onPremisesAgent.](../resources/onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="77979-105">Retrieve the properties and relationships of an [onPremisesAgent](../resources/onpremisesagent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77979-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77979-106">Permissions</span></span>

<span data-ttu-id="77979-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77979-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77979-109">Permission type</span></span>                        | <span data-ttu-id="77979-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77979-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="77979-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77979-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="77979-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77979-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="77979-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77979-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77979-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77979-114">Not supported.</span></span> |
| <span data-ttu-id="77979-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77979-115">Application</span></span>                            | <span data-ttu-id="77979-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77979-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77979-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77979-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/?$expand=agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77979-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77979-118">Optional query parameters</span></span>

<span data-ttu-id="77979-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="77979-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77979-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77979-120">Request headers</span></span>

| <span data-ttu-id="77979-121">Имя</span><span class="sxs-lookup"><span data-stu-id="77979-121">Name</span></span>      |<span data-ttu-id="77979-122">Описание</span><span class="sxs-lookup"><span data-stu-id="77979-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77979-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77979-123">Authorization</span></span> | <span data-ttu-id="77979-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="77979-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="77979-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77979-125">Request body</span></span>

<span data-ttu-id="77979-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77979-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77979-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="77979-127">Response</span></span>

<span data-ttu-id="77979-128">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект onPremisesAgent](../resources/onpremisesagent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77979-128">If successful, this method returns a `200 OK` response code and an [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77979-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="77979-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77979-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="77979-130">Request</span></span>

<span data-ttu-id="77979-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77979-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77979-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="77979-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="77979-133">C#</span><span class="sxs-lookup"><span data-stu-id="77979-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77979-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77979-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77979-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77979-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77979-136">Java</span><span class="sxs-lookup"><span data-stu-id="77979-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisesagent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77979-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="77979-137">Response</span></span>

<span data-ttu-id="77979-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="77979-138">The following is an example of the response.</span></span>

> <span data-ttu-id="77979-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="77979-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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



