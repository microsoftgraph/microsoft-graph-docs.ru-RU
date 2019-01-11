---
title: 'bookingAppointment: Отмена'
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ffb800b5084177b05b62e1ba14b475b8a760d766
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844480"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="42a08-104">bookingAppointment: Отмена</span><span class="sxs-lookup"><span data-stu-id="42a08-104">bookingAppointment: cancel</span></span>

 > <span data-ttu-id="42a08-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42a08-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42a08-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a08-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="42a08-107">Отменить указанного [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md)и отправить сообщение связанных клиентов и сотрудников.</span><span class="sxs-lookup"><span data-stu-id="42a08-107">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="42a08-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42a08-108">Permissions</span></span>
<span data-ttu-id="42a08-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42a08-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42a08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42a08-111">Permission type</span></span>      | <span data-ttu-id="42a08-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42a08-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42a08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42a08-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="42a08-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="42a08-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="42a08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42a08-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42a08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a08-116">Not supported.</span></span>   |
|<span data-ttu-id="42a08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42a08-117">Application</span></span> | <span data-ttu-id="42a08-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a08-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="42a08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42a08-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="42a08-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42a08-120">Request headers</span></span>
| <span data-ttu-id="42a08-121">Имя</span><span class="sxs-lookup"><span data-stu-id="42a08-121">Name</span></span>       | <span data-ttu-id="42a08-122">Описание</span><span class="sxs-lookup"><span data-stu-id="42a08-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42a08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42a08-123">Authorization</span></span>  | <span data-ttu-id="42a08-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="42a08-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="42a08-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42a08-125">Request body</span></span>
<span data-ttu-id="42a08-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="42a08-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="42a08-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="42a08-127">Parameter</span></span>    | <span data-ttu-id="42a08-128">Тип</span><span class="sxs-lookup"><span data-stu-id="42a08-128">Type</span></span>   |<span data-ttu-id="42a08-129">Описание</span><span class="sxs-lookup"><span data-stu-id="42a08-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42a08-130">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="42a08-130">cancellationMessage</span></span>|<span data-ttu-id="42a08-131">Строка</span><span class="sxs-lookup"><span data-stu-id="42a08-131">String</span></span>|<span data-ttu-id="42a08-132">Сообщение для подтверждения с клиентом отменена встречи.</span><span class="sxs-lookup"><span data-stu-id="42a08-132">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="42a08-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a08-133">Response</span></span>
<span data-ttu-id="42a08-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="42a08-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="42a08-136">При попытке отменить встречи, которая не существует, этот метод возвращает `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="42a08-136">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="42a08-137">Пример</span><span class="sxs-lookup"><span data-stu-id="42a08-137">Example</span></span>
<span data-ttu-id="42a08-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="42a08-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="42a08-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="42a08-139">Request</span></span>
<span data-ttu-id="42a08-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42a08-140">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="42a08-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="42a08-141">Response</span></span>
<span data-ttu-id="42a08-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42a08-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
