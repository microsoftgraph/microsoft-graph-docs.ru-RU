---
title: Остановка accessReviewInstance
description: Остановите активный в настоящее время accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0655b0acd7dbd32b0ae4aae5337422f26f9c7c96
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048395"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="b5967-103">Остановка accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b5967-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="b5967-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5967-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5967-105">Остановите активный в настоящее [время accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="b5967-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="b5967-106">Чтобы предотвратить повторяющиеся проверки доступа [](accessreviewscheduledefinition-update.md) от запуска будущих экземпляров, обнови его, чтобы изменить запланированную дату окончания.</span><span class="sxs-lookup"><span data-stu-id="b5967-106">To prevent a recurring access review from starting future instances, [update it](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>  <span data-ttu-id="b5967-107">После остановки проверки доступа рецензенты больше не могут вводить ввод, и можно применять решения о проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="b5967-107">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5967-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5967-108">Permissions</span></span>
<span data-ttu-id="b5967-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5967-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5967-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5967-111">Permission type</span></span>                        | <span data-ttu-id="b5967-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5967-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5967-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5967-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5967-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5967-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b5967-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5967-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5967-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5967-116">Not supported.</span></span>|
|<span data-ttu-id="b5967-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b5967-117">Application</span></span>                            | <span data-ttu-id="b5967-118">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5967-118">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5967-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5967-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="b5967-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5967-120">Request headers</span></span>
<span data-ttu-id="b5967-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b5967-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="b5967-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5967-122">Request body</span></span>
<span data-ttu-id="b5967-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5967-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5967-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5967-124">Response</span></span>
<span data-ttu-id="b5967-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5967-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5967-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5967-127">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b5967-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5967-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b5967-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5967-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="b5967-130">C#</span><span class="sxs-lookup"><span data-stu-id="b5967-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5967-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5967-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5967-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5967-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5967-133">Java</span><span class="sxs-lookup"><span data-stu-id="b5967-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="b5967-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5967-134">Response</span></span>
><span data-ttu-id="b5967-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b5967-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Stop accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
