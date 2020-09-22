---
title: Удаление Онпремисесажентграуп
description: Удаление объекта **онпремисесажентграуп** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e577d25d3dc2e9c6c17186f2ed585b320f1a8e82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017425"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="6e720-103">Удаление Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="6e720-103">Delete onPremisesAgentGroup</span></span>

<span data-ttu-id="6e720-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e720-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e720-105">Удаление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6e720-105">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e720-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e720-106">Permissions</span></span>

<span data-ttu-id="6e720-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e720-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e720-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e720-109">Permission type</span></span>                        | <span data-ttu-id="6e720-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e720-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e720-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e720-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e720-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e720-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6e720-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e720-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e720-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e720-114">Not supported.</span></span> |
| <span data-ttu-id="6e720-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e720-115">Application</span></span>                            | <span data-ttu-id="6e720-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e720-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e720-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e720-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="6e720-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e720-118">Request headers</span></span>

| <span data-ttu-id="6e720-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6e720-119">Name</span></span>          | <span data-ttu-id="6e720-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6e720-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6e720-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e720-121">Authorization</span></span> | <span data-ttu-id="6e720-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6e720-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e720-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e720-123">Request body</span></span>

<span data-ttu-id="6e720-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e720-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e720-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e720-125">Response</span></span>

<span data-ttu-id="6e720-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e720-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e720-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e720-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e720-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e720-129">Request</span></span>

<span data-ttu-id="6e720-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e720-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e720-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e720-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="c"></a>[<span data-ttu-id="6e720-132">C#</span><span class="sxs-lookup"><span data-stu-id="6e720-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e720-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e720-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e720-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e720-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e720-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e720-135">Response</span></span>

<span data-ttu-id="6e720-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6e720-136">The following is an example of the response.</span></span>

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
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


