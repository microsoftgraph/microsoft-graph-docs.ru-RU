---
title: Список Акцессревиевинстанце
description: Получение объектов Акцессревиевинстанце.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 844564c383b065adc80672cad727807cbb590ca7
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001011"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="0244d-103">Список Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="0244d-103">List accessReviewInstance</span></span>

<span data-ttu-id="0244d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0244d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0244d-105">Получение объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) для определенного [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0244d-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="0244d-106">Возвращается список из нуля или более объектов **акцессревиевинстанце** , включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="0244d-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="0244d-107">Возвращенные объекты не включают связанные АкцессревиевинстанцедеЦисионитемс.</span><span class="sxs-lookup"><span data-stu-id="0244d-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="0244d-108">Чтобы получить решения для экземпляра, используйте [List акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="0244d-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="0244d-109">Если возвращается множество **акцессревиевинстанцес** , чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на страницы, включив в него как параметр запроса $Top, который содержит не более 100, и параметр запроса $Skip = 0 в запросе.</span><span class="sxs-lookup"><span data-stu-id="0244d-109">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="0244d-110">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу с помощью свойства @odata. nextLink в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="0244d-110">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="0244d-111">При наличии этого свойства Продолжайте делать дополнительные запросы с URL-адресом @odata. nextLink в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе разбиение данных Microsoft Graph в приложении.</span><span class="sxs-lookup"><span data-stu-id="0244d-111">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="0244d-112">Если не указано ни одного параметра запроса и число результатов превышает 100, Microsoft Graph автоматически разбивать результаты на страницы 100 на каждой странице.</span><span class="sxs-lookup"><span data-stu-id="0244d-112">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="0244d-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0244d-113">Permissions</span></span>
<span data-ttu-id="0244d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0244d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0244d-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0244d-116">Permission type</span></span>                        | <span data-ttu-id="0244d-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0244d-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0244d-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0244d-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="0244d-119">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0244d-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="0244d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0244d-120">Application</span></span>                            | <span data-ttu-id="0244d-121">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0244d-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="0244d-122">Вошедшего в систему пользователя также должен находиться в роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="0244d-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="0244d-123">Чтобы просмотреть только те экземпляры, для которых пользователь, вошедшего в систему, назначен проверяющему, ознакомьтесь со статьей [Просмотр списка ожидающих доступных экземпляров](accessreviewinstance-pendingaccessreviewinstances.md)</span><span class="sxs-lookup"><span data-stu-id="0244d-123">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="0244d-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0244d-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a><span data-ttu-id="0244d-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0244d-125">Request headers</span></span>
<span data-ttu-id="0244d-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="0244d-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="0244d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0244d-127">Request body</span></span>
<span data-ttu-id="0244d-128">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="0244d-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0244d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0244d-129">Response</span></span>
<span data-ttu-id="0244d-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0244d-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0244d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0244d-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0244d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0244d-132">Request</span></span>
<span data-ttu-id="0244d-133">В приведенном ниже примере показан запрос на получение всех экземпляров проверки доступа для определения.</span><span class="sxs-lookup"><span data-stu-id="0244d-133">The following example shows a request to retrieve all the access review instances for a definition.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances?$top=100&$skip=0
```

### <a name="response"></a><span data-ttu-id="0244d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0244d-134">Response</span></span>
><span data-ttu-id="0244d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0244d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
            "startDateTime": "2020-09-21T20:03:36Z",
            "endDateTime": "2020-09-23T20:03:36Z",
            "status": "NotStarted",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        },
        {
            "id": "64444761-b89f-4d9c-afb9-fcfc8bb9cf45",
            "startDateTime": "2020-09-14T20:03:36.74Z",
            "endDateTime": "2020-09-16T20:03:36.74Z",
            "status": "Completed",
            "scope": {
                "query": "/groups/b7a04444-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="0244d-137">См. также</span><span class="sxs-lookup"><span data-stu-id="0244d-137">See also</span></span>

- [<span data-ttu-id="0244d-138">Список Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="0244d-138">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="0244d-139">Получение Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="0244d-139">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
