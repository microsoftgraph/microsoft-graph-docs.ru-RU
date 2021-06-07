---
title: Остановка accessReview
description: В функции обзоров доступа Azure AD остановите активный accessReview.  Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.  (Чтобы повторный обзор доступа не запускал будущие экземпляры, обнови его, чтобы изменить запланированную дату окончания).  После остановки проверки доступа рецензенты больше не могут вводить ввод, и можно применять решения о проверке доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9ca0dffdc48e059e303e05afac791a8d431f5600
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751017"
---
# <a name="stop-accessreview"></a><span data-ttu-id="fefa1-106">Остановка accessReview</span><span class="sxs-lookup"><span data-stu-id="fefa1-106">Stop accessReview</span></span>

<span data-ttu-id="fefa1-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fefa1-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fefa1-108">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) остановите активный [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="fefa1-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="fefa1-109">Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="fefa1-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="fefa1-110">(Чтобы повторный обзор доступа не запускал [](accessreview-update.md) будущие экземпляры, обнови его, чтобы изменить запланированную дату окончания).</span><span class="sxs-lookup"><span data-stu-id="fefa1-110">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="fefa1-111">После остановки проверки доступа рецензенты больше не могут вводить ввод, и можно применять решения о проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="fefa1-111">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="fefa1-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fefa1-112">Permissions</span></span>
<span data-ttu-id="fefa1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fefa1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fefa1-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fefa1-115">Permission type</span></span>                        | <span data-ttu-id="fefa1-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fefa1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fefa1-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fefa1-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="fefa1-118">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fefa1-118">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="fefa1-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fefa1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fefa1-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fefa1-120">Not supported.</span></span> |
|<span data-ttu-id="fefa1-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="fefa1-121">Application</span></span>                            | <span data-ttu-id="fefa1-122">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="fefa1-122">AccessReview.ReadWrite.Membership</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fefa1-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fefa1-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/stop
```
## <a name="request-headers"></a><span data-ttu-id="fefa1-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fefa1-124">Request headers</span></span>
| <span data-ttu-id="fefa1-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fefa1-125">Name</span></span>         | <span data-ttu-id="fefa1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fefa1-126">Type</span></span>        | <span data-ttu-id="fefa1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fefa1-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fefa1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="fefa1-128">Authorization</span></span> | <span data-ttu-id="fefa1-129">string</span><span class="sxs-lookup"><span data-stu-id="fefa1-129">string</span></span> | <span data-ttu-id="fefa1-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fefa1-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fefa1-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fefa1-132">Request body</span></span>
<span data-ttu-id="fefa1-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fefa1-133">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fefa1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fefa1-134">Response</span></span>
<span data-ttu-id="fefa1-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fefa1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fefa1-137">Пример</span><span class="sxs-lookup"><span data-stu-id="fefa1-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fefa1-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="fefa1-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fefa1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="fefa1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="c"></a>[<span data-ttu-id="fefa1-140">C#</span><span class="sxs-lookup"><span data-stu-id="fefa1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fefa1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fefa1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fefa1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fefa1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fefa1-143">Java</span><span class="sxs-lookup"><span data-stu-id="fefa1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fefa1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fefa1-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


