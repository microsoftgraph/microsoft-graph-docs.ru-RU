---
title: Получить accessReviewInstance
description: Извлечение объекта accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: dffd394e5724a3954324432abccd15f8a9be9318
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048430"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="9b109-103">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9b109-103">Get accessReviewInstance</span></span>

<span data-ttu-id="9b109-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b109-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b109-105">Извлечение [объекта accessReviewInstance](../resources/accessreviewinstance.md) с помощью идентификатора accessReviewInstance и родительского [доступаReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9b109-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="9b109-106">Это возвращает все свойства экземпляра, за исключением связанного [доступаReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b109-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="9b109-107">Чтобы получить решения в экземпляре, используйте [list accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="9b109-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b109-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b109-108">Permissions</span></span>
<span data-ttu-id="9b109-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b109-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b109-111">Permission type</span></span>                        | <span data-ttu-id="9b109-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b109-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b109-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b109-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b109-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b109-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="9b109-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b109-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b109-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b109-116">Not supported.</span></span>|
|<span data-ttu-id="9b109-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9b109-117">Application</span></span>                            | <span data-ttu-id="9b109-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b109-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="9b109-119">Чтобы вызвать этот API, подписанный пользователем должен также быть в роли каталога, который позволяет ему читать обзор доступа, или пользователь может быть назначен в качестве рецензента в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="9b109-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="9b109-120">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="9b109-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="9b109-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b109-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```
## <a name="request-headers"></a><span data-ttu-id="9b109-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b109-122">Request headers</span></span>
<span data-ttu-id="9b109-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b109-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="9b109-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b109-124">Request body</span></span>
<span data-ttu-id="9b109-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b109-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b109-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b109-126">Response</span></span>
<span data-ttu-id="9b109-127">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9b109-127">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b109-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9b109-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="9b109-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b109-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9b109-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b109-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/6af553ce-104d-4842-ab5f-67d7b556e9dd/instances/9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24
```
# <a name="c"></a>[<span data-ttu-id="9b109-131">C#</span><span class="sxs-lookup"><span data-stu-id="9b109-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b109-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b109-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b109-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b109-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b109-134">Java</span><span class="sxs-lookup"><span data-stu-id="9b109-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---



### <a name="response"></a><span data-ttu-id="9b109-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b109-135">Response</span></span>
><span data-ttu-id="9b109-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9b109-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('6af553ce-104d-4842-ab5f-67d7b556e9dd')/instances/$entity",
    "id": "9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24",
    "startDateTime": "2021-03-11T16:44:59.337Z",
    "endDateTime": "2021-06-09T16:44:59.337Z",
    "status": "InProgress",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/97eebd44-61fd-4d42-8b2a-a4de41b6c572/transitiveMembers",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    }
}
```

## <a name="see-also"></a><span data-ttu-id="9b109-137">См. также</span><span class="sxs-lookup"><span data-stu-id="9b109-137">See also</span></span>

- [<span data-ttu-id="9b109-138">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="9b109-138">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="9b109-139">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9b109-139">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
