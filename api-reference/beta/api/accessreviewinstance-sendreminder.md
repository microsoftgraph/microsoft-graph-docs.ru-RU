---
title: 'accessReviewInstance: sendReminder'
description: Отправляет напоминание рецензентам активного доступаReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 20e662e0501091b4482c44450f4223ed5d39a95a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048409"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="9c911-103">accessReviewInstance: sendReminder</span><span class="sxs-lookup"><span data-stu-id="9c911-103">accessReviewInstance: sendReminder</span></span>

<span data-ttu-id="9c911-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c911-105">Отправьте напоминание рецензентам активного в настоящее время [accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="9c911-105">Send a reminder to the reviewers of a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c911-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c911-106">Permissions</span></span>
<span data-ttu-id="9c911-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c911-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c911-109">Permission type</span></span>                        | <span data-ttu-id="9c911-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c911-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c911-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c911-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c911-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c911-112">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9c911-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c911-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c911-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c911-114">Not supported.</span></span>|
|<span data-ttu-id="9c911-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9c911-115">Application</span></span>                            | <span data-ttu-id="9c911-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c911-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c911-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c911-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definitionId}/instances/{instanceId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="9c911-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c911-118">Request headers</span></span>
<span data-ttu-id="9c911-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c911-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="9c911-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c911-120">Request body</span></span>
<span data-ttu-id="9c911-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c911-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c911-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c911-122">Response</span></span>
<span data-ttu-id="9c911-p102">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9c911-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c911-125">Примеры</span><span class="sxs-lookup"><span data-stu-id="9c911-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="9c911-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c911-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9c911-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c911-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_2"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="9c911-128">C#</span><span class="sxs-lookup"><span data-stu-id="9c911-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c911-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c911-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c911-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c911-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c911-131">Java</span><span class="sxs-lookup"><span data-stu-id="9c911-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="9c911-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c911-132">Response</span></span>
><span data-ttu-id="9c911-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9c911-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "SendReminder accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
