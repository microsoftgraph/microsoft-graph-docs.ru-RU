---
title: Список onPremisesAgents
description: Извлечение списка onPremisesAgents.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 31a9077b1c9b3c53f516f55532dab741fbef3ff7
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781158"
---
# <a name="list-onpremisesagents"></a><span data-ttu-id="b0e63-103">Список onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="b0e63-103">List onPremisesAgents</span></span>

<span data-ttu-id="b0e63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0e63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0e63-105">Извлечение списка [объектов onPremisesAgent.](../resources/onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="b0e63-105">Retrieve a list of [onPremisesAgent](../resources/onpremisesagent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0e63-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0e63-106">Permissions</span></span>

<span data-ttu-id="b0e63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0e63-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0e63-109">Permission type</span></span>                        | <span data-ttu-id="b0e63-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0e63-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="b0e63-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0e63-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0e63-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e63-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="b0e63-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0e63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0e63-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0e63-114">Not supported.</span></span> |
| <span data-ttu-id="b0e63-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0e63-115">Application</span></span>                            | <span data-ttu-id="b0e63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0e63-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0e63-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0e63-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /onPremisesPublishingProfiles/{publishingType}/agents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0e63-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0e63-118">Optional query parameters</span></span>

<span data-ttu-id="b0e63-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b0e63-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0e63-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0e63-120">Request headers</span></span>

| <span data-ttu-id="b0e63-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b0e63-121">Name</span></span>      |<span data-ttu-id="b0e63-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0e63-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0e63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0e63-123">Authorization</span></span> | <span data-ttu-id="b0e63-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b0e63-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0e63-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0e63-125">Request body</span></span>

<span data-ttu-id="b0e63-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0e63-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0e63-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0e63-127">Response</span></span>

<span data-ttu-id="b0e63-128">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0e63-128">If successful, this method returns a `200 OK` response code and a collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0e63-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0e63-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0e63-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0e63-130">Request</span></span>

<span data-ttu-id="b0e63-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0e63-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0e63-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0e63-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="b0e63-133">C#</span><span class="sxs-lookup"><span data-stu-id="b0e63-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0e63-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0e63-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0e63-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0e63-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0e63-136">Java</span><span class="sxs-lookup"><span data-stu-id="b0e63-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0e63-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0e63-137">Response</span></span>

<span data-ttu-id="b0e63-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b0e63-138">The following is an example of the response.</span></span>

> <span data-ttu-id="b0e63-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b0e63-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agentGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



