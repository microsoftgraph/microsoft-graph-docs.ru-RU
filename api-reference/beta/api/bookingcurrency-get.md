---
title: Получение Букингкурренци
description: Получение свойств объекта Букингкурренци, доступного для корпоративных книг корпорации Майкрософт.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 31d8791f6ae2345bedffa7fe25a80f83651bda3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987955"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="aa3fe-103">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="aa3fe-103">Get bookingCurrency</span></span>

<span data-ttu-id="aa3fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa3fe-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa3fe-105">Получение свойств объекта [букингкурренци](../resources/bookingcurrency.md) , доступного для корпоративных книг корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-105">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="aa3fe-106">Чтобы указать валюту, используйте свойство **ID** , которое является кодом валюты.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-106">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa3fe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa3fe-107">Permissions</span></span>
<span data-ttu-id="aa3fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa3fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa3fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa3fe-110">Permission type</span></span>      | <span data-ttu-id="aa3fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa3fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa3fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa3fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aa3fe-113">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="aa3fe-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="aa3fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa3fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa3fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-115">Not supported.</span></span>   |
|<span data-ttu-id="aa3fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa3fe-116">Application</span></span> | <span data-ttu-id="aa3fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="aa3fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa3fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa3fe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa3fe-119">Optional query parameters</span></span>
<span data-ttu-id="aa3fe-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa3fe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa3fe-121">Request headers</span></span>
| <span data-ttu-id="aa3fe-122">Имя</span><span class="sxs-lookup"><span data-stu-id="aa3fe-122">Name</span></span>      |<span data-ttu-id="aa3fe-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aa3fe-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa3fe-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa3fe-124">Authorization</span></span>  | <span data-ttu-id="aa3fe-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="aa3fe-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa3fe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa3fe-126">Request body</span></span>
<span data-ttu-id="aa3fe-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="aa3fe-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa3fe-128">Response</span></span>
<span data-ttu-id="aa3fe-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-129">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa3fe-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aa3fe-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa3fe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa3fe-131">Request</span></span>
<span data-ttu-id="aa3fe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa3fe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa3fe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="c"></a>[<span data-ttu-id="aa3fe-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa3fe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa3fe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa3fe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa3fe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa3fe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aa3fe-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa3fe-137">Response</span></span>
<span data-ttu-id="aa3fe-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-138">The following is an example of the response.</span></span> <span data-ttu-id="aa3fe-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aa3fe-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa3fe-140">All of the properties will be returned from an actual call.</span></span>
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


