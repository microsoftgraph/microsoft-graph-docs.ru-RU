---
title: 'bookingAppointment: Отмена'
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 4cd7b511f997f32c134f70a976cd94c2ed910fb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074758"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="31051-104">bookingAppointment: Отмена</span><span class="sxs-lookup"><span data-stu-id="31051-104">bookingAppointment: cancel</span></span>

 > <span data-ttu-id="31051-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31051-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31051-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31051-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="31051-107">Отменить указанного [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md)и отправить сообщение связанных клиентов и сотрудников.</span><span class="sxs-lookup"><span data-stu-id="31051-107">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="31051-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31051-108">Permissions</span></span>
<span data-ttu-id="31051-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31051-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31051-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31051-111">Permission type</span></span>      | <span data-ttu-id="31051-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31051-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31051-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31051-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="31051-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="31051-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="31051-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31051-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31051-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31051-116">Not supported.</span></span>   |
|<span data-ttu-id="31051-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31051-117">Application</span></span> | <span data-ttu-id="31051-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31051-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="31051-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31051-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="31051-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31051-120">Request headers</span></span>
| <span data-ttu-id="31051-121">Имя</span><span class="sxs-lookup"><span data-stu-id="31051-121">Name</span></span>       | <span data-ttu-id="31051-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31051-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31051-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31051-123">Authorization</span></span>  | <span data-ttu-id="31051-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="31051-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="31051-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31051-125">Request body</span></span>
<span data-ttu-id="31051-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="31051-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="31051-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="31051-127">Parameter</span></span>    | <span data-ttu-id="31051-128">Тип</span><span class="sxs-lookup"><span data-stu-id="31051-128">Type</span></span>   |<span data-ttu-id="31051-129">Description</span><span class="sxs-lookup"><span data-stu-id="31051-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31051-130">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="31051-130">cancellationMessage</span></span>|<span data-ttu-id="31051-131">String</span><span class="sxs-lookup"><span data-stu-id="31051-131">String</span></span>|<span data-ttu-id="31051-132">Сообщение для подтверждения с клиентом отменена встречи.</span><span class="sxs-lookup"><span data-stu-id="31051-132">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="31051-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="31051-133">Response</span></span>
<span data-ttu-id="31051-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="31051-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="31051-136">При попытке отменить встречи, которая не существует, этот метод возвращает `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="31051-136">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="31051-137">Пример</span><span class="sxs-lookup"><span data-stu-id="31051-137">Example</span></span>
<span data-ttu-id="31051-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="31051-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="31051-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="31051-139">Request</span></span>
<span data-ttu-id="31051-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31051-140">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="31051-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="31051-141">Response</span></span>
<span data-ttu-id="31051-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="31051-142">The following is an example of the response.</span></span> 
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