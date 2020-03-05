---
title: 'Букингаппоинтмент: Отмена'
description: Отмена указанного Букингаппоинтмент в указанном букингбусинесс и отправка сообщения связанным клиентским сотрудникам и сотрудникам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 91c9da27446d7588c806f3262b5060780071a78d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441321"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="a1c0f-103">Букингаппоинтмент: Отмена</span><span class="sxs-lookup"><span data-stu-id="a1c0f-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="a1c0f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1c0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1c0f-105">Отмена указанного [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md)и отправка сообщения связанным клиентским сотрудникам и сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1c0f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1c0f-106">Permissions</span></span>
<span data-ttu-id="a1c0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1c0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1c0f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1c0f-109">Permission type</span></span>      | <span data-ttu-id="a1c0f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1c0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1c0f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1c0f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a1c0f-112">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="a1c0f-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a1c0f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1c0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1c0f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-114">Not supported.</span></span>   |
|<span data-ttu-id="a1c0f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1c0f-115">Application</span></span> | <span data-ttu-id="a1c0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a1c0f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1c0f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="a1c0f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1c0f-118">Request headers</span></span>
| <span data-ttu-id="a1c0f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a1c0f-119">Name</span></span>       | <span data-ttu-id="a1c0f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a1c0f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1c0f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1c0f-121">Authorization</span></span>  | <span data-ttu-id="a1c0f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a1c0f-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1c0f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1c0f-123">Request body</span></span>
<span data-ttu-id="a1c0f-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a1c0f-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="a1c0f-125">Parameter</span></span>    | <span data-ttu-id="a1c0f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a1c0f-126">Type</span></span>   |<span data-ttu-id="a1c0f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a1c0f-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1c0f-128">канцеллатионмессаже</span><span class="sxs-lookup"><span data-stu-id="a1c0f-128">cancellationMessage</span></span>|<span data-ttu-id="a1c0f-129">String</span><span class="sxs-lookup"><span data-stu-id="a1c0f-129">String</span></span>|<span data-ttu-id="a1c0f-130">Сообщение, которое должно быть подтверждено с клиентом о том, что встреча отменена.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="a1c0f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1c0f-131">Response</span></span>
<span data-ttu-id="a1c0f-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="a1c0f-134">При попытке отменить встречу, не ексисит, этот метод возвращает значение `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="a1c0f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a1c0f-135">Example</span></span>
<span data-ttu-id="a1c0f-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a1c0f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1c0f-137">Request</span></span>
<span data-ttu-id="a1c0f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1c0f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c0f-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a1c0f-140">C#</span><span class="sxs-lookup"><span data-stu-id="a1c0f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1c0f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1c0f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1c0f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1c0f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a1c0f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1c0f-143">Response</span></span>
<span data-ttu-id="a1c0f-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a1c0f-144">The following is an example of the response.</span></span>
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
