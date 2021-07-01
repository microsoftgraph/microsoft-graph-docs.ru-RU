---
title: Получить accessReviewInstance
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 62d18407a457de2c335656800c12d2b311ea90b6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211000"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="e70e4-103">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="e70e4-103">Get accessReviewInstance</span></span>
<span data-ttu-id="e70e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e70e4-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="e70e4-105">Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="e70e4-105">Read the properties and relationships of an [accessReviewInstance](../resources/accessreviewinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e70e4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e70e4-106">Permissions</span></span>
<span data-ttu-id="e70e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e70e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e70e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e70e4-109">Permission type</span></span>|<span data-ttu-id="e70e4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e70e4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e70e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e70e4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e70e4-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e70e4-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="e70e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e70e4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e70e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e70e4-114">Not supported.</span></span>|
|<span data-ttu-id="e70e4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e70e4-115">Application</span></span>|<span data-ttu-id="e70e4-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e70e4-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e70e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e70e4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e70e4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e70e4-118">Optional query parameters</span></span>
<span data-ttu-id="e70e4-119">Этот метод поддерживает `$select` параметр запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="e70e4-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="e70e4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e70e4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e70e4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e70e4-121">Request headers</span></span>
|<span data-ttu-id="e70e4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e70e4-122">Name</span></span>|<span data-ttu-id="e70e4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e70e4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e70e4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e70e4-124">Authorization</span></span>|<span data-ttu-id="e70e4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e70e4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e70e4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e70e4-127">Request body</span></span>
<span data-ttu-id="e70e4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e70e4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e70e4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e70e4-129">Response</span></span>

<span data-ttu-id="e70e4-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e70e4-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e70e4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e70e4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e70e4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e70e4-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e70e4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e70e4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/12345ba0-cbf0-5678-8868-4444c7f4cc06
```
# <a name="c"></a>[<span data-ttu-id="e70e4-134">C#</span><span class="sxs-lookup"><span data-stu-id="e70e4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e70e4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e70e4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e70e4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e70e4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e70e4-137">Java</span><span class="sxs-lookup"><span data-stu-id="e70e4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e70e4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e70e4-138">Response</span></span>
><span data-ttu-id="e70e4-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e70e4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
