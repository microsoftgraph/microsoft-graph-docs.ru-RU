---
title: Перечисление объектов secureScores
description: Получение свойств и связей объекта Секурескорес.
localization_priority: Normal
ms.openlocfilehash: baa4e2e887eb739160105f2ded149481f8a8d0d4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335992"
---
# <a name="list-securescores"></a><span data-ttu-id="7e40a-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="7e40a-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e40a-104">Получение свойств и связей объекта [секурескорес](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="7e40a-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e40a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e40a-105">Permissions</span></span>

<span data-ttu-id="7e40a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e40a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e40a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e40a-108">Permission type</span></span>      | <span data-ttu-id="7e40a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e40a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e40a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e40a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7e40a-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="7e40a-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="7e40a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e40a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7e40a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e40a-113">Not supported.</span></span>  |
|<span data-ttu-id="7e40a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e40a-114">Application</span></span> | <span data-ttu-id="7e40a-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="7e40a-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e40a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e40a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="7e40a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e40a-117">Request headers</span></span>

| <span data-ttu-id="7e40a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e40a-118">Name</span></span>      |<span data-ttu-id="7e40a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7e40a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7e40a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e40a-120">Authorization</span></span>  | <span data-ttu-id="7e40a-121">Bearer {Code}.</span><span class="sxs-lookup"><span data-stu-id="7e40a-121">Bearer {code}.</span></span> <span data-ttu-id="7e40a-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7e40a-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e40a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e40a-123">Request body</span></span>

<span data-ttu-id="7e40a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e40a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e40a-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e40a-125">Response</span></span>

<span data-ttu-id="7e40a-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескорес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e40a-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e40a-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7e40a-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e40a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e40a-128">Request</span></span>

<span data-ttu-id="7e40a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e40a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="7e40a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e40a-130">Response</span></span>

<span data-ttu-id="7e40a-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e40a-131">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
