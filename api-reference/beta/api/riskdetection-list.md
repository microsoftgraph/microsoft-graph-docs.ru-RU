---
title: Список Рискдетектион
description: Получение свойств коллекции объекта **рискдетектион** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c0917c451777b7c98c11a25a21b5978cf199b93b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181212"
---
# <a name="list-riskdetection"></a><span data-ttu-id="760cc-103">Список Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="760cc-103">List riskDetection</span></span>

<span data-ttu-id="760cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="760cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="760cc-105">Получение свойств коллекции объектов **рискдетектион** .</span><span class="sxs-lookup"><span data-stu-id="760cc-105">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="760cc-106">Для использования API обнаружения риска необходима лицензия Azure AD Premium P1 или P2.</span><span class="sxs-lookup"><span data-stu-id="760cc-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="760cc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="760cc-107">Permissions</span></span>

<span data-ttu-id="760cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="760cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="760cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="760cc-110">Permission type</span></span>      | <span data-ttu-id="760cc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="760cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="760cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="760cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="760cc-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="760cc-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="760cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="760cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="760cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="760cc-115">Not supported.</span></span>    |
|<span data-ttu-id="760cc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="760cc-116">Application</span></span> | <span data-ttu-id="760cc-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="760cc-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="760cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="760cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="760cc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="760cc-119">Optional query parameters</span></span>

<span data-ttu-id="760cc-120">Этот метод поддерживает `$filter` и `$select` настраивает ответ на запрос.</span><span class="sxs-lookup"><span data-stu-id="760cc-120">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="760cc-121">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="760cc-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="760cc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="760cc-122">Request headers</span></span>

| <span data-ttu-id="760cc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="760cc-123">Name</span></span>      |<span data-ttu-id="760cc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="760cc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="760cc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="760cc-125">Authorization</span></span>  | <span data-ttu-id="760cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="760cc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="760cc-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="760cc-128">Content-Type</span></span> | <span data-ttu-id="760cc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="760cc-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="760cc-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="760cc-130">Request body</span></span>

<span data-ttu-id="760cc-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="760cc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="760cc-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="760cc-132">Response</span></span>

<span data-ttu-id="760cc-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискдетектион](../resources/riskdetection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="760cc-133">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="760cc-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="760cc-134">Examples</span></span>

### <a name="example-1-list-risk-detections"></a><span data-ttu-id="760cc-135">Пример 1: список обнаруженных рисков</span><span class="sxs-lookup"><span data-stu-id="760cc-135">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="760cc-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="760cc-136">Request</span></span>

<span data-ttu-id="760cc-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="760cc-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="760cc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="760cc-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="760cc-139">C#</span><span class="sxs-lookup"><span data-stu-id="760cc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="760cc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="760cc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="760cc-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="760cc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="760cc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="760cc-142">Response</span></span>

<span data-ttu-id="760cc-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="760cc-143">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="760cc-144">Пример 2: список обнаруженных рисков и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="760cc-144">Example 2: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="760cc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="760cc-145">Request</span></span>

<span data-ttu-id="760cc-146">В приведенном ниже примере показано, `$filter` как получить коллекцию обнаружений рисков, в которой уровень риска является средним, или тип события риска — унфамиларфеатурес, что означает, что вход в систему был незнакомым или неизвестным расположением.</span><span class="sxs-lookup"><span data-stu-id="760cc-146">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="http"></a>[<span data-ttu-id="760cc-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="760cc-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections?$filter=riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="c"></a>[<span data-ttu-id="760cc-148">C#</span><span class="sxs-lookup"><span data-stu-id="760cc-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="760cc-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="760cc-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="760cc-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="760cc-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="760cc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="760cc-151">Response</span></span>

<span data-ttu-id="760cc-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="760cc-152">Here is an example of the response.</span></span>
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
