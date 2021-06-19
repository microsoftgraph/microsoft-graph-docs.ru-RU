---
title: List accessReviewInstance
description: Извлечение объектов accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 52844146764ffb85be50a9c8d8609b466a88ba2e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030528"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="66368-103">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="66368-103">List accessReviewInstance</span></span>

<span data-ttu-id="66368-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66368-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66368-105">[Извлечение объектов accessReviewInstance](../resources/accessreviewinstance.md) для определенного [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="66368-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="66368-106">Возвращается список объектов zero или more **accessReviewInstance,** включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="66368-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="66368-107">Возвращенные объекты не включают связанный accessReviewInstanceDecisionItems.</span><span class="sxs-lookup"><span data-stu-id="66368-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="66368-108">Чтобы получить решения в экземпляре, используйте [list accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="66368-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="66368-109">Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="66368-109">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="66368-110">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="66368-110">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="66368-111">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="66368-111">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="66368-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66368-112">Permissions</span></span>
<span data-ttu-id="66368-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66368-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66368-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66368-115">Permission type</span></span>                        | <span data-ttu-id="66368-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66368-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="66368-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66368-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="66368-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66368-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="66368-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="66368-119">Application</span></span>                            | <span data-ttu-id="66368-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66368-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="66368-121">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="66368-121">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="66368-122">Чтобы просмотреть только те экземпляры, в которые назначен рецензент, см. в примере [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span><span class="sxs-lookup"><span data-stu-id="66368-122">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="66368-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66368-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66368-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66368-124">Optional query parameters</span></span>
<span data-ttu-id="66368-125">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="66368-125">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="66368-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="66368-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="66368-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66368-127">Request headers</span></span>
<span data-ttu-id="66368-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="66368-128">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="66368-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66368-129">Request body</span></span>
<span data-ttu-id="66368-130">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="66368-130">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="66368-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="66368-131">Response</span></span>
<span data-ttu-id="66368-132">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReviewInstance](../resources/accessreviewinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="66368-132">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66368-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="66368-133">Examples</span></span>
### <a name="request"></a><span data-ttu-id="66368-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="66368-134">Request</span></span>
<span data-ttu-id="66368-135">В следующем примере показан запрос на извлечение всех экземпляров обзора доступа для определения.</span><span class="sxs-lookup"><span data-stu-id="66368-135">The following example shows a request to retrieve all the access review instances for a definition.</span></span>


# <a name="http"></a>[<span data-ttu-id="66368-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="66368-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="66368-137">C#</span><span class="sxs-lookup"><span data-stu-id="66368-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66368-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66368-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66368-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66368-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66368-140">Java</span><span class="sxs-lookup"><span data-stu-id="66368-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="66368-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="66368-141">Response</span></span>
><span data-ttu-id="66368-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="66368-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('8564a649-4f67-4e09-88e7-55def6530e88')/instances",
    "@odata.count": 2,
    "value": [
        {
            "id": "7bc18cf4-3d70-4009-bc8e-a7c5adb30849",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f661fdd0-f0f7-42c0-8281-e89c6527ac63/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        },
        {
            "id": "f1f35945-3f42-4941-9f7b-465e545f6f99",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f4ac55b3-3b3c-417e-85bd-183bbda3ccf2/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="66368-143">См. также</span><span class="sxs-lookup"><span data-stu-id="66368-143">See also</span></span>

- [<span data-ttu-id="66368-144">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="66368-144">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="66368-145">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="66368-145">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
