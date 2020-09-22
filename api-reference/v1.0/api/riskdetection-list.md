---
title: Список Рискдетектионс
description: Получение списка объектов Рискдетектион и их свойств.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6d1a57d0f83608169b412b520f1342662b592d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079349"
---
# <a name="list-riskdetections"></a><span data-ttu-id="48520-103">Список Рискдетектионс</span><span class="sxs-lookup"><span data-stu-id="48520-103">List riskDetections</span></span>
<span data-ttu-id="48520-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48520-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48520-105">Получение списка объектов [рискдетектион](../resources/riskdetection.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="48520-105">Get a list of the [riskDetection](../resources/riskdetection.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="48520-106">Для использования API обнаружения риска необходима лицензия Azure AD Premium P1 или P2.</span><span class="sxs-lookup"><span data-stu-id="48520-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="48520-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48520-107">Permissions</span></span>
<span data-ttu-id="48520-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="48520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="48520-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48520-110">Permission type</span></span>      | <span data-ttu-id="48520-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48520-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48520-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48520-112">Delegated (work or school account)</span></span> | <span data-ttu-id="48520-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="48520-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="48520-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48520-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48520-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48520-115">Not supported.</span></span>    |
|<span data-ttu-id="48520-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="48520-116">Application</span></span> | <span data-ttu-id="48520-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="48520-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48520-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48520-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48520-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48520-119">Optional query parameters</span></span>
<span data-ttu-id="48520-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="48520-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="48520-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="48520-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="48520-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48520-122">Request headers</span></span>
|<span data-ttu-id="48520-123">Имя</span><span class="sxs-lookup"><span data-stu-id="48520-123">Name</span></span>|<span data-ttu-id="48520-124">Описание</span><span class="sxs-lookup"><span data-stu-id="48520-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="48520-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48520-125">Authorization</span></span>|<span data-ttu-id="48520-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48520-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48520-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48520-128">Request body</span></span>
<span data-ttu-id="48520-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48520-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48520-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="48520-130">Response</span></span>

<span data-ttu-id="48520-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискдетектион](../resources/riskdetection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48520-131">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48520-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="48520-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48520-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="48520-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskdetection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections
```


### <a name="response"></a><span data-ttu-id="48520-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="48520-134">Response</span></span>
<span data-ttu-id="48520-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="48520-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
  {
    "@odata.type": "#microsoft.graph.riskDetection",
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskEventType": "unfamiliarFeatures",
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
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
  ]
}
```


