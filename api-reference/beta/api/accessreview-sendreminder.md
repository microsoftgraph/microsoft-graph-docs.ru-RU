---
title: SendReminder accessReview
description: 'В функции обзоров доступа Azure AD отправьте напоминание рецензентам активного в настоящее время accessReview.  Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа. '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bab89d572bac3df90065693bcb8886f1271b7480
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943120"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="f987e-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="f987e-104">SendReminder accessReview</span></span>

<span data-ttu-id="f987e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f987e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f987e-106">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) отправьте напоминание рецензентам активного в настоящее время [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="f987e-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="f987e-107">Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="f987e-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f987e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f987e-108">Permissions</span></span>
<span data-ttu-id="f987e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f987e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f987e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f987e-111">Permission type</span></span>                        | <span data-ttu-id="f987e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f987e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f987e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f987e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f987e-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f987e-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="f987e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f987e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f987e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f987e-116">Not supported.</span></span> |
|<span data-ttu-id="f987e-117">Application</span><span class="sxs-lookup"><span data-stu-id="f987e-117">Application</span></span>                            | <span data-ttu-id="f987e-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="f987e-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="f987e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f987e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="f987e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f987e-120">Request headers</span></span>
| <span data-ttu-id="f987e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f987e-121">Name</span></span>         | <span data-ttu-id="f987e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f987e-122">Type</span></span>        | <span data-ttu-id="f987e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f987e-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f987e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f987e-124">Authorization</span></span> | <span data-ttu-id="f987e-125">string</span><span class="sxs-lookup"><span data-stu-id="f987e-125">string</span></span> | <span data-ttu-id="f987e-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f987e-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f987e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f987e-128">Request body</span></span>
<span data-ttu-id="f987e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f987e-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f987e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f987e-130">Response</span></span>
<span data-ttu-id="f987e-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f987e-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f987e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f987e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f987e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f987e-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f987e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f987e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_1"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="f987e-136">C#</span><span class="sxs-lookup"><span data-stu-id="f987e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f987e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f987e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f987e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f987e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f987e-139">Java</span><span class="sxs-lookup"><span data-stu-id="f987e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f987e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f987e-140">Response</span></span>
><span data-ttu-id="f987e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f987e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


