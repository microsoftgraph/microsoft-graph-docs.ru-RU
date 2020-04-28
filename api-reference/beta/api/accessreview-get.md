---
title: Получение Акцессревиев
description: В функции рецензирования Access Azure AD извлеките объект Акцессревиев.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b363c2f3be60bd782e6b0524e99b846b2ace9752
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123540"
---
# <a name="get-accessreview"></a><span data-ttu-id="30030-103">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="30030-103">Get accessReview</span></span>

<span data-ttu-id="30030-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30030-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30030-105">В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD извлеките объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="30030-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="30030-106">Чтобы получить рецензентов проверки доступа, используйте API [List акцессревиев проверяющих](accessreview-listreviewers.md) .</span><span class="sxs-lookup"><span data-stu-id="30030-106">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="30030-107">Чтобы получить решение об анализе доступа, используйте API [List акцессревиев решений](accessreview-listdecisions.md) или [перечислите мои API решений акцессревиев](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="30030-107">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="30030-108">Если эта проверка доступа повторяется, то решения не будут связаны с серией проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="30030-108">If this is a recurring access review, no decisions will be associated with the recurring access review series.</span></span> <span data-ttu-id="30030-109">Вместо этого используйте `instances` связь этого ряда для получения коллекции [акцессревиев](../resources/accessreview.md) из прошлых, текущих и будущих экземпляров проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="30030-109">Instead, use the `instances` relationship of that series to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span> <span data-ttu-id="30030-110">Все прошедшие и текущие экземпляры будут принимать решения.</span><span class="sxs-lookup"><span data-stu-id="30030-110">Each past and current instance will have decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="30030-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30030-111">Permissions</span></span>
<span data-ttu-id="30030-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30030-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30030-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30030-114">Permission type</span></span>                        | <span data-ttu-id="30030-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30030-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="30030-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30030-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="30030-117">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="30030-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="30030-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30030-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30030-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30030-119">Not supported.</span></span> |
|<span data-ttu-id="30030-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30030-120">Application</span></span>                            | <span data-ttu-id="30030-121">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="30030-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="30030-122">Чтобы вызвать этот API, пользователь, вошедшего в систему, должен быть включен в роль каталога, которая разрешает им читать проверку доступа, или пользователь может быть назначен в качестве проверяющего при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="30030-122">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="30030-123">Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="30030-123">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="30030-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30030-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="30030-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30030-125">Request headers</span></span>
| <span data-ttu-id="30030-126">Имя</span><span class="sxs-lookup"><span data-stu-id="30030-126">Name</span></span>         | <span data-ttu-id="30030-127">Тип</span><span class="sxs-lookup"><span data-stu-id="30030-127">Type</span></span>        | <span data-ttu-id="30030-128">Описание</span><span class="sxs-lookup"><span data-stu-id="30030-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="30030-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="30030-129">Authorization</span></span> | <span data-ttu-id="30030-130">string</span><span class="sxs-lookup"><span data-stu-id="30030-130">string</span></span> | <span data-ttu-id="30030-p105">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30030-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30030-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30030-133">Request body</span></span>
<span data-ttu-id="30030-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30030-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30030-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="30030-135">Response</span></span>
<span data-ttu-id="30030-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30030-136">If successful, this method returns a `200 OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30030-137">Пример</span><span class="sxs-lookup"><span data-stu-id="30030-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30030-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="30030-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="30030-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="30030-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="30030-140">C#</span><span class="sxs-lookup"><span data-stu-id="30030-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30030-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30030-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30030-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30030-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="30030-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="30030-143">Response</span></span>
><span data-ttu-id="30030-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30030-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="30030-146">См. также</span><span class="sxs-lookup"><span data-stu-id="30030-146">See also</span></span>

- [<span data-ttu-id="30030-147">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="30030-147">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="30030-148">Список Акцессревиевс</span><span class="sxs-lookup"><span data-stu-id="30030-148">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="30030-149">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="30030-149">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="30030-150">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="30030-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="30030-151">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="30030-151">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="30030-152">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="30030-152">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


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
