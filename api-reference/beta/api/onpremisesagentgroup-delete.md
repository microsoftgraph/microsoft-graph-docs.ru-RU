---
title: Удаление Онпремисесажентграуп
description: Удаление объекта **онпремисесажентграуп** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e6a78a79c2eab50cdf035d2c17c4d11637e74b4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414541"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="8dca5-103">Удаление Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="8dca5-103">Delete onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dca5-104">Удаление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8dca5-104">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dca5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8dca5-105">Permissions</span></span>

<span data-ttu-id="8dca5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dca5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dca5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dca5-108">Permission type</span></span>                        | <span data-ttu-id="8dca5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dca5-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dca5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dca5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dca5-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8dca5-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="8dca5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dca5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dca5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dca5-113">Not supported.</span></span> |
| <span data-ttu-id="8dca5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8dca5-114">Application</span></span>                            | <span data-ttu-id="8dca5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dca5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dca5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dca5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="8dca5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dca5-117">Request headers</span></span>

| <span data-ttu-id="8dca5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8dca5-118">Name</span></span>          | <span data-ttu-id="8dca5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8dca5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8dca5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dca5-120">Authorization</span></span> | <span data-ttu-id="8dca5-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8dca5-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dca5-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8dca5-122">Request body</span></span>

<span data-ttu-id="8dca5-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8dca5-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dca5-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dca5-124">Response</span></span>

<span data-ttu-id="8dca5-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8dca5-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dca5-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="8dca5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8dca5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dca5-128">Request</span></span>

<span data-ttu-id="8dca5-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dca5-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8dca5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dca5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8dca5-131">C#</span><span class="sxs-lookup"><span data-stu-id="8dca5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8dca5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dca5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8dca5-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8dca5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8dca5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dca5-134">Response</span></span>

<span data-ttu-id="8dca5-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8dca5-135">The following is an example of the response.</span></span>

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
