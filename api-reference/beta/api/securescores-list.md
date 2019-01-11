---
title: Перечисление объектов secureScores
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 6bf0a1e1964c93043bad4a81ab812786627ea737
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831817"
---
# <a name="list-securescores"></a><span data-ttu-id="b9e19-104">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="b9e19-104">List secureScores</span></span>

 > <span data-ttu-id="b9e19-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9e19-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9e19-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e19-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9e19-107">Извлечение свойств и связи объекта [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="b9e19-107">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e19-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9e19-108">Permissions</span></span>

<span data-ttu-id="b9e19-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9e19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9e19-111">Permission type</span></span>      | <span data-ttu-id="b9e19-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9e19-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9e19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9e19-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9e19-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="b9e19-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="b9e19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9e19-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b9e19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e19-116">Not supported.</span></span>  |
|<span data-ttu-id="b9e19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9e19-117">Application</span></span> | <span data-ttu-id="b9e19-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="b9e19-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9e19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9e19-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="b9e19-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9e19-120">Request headers</span></span>

| <span data-ttu-id="b9e19-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b9e19-121">Name</span></span>      |<span data-ttu-id="b9e19-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9e19-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9e19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e19-123">Authorization</span></span>  | <span data-ttu-id="b9e19-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9e19-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e19-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9e19-126">Request body</span></span>

<span data-ttu-id="b9e19-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9e19-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e19-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9e19-128">Response</span></span>

<span data-ttu-id="b9e19-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **secureScores** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9e19-129">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e19-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b9e19-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9e19-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9e19-131">Request</span></span>

<span data-ttu-id="b9e19-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9e19-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="b9e19-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9e19-133">Response</span></span>

<span data-ttu-id="b9e19-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b9e19-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScores"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "activeUserCount": "activeUserCount.value",
            "createdDateTime": "createdDateTime.value",
            "currentScore": "currentScore.value",
            "enabledServices": "enabledServices.value",
            "licensedUserCount": "licensedUserCount.value",
            "maxScore": "maxScore.value",
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


<!-- {
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
