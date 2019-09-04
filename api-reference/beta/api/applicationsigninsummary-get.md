---
title: Получение Аппликатионсигнинсуммари
description: Получение свойств и связей объекта **аппликатионсигнинсуммари** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f52c24bb1b47e1c8c3302ac3b876ae6983d067d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719019"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="c2ec4-103">Получение Аппликатионсигнинсуммари</span><span class="sxs-lookup"><span data-stu-id="c2ec4-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2ec4-104">Получение свойств и связей объекта [аппликатионсигнинсуммари](../resources/applicationsigninsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c2ec4-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2ec4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ec4-105">Permissions</span></span>
<span data-ttu-id="c2ec4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2ec4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="c2ec4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ec4-108">Permission type</span></span>      | <span data-ttu-id="c2ec4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2ec4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2ec4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2ec4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2ec4-111">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c2ec4-111">Report.Read.All</span></span> |
|<span data-ttu-id="c2ec4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2ec4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ec4-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2ec4-113">Not supported</span></span>   |
|<span data-ttu-id="c2ec4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2ec4-114">Application</span></span> | <span data-ttu-id="c2ec4-115">Report. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c2ec4-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c2ec4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2ec4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="c2ec4-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c2ec4-117">Function parameters</span></span>

| <span data-ttu-id="c2ec4-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="c2ec4-118">Parameter</span></span> | <span data-ttu-id="c2ec4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c2ec4-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="c2ec4-120">period</span><span class="sxs-lookup"><span data-stu-id="c2ec4-120">period</span></span> | <span data-ttu-id="c2ec4-121">Либо `D7` (последние семь дней), `D30` либо (последние 30 дней); другие значения создают ошибки.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c2ec4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2ec4-122">Request headers</span></span>
| <span data-ttu-id="c2ec4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c2ec4-123">Name</span></span>      |<span data-ttu-id="c2ec4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c2ec4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2ec4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2ec4-125">Authorization</span></span> | <span data-ttu-id="c2ec4-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c2ec4-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2ec4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2ec4-127">Request body</span></span>
<span data-ttu-id="c2ec4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2ec4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2ec4-129">Response</span></span>
<span data-ttu-id="c2ec4-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аппликатионсигнинсуммари](../resources/applicationsigninsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2ec4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c2ec4-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2ec4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2ec4-132">Request</span></span>
<span data-ttu-id="c2ec4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2ec4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2ec4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2ec4-135">C#</span><span class="sxs-lookup"><span data-stu-id="c2ec4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2ec4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2ec4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2ec4-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c2ec4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c2ec4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2ec4-138">Response</span></span>
<span data-ttu-id="c2ec4-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c2ec4-140">**Примечание:** Объект Response, показанный здесь, ммигхт должен быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-140">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="c2ec4-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2ec4-141">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
