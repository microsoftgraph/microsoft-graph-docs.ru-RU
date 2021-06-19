---
title: Остановка accessReviewInstance
description: Остановите активный в настоящее время accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c59b08c3a451d54a03502b28d2f05350f38e126f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030490"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="3409a-103">Остановка accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="3409a-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="3409a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3409a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3409a-105">Остановите активный в настоящее [время accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="3409a-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="3409a-106">После остановки экземпляра проверки доступа состояние экземпляра будет, рецензенты больше не могут давать входные данные, а решения о проверке доступа могут `Completed` применяться.</span><span class="sxs-lookup"><span data-stu-id="3409a-106">After the access review instance stops, the instance status will be `Completed`, the reviewers can no longer give input, and the access review decisions can be applied.</span></span>

<span data-ttu-id="3409a-107">Остановка экземпляра не влияет на будущие экземпляры.</span><span class="sxs-lookup"><span data-stu-id="3409a-107">Stopping an instance will not effect future instances.</span></span> <span data-ttu-id="3409a-108">Чтобы предотвратить повторный обзор доступа при [](accessreviewscheduledefinition-update.md) запуске будущих экземпляров, обнови определение расписания, чтобы изменить запланированную дату окончания.</span><span class="sxs-lookup"><span data-stu-id="3409a-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="3409a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3409a-109">Permissions</span></span>
<span data-ttu-id="3409a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3409a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3409a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3409a-112">Permission type</span></span>                        | <span data-ttu-id="3409a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3409a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3409a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3409a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3409a-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3409a-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="3409a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3409a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3409a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3409a-117">Not supported.</span></span>|
|<span data-ttu-id="3409a-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="3409a-118">Application</span></span>                            | <span data-ttu-id="3409a-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3409a-119">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3409a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3409a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="3409a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3409a-121">Request headers</span></span>
<span data-ttu-id="3409a-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="3409a-122">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="3409a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3409a-123">Request body</span></span>
<span data-ttu-id="3409a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3409a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3409a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3409a-125">Response</span></span>
<span data-ttu-id="3409a-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3409a-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3409a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3409a-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="3409a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3409a-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3409a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3409a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="3409a-131">C#</span><span class="sxs-lookup"><span data-stu-id="3409a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3409a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3409a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3409a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3409a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3409a-134">Java</span><span class="sxs-lookup"><span data-stu-id="3409a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="3409a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3409a-135">Response</span></span>
><span data-ttu-id="3409a-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3409a-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
