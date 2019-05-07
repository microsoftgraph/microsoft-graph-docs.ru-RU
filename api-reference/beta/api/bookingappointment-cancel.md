---
title: 'Букингаппоинтмент: Отмена'
description: Отмена указанного Букингаппоинтмент в указанном букингбусинесс и отправка сообщения связанным клиентским сотрудникам и сотрудникам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c96ed0403e59f4b2dd357514168361fc3bc683f6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636536"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="540d8-103">Букингаппоинтмент: Отмена</span><span class="sxs-lookup"><span data-stu-id="540d8-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="540d8-104">Отмена указанного [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md)и отправка сообщения связанным клиентским сотрудникам и сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="540d8-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="540d8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="540d8-105">Permissions</span></span>
<span data-ttu-id="540d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="540d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="540d8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="540d8-108">Permission type</span></span>      | <span data-ttu-id="540d8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="540d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="540d8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="540d8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="540d8-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="540d8-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="540d8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="540d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="540d8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="540d8-113">Not supported.</span></span>   |
|<span data-ttu-id="540d8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="540d8-114">Application</span></span> | <span data-ttu-id="540d8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="540d8-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="540d8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="540d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="540d8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="540d8-117">Request headers</span></span>
| <span data-ttu-id="540d8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="540d8-118">Name</span></span>       | <span data-ttu-id="540d8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="540d8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="540d8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="540d8-120">Authorization</span></span>  | <span data-ttu-id="540d8-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="540d8-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="540d8-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="540d8-122">Request body</span></span>
<span data-ttu-id="540d8-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="540d8-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="540d8-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="540d8-124">Parameter</span></span>    | <span data-ttu-id="540d8-125">Тип</span><span class="sxs-lookup"><span data-stu-id="540d8-125">Type</span></span>   |<span data-ttu-id="540d8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="540d8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="540d8-127">Канцеллатионмессаже</span><span class="sxs-lookup"><span data-stu-id="540d8-127">cancellationMessage</span></span>|<span data-ttu-id="540d8-128">String</span><span class="sxs-lookup"><span data-stu-id="540d8-128">String</span></span>|<span data-ttu-id="540d8-129">Сообщение, которое должно быть подтверждено с клиентом о том, что встреча отменена.</span><span class="sxs-lookup"><span data-stu-id="540d8-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="540d8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="540d8-130">Response</span></span>
<span data-ttu-id="540d8-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="540d8-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="540d8-133">При попытке отменить встречу, не ексисит, этот метод возвращает значение `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="540d8-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="540d8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="540d8-134">Example</span></span>
<span data-ttu-id="540d8-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="540d8-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="540d8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="540d8-136">Request</span></span>
<span data-ttu-id="540d8-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="540d8-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingappointment_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```

##### <a name="response"></a><span data-ttu-id="540d8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="540d8-138">Response</span></span>
<span data-ttu-id="540d8-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="540d8-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="540d8-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="540d8-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="540d8-141">Языках</span><span class="sxs-lookup"><span data-stu-id="540d8-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="540d8-142">Язык</span><span class="sxs-lookup"><span data-stu-id="540d8-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
