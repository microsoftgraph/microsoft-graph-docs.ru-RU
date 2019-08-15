---
title: Получение Букингкурренци
description: Получение свойств объекта Букингкурренци, доступного для корпоративных книг корпорации Майкрософт.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b3e6c49ef67d97b636ed29d84a2e085c90305b1f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419442"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="28204-103">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="28204-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28204-104">Получение свойств объекта [букингкурренци](../resources/bookingcurrency.md) , доступного для корпоративных книг корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="28204-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="28204-105">Чтобы указать валюту, используйте свойство **ID** , которое является кодом валюты.</span><span class="sxs-lookup"><span data-stu-id="28204-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="28204-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28204-106">Permissions</span></span>
<span data-ttu-id="28204-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28204-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28204-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28204-109">Permission type</span></span>      | <span data-ttu-id="28204-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28204-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28204-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28204-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28204-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="28204-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="28204-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28204-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28204-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28204-114">Not supported.</span></span>   |
|<span data-ttu-id="28204-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28204-115">Application</span></span> | <span data-ttu-id="28204-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28204-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="28204-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28204-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28204-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28204-118">Optional query parameters</span></span>
<span data-ttu-id="28204-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="28204-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28204-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28204-120">Request headers</span></span>
| <span data-ttu-id="28204-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28204-121">Name</span></span>      |<span data-ttu-id="28204-122">Описание</span><span class="sxs-lookup"><span data-stu-id="28204-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28204-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28204-123">Authorization</span></span>  | <span data-ttu-id="28204-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="28204-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="28204-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28204-125">Request body</span></span>
<span data-ttu-id="28204-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28204-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="28204-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="28204-127">Response</span></span>
<span data-ttu-id="28204-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28204-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28204-129">Пример</span><span class="sxs-lookup"><span data-stu-id="28204-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28204-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="28204-130">Request</span></span>
<span data-ttu-id="28204-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28204-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28204-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="28204-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28204-133">C#</span><span class="sxs-lookup"><span data-stu-id="28204-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28204-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28204-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28204-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="28204-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28204-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="28204-136">Response</span></span>
<span data-ttu-id="28204-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28204-137">The following is an example of the response.</span></span> <span data-ttu-id="28204-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="28204-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="28204-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28204-139">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
