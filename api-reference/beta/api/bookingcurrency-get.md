---
title: Получение bookingCurrency
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f408ab0110de5124bb4154d0107c801b026de29a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926353"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="78b2a-104">Получение bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="78b2a-104">Get bookingCurrency</span></span>

 > <span data-ttu-id="78b2a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78b2a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78b2a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78b2a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="78b2a-107">Получение свойств объекта [bookingCurrency](../resources/bookingcurrency.md) , доступные для резервирования Microsoft business.</span><span class="sxs-lookup"><span data-stu-id="78b2a-107">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="78b2a-108">Используйте свойство **id** , которая код валюты, чтобы указать валюты.</span><span class="sxs-lookup"><span data-stu-id="78b2a-108">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="78b2a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78b2a-109">Permissions</span></span>
<span data-ttu-id="78b2a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78b2a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78b2a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78b2a-112">Permission type</span></span>      | <span data-ttu-id="78b2a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78b2a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78b2a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78b2a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="78b2a-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="78b2a-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="78b2a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78b2a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78b2a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78b2a-117">Not supported.</span></span>   |
|<span data-ttu-id="78b2a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78b2a-118">Application</span></span> | <span data-ttu-id="78b2a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78b2a-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="78b2a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78b2a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78b2a-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78b2a-121">Optional query parameters</span></span>
<span data-ttu-id="78b2a-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="78b2a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78b2a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78b2a-123">Request headers</span></span>
| <span data-ttu-id="78b2a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="78b2a-124">Name</span></span>      |<span data-ttu-id="78b2a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="78b2a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78b2a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="78b2a-126">Authorization</span></span>  | <span data-ttu-id="78b2a-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="78b2a-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="78b2a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78b2a-128">Request body</span></span>
<span data-ttu-id="78b2a-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78b2a-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="78b2a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="78b2a-130">Response</span></span>
<span data-ttu-id="78b2a-131">Успешно завершена, этот метод возвращает `200 OK` объект [bookingCurrency](../resources/bookingcurrency.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="78b2a-131">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78b2a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="78b2a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78b2a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="78b2a-133">Request</span></span>
<span data-ttu-id="78b2a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78b2a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="78b2a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="78b2a-135">Response</span></span>
<span data-ttu-id="78b2a-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="78b2a-136">The following is an example of the response.</span></span> <span data-ttu-id="78b2a-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="78b2a-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="78b2a-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78b2a-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
