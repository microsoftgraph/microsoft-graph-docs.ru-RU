---
title: Получить accessReviewScheduleDefinition
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a5c6713d9fb99a7077888c903a61bfde12574a43
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030315"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="f1ac3-103">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="f1ac3-103">Get accessReviewScheduleDefinition</span></span>
<span data-ttu-id="f1ac3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1ac3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1ac3-105">Ознакомьтесь с свойствами и отношениями [объекта accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1ac3-105">Read the properties and relationships of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="f1ac3-106">Чтобы получить экземпляры серии обзоров доступа, используйте [API accessReviewInstance.](accessreviewinstance-list.md)</span><span class="sxs-lookup"><span data-stu-id="f1ac3-106">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>   

## <a name="permissions"></a><span data-ttu-id="f1ac3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1ac3-107">Permissions</span></span>
<span data-ttu-id="f1ac3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1ac3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ac3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1ac3-110">Permission type</span></span>|<span data-ttu-id="f1ac3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1ac3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1ac3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1ac3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1ac3-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ac3-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="f1ac3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1ac3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1ac3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1ac3-115">Not supported.</span></span>|
|<span data-ttu-id="f1ac3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1ac3-116">Application</span></span>|<span data-ttu-id="f1ac3-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ac3-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="f1ac3-118">Чтобы вызвать этот API, входив в каталог, пользователь должен также быть в роли каталога, которая позволяет ему читать обзор доступа, или пользователь может быть назначен в качестве рецензента в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="f1ac3-118">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="f1ac3-119">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="f1ac3-119">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="f1ac3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1ac3-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1ac3-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f1ac3-121">Optional query parameters</span></span>
<span data-ttu-id="f1ac3-122">Этот метод поддерживает `$select` параметр запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="f1ac3-122">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="f1ac3-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f1ac3-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1ac3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1ac3-124">Request headers</span></span>
|<span data-ttu-id="f1ac3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f1ac3-125">Name</span></span>|<span data-ttu-id="f1ac3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f1ac3-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f1ac3-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1ac3-127">Authorization</span></span>|<span data-ttu-id="f1ac3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1ac3-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ac3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1ac3-130">Request body</span></span>
<span data-ttu-id="f1ac3-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1ac3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1ac3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1ac3-132">Response</span></span>

<span data-ttu-id="f1ac3-133">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f1ac3-133">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1ac3-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="f1ac3-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1ac3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1ac3-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewscheduledefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```


### <a name="response"></a><span data-ttu-id="f1ac3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1ac3-136">Response</span></span>
><span data-ttu-id="f1ac3-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f1ac3-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6bf2f6c-2f6c-d6bf-6c2f-bfd66c2fbfd6",
    "displayName": "Review example",
    "status": "Applying",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "reviewers": [
        {
            "query": "/v1.0/users/5555556e-fce3-4e2d-b28e-4ac0c7d2fa10",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "instanceEnumerationScope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": false,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 10,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-04-28",
                "endDate": "2021-05-08"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.disableAndDeleteUserApplyAction"
            }
        ]
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="f1ac3-138">См. также</span><span class="sxs-lookup"><span data-stu-id="f1ac3-138">See also</span></span>

- [<span data-ttu-id="f1ac3-139">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="f1ac3-139">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-post.md)
- [<span data-ttu-id="f1ac3-140">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="f1ac3-140">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="f1ac3-141">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f1ac3-141">List accessReviewInstance</span></span>](accessreviewinstance-list.md)
