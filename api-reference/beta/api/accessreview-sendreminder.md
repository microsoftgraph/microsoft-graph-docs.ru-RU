---
title: Сендреминдер Акцессревиев
description: 'В функции рецензирования Access Azure AD отправьте напоминание рецензентам, которые активны в настоящее время Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1314ffa567aedfe615e9d24f27acb04f22b0c010
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408771"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="b0da8-104">Сендреминдер Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="b0da8-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0da8-105">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD отправьте напоминание рецензентам, которые активны в настоящее время [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="b0da8-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="b0da8-106">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="b0da8-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b0da8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0da8-107">Permissions</span></span>
<span data-ttu-id="b0da8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0da8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0da8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0da8-110">Permission type</span></span>                        | <span data-ttu-id="b0da8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0da8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0da8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0da8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0da8-113">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b0da8-113">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b0da8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0da8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0da8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0da8-115">Not supported.</span></span> |
|<span data-ttu-id="b0da8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0da8-116">Application</span></span>                            | <span data-ttu-id="b0da8-117">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="b0da8-117">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0da8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0da8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="b0da8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0da8-119">Request headers</span></span>
| <span data-ttu-id="b0da8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b0da8-120">Name</span></span>         | <span data-ttu-id="b0da8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b0da8-121">Type</span></span>        | <span data-ttu-id="b0da8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0da8-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b0da8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0da8-123">Authorization</span></span> | <span data-ttu-id="b0da8-124">string</span><span class="sxs-lookup"><span data-stu-id="b0da8-124">string</span></span> | <span data-ttu-id="b0da8-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0da8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0da8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0da8-127">Request body</span></span>
<span data-ttu-id="b0da8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0da8-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b0da8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0da8-129">Response</span></span>
<span data-ttu-id="b0da8-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0da8-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0da8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b0da8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0da8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0da8-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0da8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0da8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0da8-135">C#</span><span class="sxs-lookup"><span data-stu-id="b0da8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0da8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0da8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0da8-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0da8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0da8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0da8-138">Response</span></span>
><span data-ttu-id="b0da8-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0da8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
