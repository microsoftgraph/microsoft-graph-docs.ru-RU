---
title: Перечисление объектов secureScores
description: Получение свойств и связей объекта Секурескорес.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 5d2712d2d77271116d9ad59b1e0f5a28491536f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046948"
---
# <a name="list-securescores"></a><span data-ttu-id="08404-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="08404-103">List secureScores</span></span>

<span data-ttu-id="08404-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08404-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08404-105">Получение свойств и связей объекта [секурескорес](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="08404-105">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08404-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08404-106">Permissions</span></span>

<span data-ttu-id="08404-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08404-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08404-109">Permission type</span></span>      | <span data-ttu-id="08404-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08404-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08404-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08404-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="08404-112">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="08404-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="08404-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08404-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="08404-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08404-114">Not supported.</span></span>  |
|<span data-ttu-id="08404-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08404-115">Application</span></span> | <span data-ttu-id="08404-116">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="08404-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08404-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08404-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="08404-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08404-118">Request headers</span></span>

| <span data-ttu-id="08404-119">Имя</span><span class="sxs-lookup"><span data-stu-id="08404-119">Name</span></span>      |<span data-ttu-id="08404-120">Описание</span><span class="sxs-lookup"><span data-stu-id="08404-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08404-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08404-121">Authorization</span></span>  | <span data-ttu-id="08404-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="08404-122">Bearer {code}.</span></span> <span data-ttu-id="08404-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="08404-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08404-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08404-124">Request body</span></span>

<span data-ttu-id="08404-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08404-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08404-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="08404-126">Response</span></span>

<span data-ttu-id="08404-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескорес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08404-127">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08404-128">Пример</span><span class="sxs-lookup"><span data-stu-id="08404-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="08404-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="08404-129">Request</span></span>

<span data-ttu-id="08404-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08404-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08404-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="08404-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```
# <a name="c"></a>[<span data-ttu-id="08404-132">C#</span><span class="sxs-lookup"><span data-stu-id="08404-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescores-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08404-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08404-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescores-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08404-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08404-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescores-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08404-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="08404-135">Response</span></span>

<span data-ttu-id="08404-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08404-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection":true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 1,
            "createdDateTime": "createdDateTime.value",
            "currentScore": 1,
            "enabledServices": "enabledServices.value",
            "licensedUserCount": 1,
            "maxScore": 1,
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value"
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "seatSizeRangeUpperValue": "seatSizeRangeUpperValue.value",
                    "categoryValue": "categoryValue.value",
                    "seatSizeRangeLowerValue": "seatSizeRangeLowerValue.value"
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "categoryValue": "categoryValue.value"
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


