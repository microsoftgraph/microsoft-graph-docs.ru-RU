---
title: Список Рискдетектион
description: Получение свойств коллекции объекта **рискдетектион** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb6134ffd5af646f67b2caac29df7384c1d44c59
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871114"
---
# <a name="list-riskdetection"></a><span data-ttu-id="8c485-103">Список Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="8c485-103">List riskDetection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c485-104">Получение свойств коллекции объектов **рискдетектион** .</span><span class="sxs-lookup"><span data-stu-id="8c485-104">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="8c485-105">Для использования API обнаружения рисков необходима лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="8c485-105">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c485-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c485-106">Permissions</span></span>

<span data-ttu-id="8c485-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c485-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c485-109">Permission type</span></span>      | <span data-ttu-id="8c485-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c485-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c485-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c485-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c485-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c485-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="8c485-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c485-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c485-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c485-114">Not supported.</span></span>    |
|<span data-ttu-id="8c485-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c485-115">Application</span></span> | <span data-ttu-id="8c485-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c485-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c485-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c485-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c485-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c485-118">Optional query parameters</span></span>

<span data-ttu-id="8c485-119">Этот метод поддерживает `$filter` и `$select` настраивает ответ на запрос.</span><span class="sxs-lookup"><span data-stu-id="8c485-119">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="8c485-120">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="8c485-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="8c485-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c485-121">Request headers</span></span>

| <span data-ttu-id="8c485-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8c485-122">Name</span></span>      |<span data-ttu-id="8c485-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8c485-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c485-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c485-124">Authorization</span></span>  | <span data-ttu-id="8c485-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c485-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c485-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c485-127">Content-Type</span></span> | <span data-ttu-id="8c485-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8c485-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c485-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c485-129">Request body</span></span>

<span data-ttu-id="8c485-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c485-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c485-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c485-131">Response</span></span>

<span data-ttu-id="8c485-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискдетектион](../resources/riskdetection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c485-132">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c485-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c485-133">Examples</span></span>

### <a name="example-1-list-risk-detections"></a><span data-ttu-id="8c485-134">Пример 1: список обнаруженных рисков</span><span class="sxs-lookup"><span data-stu-id="8c485-134">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="8c485-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c485-135">Request</span></span>

<span data-ttu-id="8c485-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c485-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c485-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c485-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```http
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c485-138">C#</span><span class="sxs-lookup"><span data-stu-id="8c485-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c485-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c485-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c485-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8c485-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c485-141">Java</span><span class="sxs-lookup"><span data-stu-id="8c485-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8c485-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c485-142">Response</span></span>

<span data-ttu-id="8c485-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c485-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskType": "unfamiliarFeatures",
    "riskState": "remediated",
    "riskLevel": "medium",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "source": "activeDirectory",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-2-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="8c485-144">Пример 2: список обнаруженных рисков и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="8c485-144">Example 2: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="8c485-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c485-145">Request</span></span>

<span data-ttu-id="8c485-146">В приведенном ниже примере показано, `$filter` как получить коллекцию обнаружений рисков, в которой уровень риска является средним, или тип события риска — унфамиларфеатурес, что означает, что вход в систему был незнакомым или неизвестным расположением.</span><span class="sxs-lookup"><span data-stu-id="8c485-146">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8c485-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c485-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```http
GET https://graph.microsoft.com/beta/riskDetections?$filter=riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c485-148">C#</span><span class="sxs-lookup"><span data-stu-id="8c485-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c485-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="8c485-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c485-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8c485-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8c485-151">Java</span><span class="sxs-lookup"><span data-stu-id="8c485-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskdetections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8c485-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c485-152">Response</span></span>

<span data-ttu-id="8c485-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c485-153">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
    "id": "1d68fc3d60d012ff80ad4b16818bf304df1bde295fdf1db31fa5389ba9532cd1",
    "requestId": "3295073e-04b1-4871-9d15-c1f871b41100",
    "correlationId": "f141d8e5-93e9-4fd0-9eb0-c40e5f8fc092",
    "riskType": "unfamiliarFeatures",
    "riskState": "atRisk",
    "riskLevel": "medium",
    "riskDetail": "none",
    "source": "Identity Protection",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskDetections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
