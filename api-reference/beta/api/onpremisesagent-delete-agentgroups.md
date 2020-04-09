---
title: Удаление Онпремисесажент из Онпремисесажентграуп
description: Удаление Онпремисесажент из Онпремисесажентграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53994f70dd4102468f1321f2425a1794e69d9e3f
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199566"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="83481-103">Удаление Онпремисесажент из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="83481-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

<span data-ttu-id="83481-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83481-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83481-105">Удаление [онпремисесажент](../resources/onpremisesagent.md) из [онпремисесажентграуп](../resources/onpremisesagentgroup.md).</span><span class="sxs-lookup"><span data-stu-id="83481-105">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83481-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83481-106">Permissions</span></span>

<span data-ttu-id="83481-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83481-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83481-109">Permission type</span></span>                        | <span data-ttu-id="83481-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83481-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="83481-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83481-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83481-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83481-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="83481-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83481-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83481-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83481-114">Not supported.</span></span> |
| <span data-ttu-id="83481-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83481-115">Application</span></span>                            | <span data-ttu-id="83481-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83481-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83481-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83481-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="83481-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83481-118">Request headers</span></span>

| <span data-ttu-id="83481-119">Имя</span><span class="sxs-lookup"><span data-stu-id="83481-119">Name</span></span>          | <span data-ttu-id="83481-120">Описание</span><span class="sxs-lookup"><span data-stu-id="83481-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="83481-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83481-121">Authorization</span></span> | <span data-ttu-id="83481-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="83481-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="83481-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83481-123">Request body</span></span>

<span data-ttu-id="83481-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83481-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83481-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="83481-125">Response</span></span>

<span data-ttu-id="83481-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="83481-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83481-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="83481-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83481-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="83481-129">Request</span></span>

<span data-ttu-id="83481-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83481-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83481-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="83481-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="83481-132">C#</span><span class="sxs-lookup"><span data-stu-id="83481-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83481-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83481-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83481-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83481-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="83481-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="83481-135">Response</span></span>

<span data-ttu-id="83481-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="83481-136">The following is an example of the response.</span></span>

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
