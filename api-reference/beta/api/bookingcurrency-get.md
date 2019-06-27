---
title: Получение Букингкурренци
description: Получение свойств объекта Букингкурренци, доступного для корпоративных книг корпорации Майкрософт.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cbbf19d6c22ae655eabaad0647cb3e4bfee47f07
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257927"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="c8e33-103">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="c8e33-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8e33-104">Получение свойств объекта [букингкурренци](../resources/bookingcurrency.md) , доступного для корпоративных книг корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c8e33-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="c8e33-105">Чтобы указать валюту, используйте свойство **ID** , которое является кодом валюты.</span><span class="sxs-lookup"><span data-stu-id="c8e33-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e33-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e33-106">Permissions</span></span>
<span data-ttu-id="c8e33-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e33-109">Permission type</span></span>      | <span data-ttu-id="c8e33-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8e33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c8e33-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="c8e33-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c8e33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e33-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e33-114">Not supported.</span></span>   |
|<span data-ttu-id="c8e33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8e33-115">Application</span></span> | <span data-ttu-id="c8e33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e33-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c8e33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8e33-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8e33-118">Optional query parameters</span></span>
<span data-ttu-id="c8e33-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c8e33-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8e33-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8e33-120">Request headers</span></span>
| <span data-ttu-id="c8e33-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c8e33-121">Name</span></span>      |<span data-ttu-id="c8e33-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e33-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8e33-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e33-123">Authorization</span></span>  | <span data-ttu-id="c8e33-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c8e33-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e33-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8e33-125">Request body</span></span>
<span data-ttu-id="c8e33-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8e33-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c8e33-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8e33-127">Response</span></span>
<span data-ttu-id="c8e33-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e33-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8e33-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c8e33-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8e33-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e33-130">Request</span></span>
<span data-ttu-id="c8e33-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8e33-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="c8e33-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e33-132">Response</span></span>
<span data-ttu-id="c8e33-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e33-133">The following is an example of the response.</span></span> <span data-ttu-id="c8e33-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c8e33-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c8e33-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8e33-135">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 50

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingCurrencies/$entity",
    "id": "USD",
    "symbol": "$"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c8e33-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c8e33-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c8e33-137">C#</span><span class="sxs-lookup"><span data-stu-id="c8e33-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcurrency-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8e33-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8e33-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcurrency-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c8e33-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c8e33-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingcurrency-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcurrency-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingcurrency-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcurrency-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
