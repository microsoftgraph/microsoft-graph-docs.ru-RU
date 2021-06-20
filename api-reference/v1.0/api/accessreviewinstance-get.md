---
title: Получить accessReviewInstance
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8a8e2ec2ec059201dabea44523bf45ef054a4f3f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031351"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="9956f-103">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9956f-103">Get accessReviewInstance</span></span>
<span data-ttu-id="9956f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9956f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="9956f-105">Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="9956f-105">Read the properties and relationships of an [accessReviewInstance](../resources/accessreviewinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9956f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9956f-106">Permissions</span></span>
<span data-ttu-id="9956f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9956f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9956f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9956f-109">Permission type</span></span>|<span data-ttu-id="9956f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9956f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9956f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9956f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9956f-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9956f-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="9956f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9956f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9956f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9956f-114">Not supported.</span></span>|
|<span data-ttu-id="9956f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9956f-115">Application</span></span>|<span data-ttu-id="9956f-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9956f-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9956f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9956f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9956f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9956f-118">Optional query parameters</span></span>
<span data-ttu-id="9956f-119">Этот метод поддерживает `$select` параметр запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="9956f-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9956f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9956f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9956f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9956f-121">Request headers</span></span>
|<span data-ttu-id="9956f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9956f-122">Name</span></span>|<span data-ttu-id="9956f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9956f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9956f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9956f-124">Authorization</span></span>|<span data-ttu-id="9956f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9956f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9956f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9956f-127">Request body</span></span>
<span data-ttu-id="9956f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9956f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9956f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9956f-129">Response</span></span>

<span data-ttu-id="9956f-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9956f-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9956f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="9956f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9956f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9956f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/12345ba0-cbf0-5678-8868-4444c7f4cc06
```


### <a name="response"></a><span data-ttu-id="9956f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9956f-133">Response</span></span>
><span data-ttu-id="9956f-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9956f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewInstance",
    "id": "d7fbc019-c019-d7fb-19c0-fbd719c0fbd7",
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
}
```
