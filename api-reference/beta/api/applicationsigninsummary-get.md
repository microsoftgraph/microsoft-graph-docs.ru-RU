---
title: Получение Аппликатионсигнинсуммари
description: Получение свойств и связей объекта **аппликатионсигнинсуммари** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 141d531693e2cf49b5aaad30002e024d06883939
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655098"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="73587-103">Получение Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="73587-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73587-104">Получение свойств и связей объекта [аппликатионсигнинсуммари](../resources/applicationsigninsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="73587-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73587-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73587-105">Permissions</span></span>
<span data-ttu-id="73587-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="73587-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="73587-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73587-108">Permission type</span></span>      | <span data-ttu-id="73587-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73587-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73587-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73587-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73587-111">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="73587-111">Report.Read.All</span></span> |
|<span data-ttu-id="73587-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73587-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73587-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73587-113">Not supported</span></span>   |
|<span data-ttu-id="73587-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73587-114">Application</span></span> | <span data-ttu-id="73587-115">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="73587-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="73587-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73587-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="73587-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="73587-117">Function parameters</span></span>

| <span data-ttu-id="73587-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="73587-118">Parameter</span></span> | <span data-ttu-id="73587-119">Описание</span><span class="sxs-lookup"><span data-stu-id="73587-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="73587-120">period</span><span class="sxs-lookup"><span data-stu-id="73587-120">period</span></span> | <span data-ttu-id="73587-121">Либо `D7` (последние семь дней), `D30` либо (последние 30 дней); другие значения создают ошибки.</span><span class="sxs-lookup"><span data-stu-id="73587-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="73587-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73587-122">Request headers</span></span>
| <span data-ttu-id="73587-123">Имя</span><span class="sxs-lookup"><span data-stu-id="73587-123">Name</span></span>      |<span data-ttu-id="73587-124">Описание</span><span class="sxs-lookup"><span data-stu-id="73587-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73587-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73587-125">Authorization</span></span> | <span data-ttu-id="73587-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="73587-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="73587-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73587-127">Request body</span></span>
<span data-ttu-id="73587-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73587-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73587-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="73587-129">Response</span></span>
<span data-ttu-id="73587-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аппликатионсигнинсуммари](../resources/applicationsigninsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73587-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73587-131">Пример</span><span class="sxs-lookup"><span data-stu-id="73587-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="73587-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73587-132">Request</span></span>
<span data-ttu-id="73587-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73587-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
### <a name="response"></a><span data-ttu-id="73587-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="73587-134">Response</span></span>
<span data-ttu-id="73587-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73587-135">The following is an example of the response.</span></span> 

><span data-ttu-id="73587-136">**Примечание:** Объект Response, показанный здесь, ммигхт должен быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="73587-136">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="73587-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73587-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="73587-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="73587-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="73587-139">C#</span><span class="sxs-lookup"><span data-stu-id="73587-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73587-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="73587-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
