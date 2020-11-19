---
title: Удаление Акцессревиевсчедуледефинитион
description: Удаление объекта Акцессревиевсчедуледефинитион.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93d61dd2b903014ee92f41929e1cb4ad13f05b50
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214267"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="54627-103">Удаление Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="54627-103">Delete accessReviewScheduleDefinition</span></span>

<span data-ttu-id="54627-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54627-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54627-105">Удаление объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="54627-105">Delete an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="54627-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54627-106">Permissions</span></span>
<span data-ttu-id="54627-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54627-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54627-109">Permission type</span></span>                        | <span data-ttu-id="54627-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54627-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="54627-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54627-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54627-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54627-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="54627-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54627-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54627-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54627-114">Not supported.</span></span>|
|<span data-ttu-id="54627-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="54627-115">Application</span></span>                            | <span data-ttu-id="54627-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54627-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54627-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54627-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="54627-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54627-118">Request headers</span></span>
<span data-ttu-id="54627-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="54627-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="54627-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54627-120">Request body</span></span>
<span data-ttu-id="54627-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54627-121">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="54627-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="54627-122">Response</span></span>
<span data-ttu-id="54627-p102">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="54627-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54627-125">Примеры</span><span class="sxs-lookup"><span data-stu-id="54627-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="54627-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="54627-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="54627-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="54627-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8
```
# <a name="c"></a>[<span data-ttu-id="54627-128">C#</span><span class="sxs-lookup"><span data-stu-id="54627-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54627-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54627-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54627-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54627-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54627-131">Java</span><span class="sxs-lookup"><span data-stu-id="54627-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="54627-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="54627-132">Response</span></span>
><span data-ttu-id="54627-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54627-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
