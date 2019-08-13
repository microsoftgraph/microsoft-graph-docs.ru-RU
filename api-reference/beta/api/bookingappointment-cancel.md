---
title: 'Букингаппоинтмент: Отмена'
description: Отмена указанного Букингаппоинтмент в указанном букингбусинесс и отправка сообщения связанным клиентским сотрудникам и сотрудникам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ce8b34bd122b1a437dbc0069a2ab88c876fbf3ad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318462"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="fed22-103">Букингаппоинтмент: Отмена</span><span class="sxs-lookup"><span data-stu-id="fed22-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fed22-104">Отмена указанного [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md)и отправка сообщения связанным клиентским сотрудникам и сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="fed22-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="fed22-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fed22-105">Permissions</span></span>
<span data-ttu-id="fed22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fed22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fed22-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fed22-108">Permission type</span></span>      | <span data-ttu-id="fed22-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fed22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fed22-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fed22-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fed22-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="fed22-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fed22-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fed22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fed22-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fed22-113">Not supported.</span></span>   |
|<span data-ttu-id="fed22-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fed22-114">Application</span></span> | <span data-ttu-id="fed22-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fed22-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fed22-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fed22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="fed22-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fed22-117">Request headers</span></span>
| <span data-ttu-id="fed22-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fed22-118">Name</span></span>       | <span data-ttu-id="fed22-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fed22-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fed22-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fed22-120">Authorization</span></span>  | <span data-ttu-id="fed22-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fed22-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fed22-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fed22-122">Request body</span></span>
<span data-ttu-id="fed22-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fed22-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fed22-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="fed22-124">Parameter</span></span>    | <span data-ttu-id="fed22-125">Тип</span><span class="sxs-lookup"><span data-stu-id="fed22-125">Type</span></span>   |<span data-ttu-id="fed22-126">Описание</span><span class="sxs-lookup"><span data-stu-id="fed22-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fed22-127">канцеллатионмессаже</span><span class="sxs-lookup"><span data-stu-id="fed22-127">cancellationMessage</span></span>|<span data-ttu-id="fed22-128">String</span><span class="sxs-lookup"><span data-stu-id="fed22-128">String</span></span>|<span data-ttu-id="fed22-129">Сообщение, которое должно быть подтверждено с клиентом о том, что встреча отменена.</span><span class="sxs-lookup"><span data-stu-id="fed22-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="fed22-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fed22-130">Response</span></span>
<span data-ttu-id="fed22-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fed22-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="fed22-133">При попытке отменить встречу, не ексисит, этот метод возвращает значение `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="fed22-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="fed22-134">Пример</span><span class="sxs-lookup"><span data-stu-id="fed22-134">Example</span></span>
<span data-ttu-id="fed22-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fed22-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fed22-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="fed22-136">Request</span></span>
<span data-ttu-id="fed22-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fed22-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fed22-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="fed22-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fed22-139">C#</span><span class="sxs-lookup"><span data-stu-id="fed22-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fed22-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fed22-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fed22-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fed22-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fed22-142">Java</span><span class="sxs-lookup"><span data-stu-id="fed22-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingappointment-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fed22-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fed22-143">Response</span></span>
<span data-ttu-id="fed22-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fed22-144">The following is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
