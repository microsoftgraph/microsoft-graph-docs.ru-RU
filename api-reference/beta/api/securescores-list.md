---
title: Перечисление объектов secureScores
description: Извлечение свойств и связи объекта secureScores.
localization_priority: Normal
ms.openlocfilehash: e574c3e52eb60f29dac89e2795b04666c7a1f02b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642963"
---
# <a name="list-securescores"></a><span data-ttu-id="a0d1e-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="a0d1e-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d1e-104">Извлечение свойств и связи объекта [secureScores](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="a0d1e-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0d1e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0d1e-105">Permissions</span></span>

<span data-ttu-id="a0d1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d1e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0d1e-108">Permission type</span></span>      | <span data-ttu-id="a0d1e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0d1e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0d1e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0d1e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a0d1e-111">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="a0d1e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0d1e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a0d1e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-113">Not supported.</span></span>  |
|<span data-ttu-id="a0d1e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0d1e-114">Application</span></span> | <span data-ttu-id="a0d1e-115">SecurityEvents.Read.All SecurityEvents.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0d1e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0d1e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="a0d1e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0d1e-117">Request headers</span></span>

| <span data-ttu-id="a0d1e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a0d1e-118">Name</span></span>      |<span data-ttu-id="a0d1e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a0d1e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0d1e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0d1e-120">Authorization</span></span>  | <span data-ttu-id="a0d1e-p102">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-p102">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d1e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0d1e-123">Request body</span></span>

<span data-ttu-id="a0d1e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0d1e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d1e-125">Response</span></span>

<span data-ttu-id="a0d1e-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **secureScores** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d1e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a0d1e-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0d1e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0d1e-128">Request</span></span>

<span data-ttu-id="a0d1e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="a0d1e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d1e-130">Response</span></span>

<span data-ttu-id="a0d1e-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a0d1e-131">The following is an example of the response.</span></span>
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
