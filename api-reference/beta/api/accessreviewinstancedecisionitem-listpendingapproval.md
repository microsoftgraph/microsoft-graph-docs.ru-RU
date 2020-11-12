---
title: Список ожидающих утверждения АкцессревиевинстанцедеЦисионитем
description: Получение объектов АкцессревиевинстанцедеЦисионитем, ожидающих утверждения вызывающим пользователем.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e245d58966b1fa6e206dff1c7a29f38a3146ac21
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000987"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval"></a><span data-ttu-id="6be2a-103">Список ожидающих утверждения АкцессревиевинстанцедеЦисионитемс</span><span class="sxs-lookup"><span data-stu-id="6be2a-103">List accessReviewInstanceDecisionItems pending approval</span></span>

<span data-ttu-id="6be2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6be2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6be2a-105">Получение объектов [акцессревиевинстанцедеЦисионитем](../resources/accessreviewinstance.md) для определенных [акцессревиевинстанце](../resources/accessreviewscheduledefinition.md) , ожидающих утверждения вызывающим пользователем.</span><span class="sxs-lookup"><span data-stu-id="6be2a-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="6be2a-106">Возвращается список из нуля или более объектов АкцессревиевинстанцедеЦисионитем, включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="6be2a-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="6be2a-107">Если возвращается множество **акцессревиевинстанцедеЦисионитемс** , чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на страницы, включив в него как параметр запроса $Top, который содержит не более 100, и параметр запроса $Skip = 0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="6be2a-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="6be2a-108">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с помощью свойства @odata. nextLink в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="6be2a-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="6be2a-109">При наличии этого свойства Продолжайте делать дополнительные запросы с URL-адресом @odata. nextLink в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе разбиение данных Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="6be2a-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="6be2a-110">Если не указано ни одного параметра запроса и число результатов превышает 100, Microsoft Graph автоматически разбивать результаты на страницы 100 на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="6be2a-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="6be2a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6be2a-111">Permissions</span></span>
<span data-ttu-id="6be2a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6be2a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6be2a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6be2a-114">Permission type</span></span>                        | <span data-ttu-id="6be2a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6be2a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6be2a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6be2a-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6be2a-117">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6be2a-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="6be2a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6be2a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6be2a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be2a-119">Not supported.</span></span>|

<span data-ttu-id="6be2a-120">Кроме того, вошедшего в систему пользователя будут отображаться только те решения, которым назначен проверяющий в инстанце'с Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="6be2a-120">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="6be2a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6be2a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="6be2a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6be2a-122">Request headers</span></span>
<span data-ttu-id="6be2a-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="6be2a-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="6be2a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6be2a-124">Request body</span></span>
<span data-ttu-id="6be2a-125">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="6be2a-125">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="6be2a-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="6be2a-126">Response</span></span>
<span data-ttu-id="6be2a-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиевинстанцедеЦисионитем](../resources/accessreviewinstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6be2a-127">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6be2a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6be2a-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="6be2a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6be2a-129">Request</span></span>
<span data-ttu-id="6be2a-130">В приведенном ниже примере показан запрос на получение всех решений для экземпляра проверки доступа, ожидающей утверждения вызывающего пользователя.</span><span class="sxs-lookup"><span data-stu-id="6be2a-130">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```

---


### <a name="response"></a><span data-ttu-id="6be2a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6be2a-131">Response</span></span>
><span data-ttu-id="6be2a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6be2a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 2,
    "value": [
        {
            "id": "654b34e7-b48f-4772-a2d4-08f1d0dd014c",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "7eae986b-d425-48b2-adf2-3c777f6256f3",
                "userDisplayName": "Adele Vance",
                "userPrincipalName": "AdeleV@microsoft.com"
            }
        },
        {
            "id": "0311dba4-c60c-412e-ac77-14e1da23daf1",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "userDisplayName": "MOD Administrator",
                "userPrincipalName": "admin@microsoft.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="6be2a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="6be2a-134">See also</span></span>

- [<span data-ttu-id="6be2a-135">Получение Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="6be2a-135">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="6be2a-136">Получение Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="6be2a-136">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
