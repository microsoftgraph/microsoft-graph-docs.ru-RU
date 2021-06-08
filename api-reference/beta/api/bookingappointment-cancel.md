---
title: 'bookingAppointment: отмена'
description: Отмените указанное бронированиеAppointment в указанном bookingbusiness и отправьте сообщение участвующим клиентам и сотрудникам.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 4d05157faf95beaf6dab95742314472586f00063
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786276"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="4ddc3-103">bookingAppointment: отмена</span><span class="sxs-lookup"><span data-stu-id="4ddc3-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="4ddc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ddc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ddc3-105">Отмените указанное [бронированиеAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md)и отправьте сообщение участвующим клиентам и сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ddc3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ddc3-106">Permissions</span></span>
<span data-ttu-id="4ddc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ddc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ddc3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ddc3-109">Permission type</span></span>      | <span data-ttu-id="4ddc3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ddc3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ddc3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ddc3-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4ddc3-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4ddc3-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4ddc3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ddc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ddc3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-114">Not supported.</span></span>   |
|<span data-ttu-id="4ddc3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ddc3-115">Application</span></span> | <span data-ttu-id="4ddc3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4ddc3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ddc3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="4ddc3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ddc3-118">Request headers</span></span>
| <span data-ttu-id="4ddc3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4ddc3-119">Name</span></span>       | <span data-ttu-id="4ddc3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ddc3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ddc3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ddc3-121">Authorization</span></span>  | <span data-ttu-id="4ddc3-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4ddc3-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ddc3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ddc3-123">Request body</span></span>
<span data-ttu-id="4ddc3-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4ddc3-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4ddc3-125">Parameter</span></span>    | <span data-ttu-id="4ddc3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4ddc3-126">Type</span></span>   |<span data-ttu-id="4ddc3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4ddc3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ddc3-128">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="4ddc3-128">cancellationMessage</span></span>|<span data-ttu-id="4ddc3-129">String</span><span class="sxs-lookup"><span data-stu-id="4ddc3-129">String</span></span>|<span data-ttu-id="4ddc3-130">Сообщение об отмене встречи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="4ddc3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ddc3-131">Response</span></span>
<span data-ttu-id="4ddc3-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="4ddc3-134">Если вы попытается отменить встречу, которая не exisit, этот метод `HTTP 404 Not found` возвращается .</span><span class="sxs-lookup"><span data-stu-id="4ddc3-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="4ddc3-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4ddc3-135">Example</span></span>
<span data-ttu-id="4ddc3-136">Ниже приводится пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ddc3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ddc3-137">Request</span></span>
<span data-ttu-id="4ddc3-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ddc3-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ddc3-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4ddc3-140">C#</span><span class="sxs-lookup"><span data-stu-id="4ddc3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ddc3-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ddc3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ddc3-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ddc3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ddc3-143">Java</span><span class="sxs-lookup"><span data-stu-id="4ddc3-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingappointment-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ddc3-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ddc3-144">Response</span></span>
<span data-ttu-id="4ddc3-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4ddc3-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


