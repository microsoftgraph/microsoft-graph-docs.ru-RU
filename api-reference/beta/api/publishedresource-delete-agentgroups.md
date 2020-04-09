---
title: Удаление Публишедресаурце из Онпремисесажентграуп
description: Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e300f57d58dcb0d9b32f17fa603b50df9aeb4c1
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200189"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="0448c-103">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="0448c-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

<span data-ttu-id="0448c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0448c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0448c-105">Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="0448c-105">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0448c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0448c-106">Permissions</span></span>

<span data-ttu-id="0448c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0448c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0448c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0448c-109">Permission type</span></span>                        | <span data-ttu-id="0448c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0448c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="0448c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0448c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0448c-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0448c-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="0448c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0448c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0448c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0448c-114">Not supported.</span></span> |
| <span data-ttu-id="0448c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0448c-115">Application</span></span>                            | <span data-ttu-id="0448c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0448c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0448c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0448c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0448c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0448c-118">Request headers</span></span>

| <span data-ttu-id="0448c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0448c-119">Name</span></span>          | <span data-ttu-id="0448c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0448c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0448c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0448c-121">Authorization</span></span> | <span data-ttu-id="0448c-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0448c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0448c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0448c-123">Request body</span></span>

<span data-ttu-id="0448c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0448c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0448c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="0448c-125">Response</span></span>

<span data-ttu-id="0448c-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0448c-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0448c-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="0448c-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0448c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0448c-128">Request</span></span>

<span data-ttu-id="0448c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0448c-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0448c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0448c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="0448c-131">C#</span><span class="sxs-lookup"><span data-stu-id="0448c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0448c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0448c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0448c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0448c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0448c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0448c-134">Response</span></span>

<span data-ttu-id="0448c-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0448c-135">The following is an example of the response.</span></span>

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
