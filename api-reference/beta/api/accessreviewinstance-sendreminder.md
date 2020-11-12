---
title: 'Акцессревиевинстанце: Сендреминдер'
description: Отправляет напоминание рецензентам текущего активного Акцессревиевинстанце.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a31cf197cd8df1f806d5c9ead2b57903d632f1dc
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001018"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="10265-103">Акцессревиевинстанце: Сендреминдер</span><span class="sxs-lookup"><span data-stu-id="10265-103">accessReviewInstance: sendReminder</span></span>

<span data-ttu-id="10265-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10265-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10265-105">Отправка напоминания рецензентам, которые активны в настоящее время [акцессревиевинстанце](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="10265-105">Send a reminder to the reviewers of a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10265-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10265-106">Permissions</span></span>
<span data-ttu-id="10265-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10265-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10265-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10265-109">Permission type</span></span>                        | <span data-ttu-id="10265-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10265-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="10265-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10265-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10265-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10265-112">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="10265-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10265-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10265-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10265-114">Not supported.</span></span>|
|<span data-ttu-id="10265-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10265-115">Application</span></span>                            | <span data-ttu-id="10265-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10265-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10265-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10265-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definitionId}/instances/{instanceId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="10265-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10265-118">Request headers</span></span>
<span data-ttu-id="10265-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="10265-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="10265-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10265-120">Request body</span></span>
<span data-ttu-id="10265-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10265-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10265-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="10265-122">Response</span></span>
<span data-ttu-id="10265-p102">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10265-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10265-125">Примеры</span><span class="sxs-lookup"><span data-stu-id="10265-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="10265-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="10265-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder
```

---

### <a name="response"></a><span data-ttu-id="10265-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="10265-127">Response</span></span>
><span data-ttu-id="10265-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10265-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
