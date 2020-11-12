---
title: Список Акцессревиевсчедуледефинитионс
description: Получение объектов Акцессревиевсчедуледефинитион.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3d073dbf0b6f2bdb17fb9649596c6ee04332d81c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000986"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="f2c31-103">Список Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="f2c31-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="f2c31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c31-105">Получение объектов [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f2c31-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="f2c31-106">Возвращается список из нуля или более объектов Акцессревиевсчедуледефинитион, включая все вложенные свойства для каждой созданной серии проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="f2c31-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="f2c31-107">Это не относится к связанным Акцессревиевинстанцес.</span><span class="sxs-lookup"><span data-stu-id="f2c31-107">This does not include associated accessReviewInstances.</span></span>

>[!NOTE]
><span data-ttu-id="f2c31-108">Если возвращается множество **акцессревиевсчедуледефинитионс** , чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на страницы, включив в него как параметр запроса $Top, который содержит не более 100, и параметр запроса $Skip = 0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="f2c31-108">If many **accessReviewScheduleDefinitions** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="f2c31-109">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с помощью свойства @odata. nextLink в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="f2c31-109">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="f2c31-110">При наличии этого свойства Продолжайте делать дополнительные запросы с URL-адресом @odata. nextLink в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе разбиение данных Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="f2c31-110">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="f2c31-111">Если не указано ни одного параметра запроса и число результатов превышает 100, Microsoft Graph автоматически разбивать результаты на страницы 100 на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="f2c31-111">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>


## <a name="permissions"></a><span data-ttu-id="f2c31-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2c31-112">Permissions</span></span>
<span data-ttu-id="f2c31-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2c31-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c31-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2c31-115">Permission type</span></span>                        | <span data-ttu-id="f2c31-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2c31-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2c31-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2c31-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2c31-118">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2c31-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="f2c31-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2c31-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2c31-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2c31-120">Not supported.</span></span>|
|<span data-ttu-id="f2c31-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2c31-121">Application</span></span>                            | <span data-ttu-id="f2c31-122">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2c31-122">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="f2c31-123">Вошедшего в систему пользователя также должен находиться в роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="f2c31-123">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="f2c31-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2c31-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="f2c31-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2c31-125">Request headers</span></span>
<span data-ttu-id="f2c31-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="f2c31-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="f2c31-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2c31-127">Request body</span></span>
<span data-ttu-id="f2c31-128">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="f2c31-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="f2c31-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2c31-129">Response</span></span>
<span data-ttu-id="f2c31-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2c31-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2c31-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2c31-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f2c31-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2c31-132">Request</span></span>
<span data-ttu-id="f2c31-133">В приведенном ниже примере показан запрос на получение всех рядов проверки доступа в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f2c31-133">The following example shows a request to retrieve all the access review series in a tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
---

### <a name="response"></a><span data-ttu-id="f2c31-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2c31-134">Response</span></span>
><span data-ttu-id="f2c31-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2c31-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "createdDateTime": "2020-09-09T14:27:59Z",
            "lastModifiedDateTime": "2020-09-11T12:02:50Z",
            "status": "InProgress",
            "descriptionForAdmins": "",
            "descriptionForReviewers": "",
            "createdBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@microsoft.com"
            },
            "scope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
                }
            ],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": false,
                "defaultDecision": "None",
                "instanceDurationInDays": 0,
                "autoApplyDecisionsEnabled": false,
                "recommendationsEnabled": true,
                "recurrence": {
                    "pattern": {
                        "type": "weekly",
                        "interval": 1,
                        "month": 0,
                        "dayOfMonth": 0,
                        "daysOfWeek": [],
                        "firstDayOfWeek": "sunday",
                        "index": "first"
                    },
                    "range": {
                        "type": "numbered",
                        "numberOfOccurrences": 0,
                        "recurrenceTimeZone": null,
                        "startDate": "2020-09-11",
                        "endDate": "9999-12-31"
                    }
                }
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="f2c31-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f2c31-137">See also</span></span>

- [<span data-ttu-id="f2c31-138">Получение Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="f2c31-138">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
