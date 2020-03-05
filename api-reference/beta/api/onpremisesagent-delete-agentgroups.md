---
title: Удаление Онпремисесажент из Онпремисесажентграуп
description: Удаление Онпремисесажент из Онпремисесажентграуп.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 76462a4b998f29db1eb43b3cca2618b1db4b4fa2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456518"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="9f430-103">Удаление Онпремисесажент из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="9f430-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

<span data-ttu-id="9f430-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9f430-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f430-105">Удаление [онпремисесажент](../resources/onpremisesagent.md) из [онпремисесажентграуп](../resources/onpremisesagentgroup.md).</span><span class="sxs-lookup"><span data-stu-id="9f430-105">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f430-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f430-106">Permissions</span></span>

<span data-ttu-id="9f430-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f430-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f430-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f430-109">Permission type</span></span>                        | <span data-ttu-id="9f430-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f430-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f430-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f430-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f430-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f430-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9f430-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f430-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f430-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f430-114">Not supported.</span></span> |
| <span data-ttu-id="9f430-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f430-115">Application</span></span>                            | <span data-ttu-id="9f430-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f430-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f430-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f430-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9f430-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f430-118">Request headers</span></span>

| <span data-ttu-id="9f430-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f430-119">Name</span></span>          | <span data-ttu-id="9f430-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9f430-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9f430-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f430-121">Authorization</span></span> | <span data-ttu-id="9f430-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9f430-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f430-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f430-123">Request body</span></span>

<span data-ttu-id="9f430-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f430-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f430-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f430-125">Response</span></span>

<span data-ttu-id="9f430-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f430-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f430-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f430-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f430-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f430-129">Request</span></span>

<span data-ttu-id="9f430-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f430-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f430-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f430-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="9f430-132">C#</span><span class="sxs-lookup"><span data-stu-id="9f430-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f430-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f430-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f430-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f430-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f430-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f430-135">Response</span></span>

<span data-ttu-id="9f430-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9f430-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
