---
title: Перечисление объектов secureScores
description: Получение свойств и связей объекта Секурескорес.
localization_priority: Normal
ms.openlocfilehash: 55a9628d88300a97b62145f22f6fc18fce04b92b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638811"
---
# <a name="list-securescores"></a><span data-ttu-id="4b187-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="4b187-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b187-104">Получение свойств и связей объекта [секурескорес](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="4b187-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b187-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b187-105">Permissions</span></span>

<span data-ttu-id="4b187-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b187-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b187-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b187-108">Permission type</span></span>      | <span data-ttu-id="4b187-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b187-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b187-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b187-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4b187-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="4b187-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="4b187-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b187-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4b187-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b187-113">Not supported.</span></span>  |
|<span data-ttu-id="4b187-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b187-114">Application</span></span> | <span data-ttu-id="4b187-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="4b187-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b187-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b187-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="4b187-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b187-117">Request headers</span></span>

| <span data-ttu-id="4b187-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4b187-118">Name</span></span>      |<span data-ttu-id="4b187-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4b187-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b187-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b187-120">Authorization</span></span>  | <span data-ttu-id="4b187-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="4b187-121">Bearer {code}.</span></span> <span data-ttu-id="4b187-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4b187-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b187-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b187-123">Request body</span></span>

<span data-ttu-id="4b187-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b187-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b187-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b187-125">Response</span></span>

<span data-ttu-id="4b187-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескорес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b187-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b187-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4b187-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b187-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b187-128">Request</span></span>

<span data-ttu-id="4b187-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b187-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="4b187-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b187-130">Response</span></span>

<span data-ttu-id="4b187-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b187-131">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4b187-132">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="4b187-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4b187-133">Языках</span><span class="sxs-lookup"><span data-stu-id="4b187-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescores_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b187-134">Язык</span><span class="sxs-lookup"><span data-stu-id="4b187-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescores_list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
