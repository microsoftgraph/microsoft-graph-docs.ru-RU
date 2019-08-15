---
title: Удаление Публишедресаурце из Онпремисесажентграуп
description: Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d83be65fb44a68a2474ce7a6ed360960c6084a9c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412399"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="1fa35-103">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="1fa35-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fa35-104">Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="1fa35-104">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fa35-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fa35-105">Permissions</span></span>

<span data-ttu-id="1fa35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fa35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fa35-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fa35-108">Permission type</span></span>                        | <span data-ttu-id="1fa35-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fa35-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="1fa35-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fa35-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fa35-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1fa35-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="1fa35-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fa35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fa35-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fa35-113">Not supported.</span></span> |
| <span data-ttu-id="1fa35-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fa35-114">Application</span></span>                            | <span data-ttu-id="1fa35-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fa35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fa35-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fa35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1fa35-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fa35-117">Request headers</span></span>

| <span data-ttu-id="1fa35-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1fa35-118">Name</span></span>          | <span data-ttu-id="1fa35-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa35-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1fa35-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fa35-120">Authorization</span></span> | <span data-ttu-id="1fa35-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1fa35-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fa35-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fa35-122">Request body</span></span>

<span data-ttu-id="1fa35-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fa35-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fa35-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa35-124">Response</span></span>

<span data-ttu-id="1fa35-125">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1fa35-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1fa35-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="1fa35-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1fa35-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fa35-127">Request</span></span>

<span data-ttu-id="1fa35-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fa35-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1fa35-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fa35-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1fa35-130">C#</span><span class="sxs-lookup"><span data-stu-id="1fa35-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fa35-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fa35-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1fa35-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1fa35-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1fa35-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa35-133">Response</span></span>

<span data-ttu-id="1fa35-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1fa35-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
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
