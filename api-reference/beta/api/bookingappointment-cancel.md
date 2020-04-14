---
title: 'Букингаппоинтмент: Отмена'
description: Отмена указанного Букингаппоинтмент в указанном букингбусинесс и отправка сообщения связанным клиентским сотрудникам и сотрудникам.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 98633524d61093c6ddc4c9c85e5e98f205a508da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43367708"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="0849a-103">Букингаппоинтмент: Отмена</span><span class="sxs-lookup"><span data-stu-id="0849a-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="0849a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0849a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0849a-105">Отмена указанного [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md)и отправка сообщения связанным клиентским сотрудникам и сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="0849a-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="0849a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0849a-106">Permissions</span></span>
<span data-ttu-id="0849a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0849a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0849a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0849a-109">Permission type</span></span>      | <span data-ttu-id="0849a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0849a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0849a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0849a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0849a-112">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="0849a-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0849a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0849a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0849a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0849a-114">Not supported.</span></span>   |
|<span data-ttu-id="0849a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0849a-115">Application</span></span> | <span data-ttu-id="0849a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0849a-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0849a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0849a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="0849a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0849a-118">Request headers</span></span>
| <span data-ttu-id="0849a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0849a-119">Name</span></span>       | <span data-ttu-id="0849a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0849a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0849a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0849a-121">Authorization</span></span>  | <span data-ttu-id="0849a-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0849a-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0849a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0849a-123">Request body</span></span>
<span data-ttu-id="0849a-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0849a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0849a-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="0849a-125">Parameter</span></span>    | <span data-ttu-id="0849a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="0849a-126">Type</span></span>   |<span data-ttu-id="0849a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="0849a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0849a-128">канцеллатионмессаже</span><span class="sxs-lookup"><span data-stu-id="0849a-128">cancellationMessage</span></span>|<span data-ttu-id="0849a-129">String</span><span class="sxs-lookup"><span data-stu-id="0849a-129">String</span></span>|<span data-ttu-id="0849a-130">Сообщение, которое должно быть подтверждено с клиентом о том, что встреча отменена.</span><span class="sxs-lookup"><span data-stu-id="0849a-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="0849a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0849a-131">Response</span></span>
<span data-ttu-id="0849a-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0849a-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="0849a-134">При попытке отменить встречу, не ексисит, этот метод возвращает значение `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="0849a-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="0849a-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0849a-135">Example</span></span>
<span data-ttu-id="0849a-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0849a-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0849a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0849a-137">Request</span></span>
<span data-ttu-id="0849a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0849a-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0849a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="0849a-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0849a-140">C#</span><span class="sxs-lookup"><span data-stu-id="0849a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0849a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0849a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0849a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0849a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0849a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0849a-143">Response</span></span>
<span data-ttu-id="0849a-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0849a-144">The following is an example of the response.</span></span>
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
