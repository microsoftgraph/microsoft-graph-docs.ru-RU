---
title: Удаление Публишедресаурце
description: Удаление объекта [публишедресаурце](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74c20ce468392d3dfb380ea9d341f9c0ccf6e9dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454873"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="95216-103">Удаление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="95216-103">Delete publishedResource</span></span>

<span data-ttu-id="95216-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95216-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95216-105">Удаление объекта [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="95216-105">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95216-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95216-106">Permissions</span></span>

<span data-ttu-id="95216-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95216-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95216-109">Permission type</span></span>                        | <span data-ttu-id="95216-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95216-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="95216-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95216-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="95216-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95216-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="95216-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95216-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95216-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95216-114">Not supported.</span></span> |
| <span data-ttu-id="95216-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95216-115">Application</span></span>                            | <span data-ttu-id="95216-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95216-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95216-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95216-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="95216-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95216-118">Request headers</span></span>

| <span data-ttu-id="95216-119">Имя</span><span class="sxs-lookup"><span data-stu-id="95216-119">Name</span></span>          | <span data-ttu-id="95216-120">Описание</span><span class="sxs-lookup"><span data-stu-id="95216-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="95216-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95216-121">Authorization</span></span> | <span data-ttu-id="95216-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="95216-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="95216-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95216-123">Request body</span></span>

<span data-ttu-id="95216-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95216-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95216-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="95216-125">Response</span></span>

<span data-ttu-id="95216-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95216-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95216-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="95216-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="95216-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="95216-129">Request</span></span>

<span data-ttu-id="95216-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95216-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95216-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="95216-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="95216-132">C#</span><span class="sxs-lookup"><span data-stu-id="95216-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95216-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95216-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95216-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95216-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95216-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="95216-135">Response</span></span>

<span data-ttu-id="95216-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="95216-136">The following is an example of the response.</span></span>

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
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
