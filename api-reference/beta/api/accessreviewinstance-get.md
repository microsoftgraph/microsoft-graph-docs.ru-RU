---
title: Получение Акцессревиевинстанце
description: Получение объекта Акцессревиевинстанце.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b14fe31961524b6aef67d08e683bfecd7a2324c2
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001015"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="502ac-103">Получение Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="502ac-103">Get accessReviewInstance</span></span>

<span data-ttu-id="502ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="502ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="502ac-105">Получение объекта [акцессревиевинстанце](../resources/accessreviewinstance.md) с помощью идентификатора акцессревиевинстанце и его родительского [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="502ac-105">Retrieve an [accessReviewInstance](../resources/accessreviewinstance.md) object using the identifier of an accessReviewInstance and its parent [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="502ac-106">Возвращает все свойства экземпляра, кроме связанного [акцессревиевинстанцедеЦисионитемс](../resources/accessreviewinstancedecisionitem.md).</span><span class="sxs-lookup"><span data-stu-id="502ac-106">This returns all properties of the instance except for the associated [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="502ac-107">Чтобы получить решения для экземпляра, используйте [List акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="502ac-107">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="502ac-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="502ac-108">Permissions</span></span>
<span data-ttu-id="502ac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="502ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="502ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="502ac-111">Permission type</span></span>                        | <span data-ttu-id="502ac-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="502ac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="502ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="502ac-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="502ac-114">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="502ac-114">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="502ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="502ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="502ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="502ac-116">Not supported.</span></span>|
|<span data-ttu-id="502ac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="502ac-117">Application</span></span>                            | <span data-ttu-id="502ac-118">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="502ac-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="502ac-119">Чтобы вызвать этот API, пользователь, вошедшего в систему, должен быть включен в роль каталога, которая разрешает им читать проверку доступа, или пользователь может быть назначен в качестве проверяющего при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="502ac-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="502ac-120">Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviewsv2-root.md).</span><span class="sxs-lookup"><span data-stu-id="502ac-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="502ac-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="502ac-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}
```
## <a name="request-headers"></a><span data-ttu-id="502ac-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="502ac-122">Request headers</span></span>
<span data-ttu-id="502ac-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="502ac-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="502ac-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="502ac-124">Request body</span></span>
<span data-ttu-id="502ac-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="502ac-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="502ac-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="502ac-126">Response</span></span>
<span data-ttu-id="502ac-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [акцессревиевинстанце](../resources/accessreviewinstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="502ac-127">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="502ac-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="502ac-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="502ac-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="502ac-129">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/12490cdb-6a18-4c08-ba2c-44442f0a0138
```


### <a name="response"></a><span data-ttu-id="502ac-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="502ac-130">Response</span></span>
><span data-ttu-id="502ac-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="502ac-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "12490cdb-6a18-4c08-ba2c-44442f0a0138",
    "startDateTime": "2020-09-21T20:03:36Z",
    "endDateTime": "2020-09-23T20:03:36Z",
    "status": "NotStarted",
    "scope": {
        "query": "/groups/b7a4444b-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="502ac-133">См. также</span><span class="sxs-lookup"><span data-stu-id="502ac-133">See also</span></span>

- [<span data-ttu-id="502ac-134">Получение Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="502ac-134">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="502ac-135">Список Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="502ac-135">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


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
