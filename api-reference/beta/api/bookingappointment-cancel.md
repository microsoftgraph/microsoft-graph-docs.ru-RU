---
title: 'Букингаппоинтмент: Отмена'
description: Отмена указанного Букингаппоинтмент в указанном букингбусинесс и отправка сообщения связанным клиентским сотрудникам и сотрудникам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f80f97f6e085980d26ce4555f35f769db6a4f4e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322553"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="fc182-103">Букингаппоинтмент: Отмена</span><span class="sxs-lookup"><span data-stu-id="fc182-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc182-104">Отмена указанного [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md)и отправка сообщения связанным клиентским сотрудникам и сотрудникам.</span><span class="sxs-lookup"><span data-stu-id="fc182-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc182-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc182-105">Permissions</span></span>
<span data-ttu-id="fc182-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc182-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc182-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc182-108">Permission type</span></span>      | <span data-ttu-id="fc182-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc182-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc182-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc182-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fc182-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="fc182-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fc182-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc182-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc182-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc182-113">Not supported.</span></span>   |
|<span data-ttu-id="fc182-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc182-114">Application</span></span> | <span data-ttu-id="fc182-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc182-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fc182-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc182-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="fc182-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc182-117">Request headers</span></span>
| <span data-ttu-id="fc182-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fc182-118">Name</span></span>       | <span data-ttu-id="fc182-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fc182-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc182-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc182-120">Authorization</span></span>  | <span data-ttu-id="fc182-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fc182-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc182-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc182-122">Request body</span></span>
<span data-ttu-id="fc182-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fc182-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc182-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc182-124">Parameter</span></span>    | <span data-ttu-id="fc182-125">Тип</span><span class="sxs-lookup"><span data-stu-id="fc182-125">Type</span></span>   |<span data-ttu-id="fc182-126">Описание</span><span class="sxs-lookup"><span data-stu-id="fc182-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc182-127">Канцеллатионмессаже</span><span class="sxs-lookup"><span data-stu-id="fc182-127">cancellationMessage</span></span>|<span data-ttu-id="fc182-128">String</span><span class="sxs-lookup"><span data-stu-id="fc182-128">String</span></span>|<span data-ttu-id="fc182-129">Сообщение, которое должно быть подтверждено с клиентом о том, что встреча отменена.</span><span class="sxs-lookup"><span data-stu-id="fc182-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="fc182-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc182-130">Response</span></span>
<span data-ttu-id="fc182-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fc182-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="fc182-133">При попытке отменить встречу, не ексисит, этот метод возвращает значение `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="fc182-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="fc182-134">Пример</span><span class="sxs-lookup"><span data-stu-id="fc182-134">Example</span></span>
<span data-ttu-id="fc182-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc182-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc182-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc182-136">Request</span></span>
<span data-ttu-id="fc182-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc182-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="fc182-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc182-138">Response</span></span>
<span data-ttu-id="fc182-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc182-139">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
