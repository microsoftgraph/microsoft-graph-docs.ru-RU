---
title: Удаление Публишедресаурце из Онпремисесажентграуп
description: Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 667ab45f08ed16abf471f626e0d9f09716f3c34d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342196"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="b85b9-103">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="b85b9-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b85b9-104">Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b85b9-104">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b85b9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b85b9-105">Permissions</span></span>

<span data-ttu-id="b85b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b85b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b85b9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b85b9-108">Permission type</span></span>                        | <span data-ttu-id="b85b9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b85b9-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="b85b9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b85b9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b85b9-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b85b9-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="b85b9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b85b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b85b9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b85b9-113">Not supported.</span></span> |
| <span data-ttu-id="b85b9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b85b9-114">Application</span></span>                            | <span data-ttu-id="b85b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b85b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b85b9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b85b9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b85b9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b85b9-117">Request headers</span></span>

| <span data-ttu-id="b85b9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b85b9-118">Name</span></span>          | <span data-ttu-id="b85b9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b85b9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b85b9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b85b9-120">Authorization</span></span> | <span data-ttu-id="b85b9-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b85b9-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b85b9-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b85b9-122">Request body</span></span>

<span data-ttu-id="b85b9-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b85b9-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b85b9-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="b85b9-124">Response</span></span>

<span data-ttu-id="b85b9-125">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b85b9-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b85b9-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="b85b9-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b85b9-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="b85b9-127">Request</span></span>

<span data-ttu-id="b85b9-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b85b9-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b85b9-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b85b9-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b85b9-130">C#</span><span class="sxs-lookup"><span data-stu-id="b85b9-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b85b9-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b85b9-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b85b9-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b85b9-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b85b9-133">Java</span><span class="sxs-lookup"><span data-stu-id="b85b9-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onpremisesagentgroup-from-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b85b9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b85b9-134">Response</span></span>

<span data-ttu-id="b85b9-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b85b9-135">The following is an example of the response.</span></span>

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
