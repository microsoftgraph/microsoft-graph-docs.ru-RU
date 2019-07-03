---
title: Перечисление объектов secureScores
description: Получение свойств и связей объекта Секурескорес.
localization_priority: Normal
ms.openlocfilehash: 1a4994b2e767906b0058bf85936375949f609fbd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457347"
---
# <a name="list-securescores"></a><span data-ttu-id="b5edc-103">Перечисление объектов secureScores</span><span class="sxs-lookup"><span data-stu-id="b5edc-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5edc-104">Получение свойств и связей объекта [секурескорес](../resources/securescores.md) .</span><span class="sxs-lookup"><span data-stu-id="b5edc-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5edc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5edc-105">Permissions</span></span>

<span data-ttu-id="b5edc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5edc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5edc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5edc-108">Permission type</span></span>      | <span data-ttu-id="b5edc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5edc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5edc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5edc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b5edc-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="b5edc-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="b5edc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5edc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b5edc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5edc-113">Not supported.</span></span>  |
|<span data-ttu-id="b5edc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5edc-114">Application</span></span> | <span data-ttu-id="b5edc-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="b5edc-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5edc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5edc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="b5edc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5edc-117">Request headers</span></span>

| <span data-ttu-id="b5edc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b5edc-118">Name</span></span>      |<span data-ttu-id="b5edc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b5edc-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5edc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5edc-120">Authorization</span></span>  | <span data-ttu-id="b5edc-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="b5edc-121">Bearer {code}.</span></span> <span data-ttu-id="b5edc-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b5edc-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5edc-123">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="b5edc-123">Request body</span></span>

<span data-ttu-id="b5edc-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5edc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5edc-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5edc-125">Response</span></span>

<span data-ttu-id="b5edc-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескорес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5edc-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5edc-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b5edc-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5edc-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5edc-128">Request</span></span>

<span data-ttu-id="b5edc-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5edc-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b5edc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5edc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5edc-131">C#</span><span class="sxs-lookup"><span data-stu-id="b5edc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescores-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5edc-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5edc-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescores-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5edc-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b5edc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescores-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5edc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5edc-134">Response</span></span>

<span data-ttu-id="b5edc-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b5edc-135">The following is an example of the response.</span></span>
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
