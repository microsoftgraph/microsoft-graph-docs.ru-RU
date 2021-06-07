---
title: SendReminder accessReview
description: 'В функции обзоров доступа Azure AD отправьте напоминание рецензентам активного в настоящее время accessReview.  Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа. '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6796fcc52473d2e45be7c594ee4bce010a9d19e7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751024"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="b72d3-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="b72d3-104">SendReminder accessReview</span></span>

<span data-ttu-id="b72d3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b72d3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b72d3-106">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) отправьте напоминание рецензентам активного в настоящее время [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="b72d3-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="b72d3-107">Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="b72d3-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b72d3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b72d3-108">Permissions</span></span>
<span data-ttu-id="b72d3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b72d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b72d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b72d3-111">Permission type</span></span>                        | <span data-ttu-id="b72d3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b72d3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b72d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b72d3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b72d3-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b72d3-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b72d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b72d3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b72d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b72d3-116">Not supported.</span></span> |
|<span data-ttu-id="b72d3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b72d3-117">Application</span></span>                            | <span data-ttu-id="b72d3-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="b72d3-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="b72d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b72d3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="b72d3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b72d3-120">Request headers</span></span>
| <span data-ttu-id="b72d3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b72d3-121">Name</span></span>         | <span data-ttu-id="b72d3-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b72d3-122">Type</span></span>        | <span data-ttu-id="b72d3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b72d3-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b72d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b72d3-124">Authorization</span></span> | <span data-ttu-id="b72d3-125">string</span><span class="sxs-lookup"><span data-stu-id="b72d3-125">string</span></span> | <span data-ttu-id="b72d3-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b72d3-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b72d3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b72d3-128">Request body</span></span>
<span data-ttu-id="b72d3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b72d3-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b72d3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b72d3-130">Response</span></span>
<span data-ttu-id="b72d3-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b72d3-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b72d3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b72d3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b72d3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b72d3-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b72d3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b72d3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_1"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="b72d3-136">C#</span><span class="sxs-lookup"><span data-stu-id="b72d3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b72d3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b72d3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b72d3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b72d3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b72d3-139">Java</span><span class="sxs-lookup"><span data-stu-id="b72d3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b72d3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b72d3-140">Response</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


