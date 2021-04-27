---
title: Получить accessReview
description: В функции обзоров доступа Azure AD извлекаем объект accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 01bf052e6e77377c5ec07eddfc005b1a05394106
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048500"
---
# <a name="get-accessreview"></a><span data-ttu-id="88223-103">Получить accessReview</span><span class="sxs-lookup"><span data-stu-id="88223-103">Get accessReview</span></span>

<span data-ttu-id="88223-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88223-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88223-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) извлекаем [объект accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="88223-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="88223-106">Для получения рецензентов обзора доступа используйте API [рецензентов списка accessReview.](accessreview-listreviewers.md)</span><span class="sxs-lookup"><span data-stu-id="88223-106">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="88223-107">Чтобы получить решения обзора доступа, используйте API решений [accessReview](accessreview-listdecisions.md) или список API решений [accessReview.](accessreview-listmydecisions.md)</span><span class="sxs-lookup"><span data-stu-id="88223-107">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="88223-108">Если это повторяющийся обзор доступа, никакие решения не будут связаны с повторяющимися сериями обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="88223-108">If this is a recurring access review, no decisions will be associated with the recurring access review series.</span></span> <span data-ttu-id="88223-109">Вместо этого используйте связь этой серии для получения `instances` [коллекции accessReview](../resources/accessreview.md) прошлых, текущих и будущих экземпляров обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="88223-109">Instead, use the `instances` relationship of that series to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span> <span data-ttu-id="88223-110">Каждый прошлый и текущий экземпляр будут иметь решения.</span><span class="sxs-lookup"><span data-stu-id="88223-110">Each past and current instance will have decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="88223-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88223-111">Permissions</span></span>
<span data-ttu-id="88223-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88223-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88223-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88223-114">Permission type</span></span>                        | <span data-ttu-id="88223-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88223-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="88223-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88223-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="88223-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88223-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="88223-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88223-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88223-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88223-119">Not supported.</span></span> |
|<span data-ttu-id="88223-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="88223-120">Application</span></span>                            | <span data-ttu-id="88223-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="88223-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="88223-122">Чтобы вызвать этот API, подписанный пользователем должен также быть в роли каталога, который позволяет ему читать обзор доступа, или пользователь может быть назначен в качестве рецензента в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="88223-122">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="88223-123">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviews-root.md)</span><span class="sxs-lookup"><span data-stu-id="88223-123">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="88223-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88223-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="88223-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88223-125">Request headers</span></span>
| <span data-ttu-id="88223-126">Имя</span><span class="sxs-lookup"><span data-stu-id="88223-126">Name</span></span>         | <span data-ttu-id="88223-127">Тип</span><span class="sxs-lookup"><span data-stu-id="88223-127">Type</span></span>        | <span data-ttu-id="88223-128">Описание</span><span class="sxs-lookup"><span data-stu-id="88223-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="88223-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="88223-129">Authorization</span></span> | <span data-ttu-id="88223-130">string</span><span class="sxs-lookup"><span data-stu-id="88223-130">string</span></span> | <span data-ttu-id="88223-p105">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88223-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88223-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88223-133">Request body</span></span>
<span data-ttu-id="88223-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88223-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88223-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="88223-135">Response</span></span>
<span data-ttu-id="88223-136">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект accessReview](../resources/accessreview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="88223-136">If successful, this method returns a `200 OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88223-137">Пример</span><span class="sxs-lookup"><span data-stu-id="88223-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88223-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="88223-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88223-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="88223-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="88223-140">C#</span><span class="sxs-lookup"><span data-stu-id="88223-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88223-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88223-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88223-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88223-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88223-143">Java</span><span class="sxs-lookup"><span data-stu-id="88223-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="88223-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="88223-144">Response</span></span>
><span data-ttu-id="88223-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="88223-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="88223-146">См. также</span><span class="sxs-lookup"><span data-stu-id="88223-146">See also</span></span>

- [<span data-ttu-id="88223-147">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="88223-147">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="88223-148">AccessReviews списка</span><span class="sxs-lookup"><span data-stu-id="88223-148">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="88223-149">List programControls</span><span class="sxs-lookup"><span data-stu-id="88223-149">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="88223-150">Рецензенты списка accessReview</span><span class="sxs-lookup"><span data-stu-id="88223-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="88223-151">Списки решений accessReview</span><span class="sxs-lookup"><span data-stu-id="88223-151">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="88223-152">Список решений accessReview</span><span class="sxs-lookup"><span data-stu-id="88223-152">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


