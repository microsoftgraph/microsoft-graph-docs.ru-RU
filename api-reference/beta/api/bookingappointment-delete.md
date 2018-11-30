---
title: Удаление bookingAppointment
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 076c08b240ee3bd9b0648a000f1399fa2f6060b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075368"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="022ae-104">Удаление bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="022ae-104">Delete bookingAppointment</span></span>

 > <span data-ttu-id="022ae-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="022ae-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="022ae-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="022ae-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="022ae-107">Удалите [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="022ae-107">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="022ae-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="022ae-108">Permissions</span></span>
<span data-ttu-id="022ae-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="022ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="022ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="022ae-111">Permission type</span></span>      | <span data-ttu-id="022ae-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="022ae-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="022ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="022ae-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="022ae-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="022ae-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="022ae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="022ae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="022ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="022ae-116">Not supported.</span></span>   |
|<span data-ttu-id="022ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="022ae-117">Application</span></span> | <span data-ttu-id="022ae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="022ae-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="022ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="022ae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="022ae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="022ae-120">Request headers</span></span>
| <span data-ttu-id="022ae-121">Имя</span><span class="sxs-lookup"><span data-stu-id="022ae-121">Name</span></span>       | <span data-ttu-id="022ae-122">Описание</span><span class="sxs-lookup"><span data-stu-id="022ae-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="022ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="022ae-123">Authorization</span></span>  | <span data-ttu-id="022ae-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="022ae-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="022ae-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="022ae-125">Request body</span></span>
<span data-ttu-id="022ae-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="022ae-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="022ae-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="022ae-127">Response</span></span>
<span data-ttu-id="022ae-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="022ae-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="022ae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="022ae-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="022ae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="022ae-131">Request</span></span>
<span data-ttu-id="022ae-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="022ae-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="022ae-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="022ae-133">Response</span></span>
<span data-ttu-id="022ae-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="022ae-134">The following is an example of the response.</span></span> <span data-ttu-id="022ae-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="022ae-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="022ae-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="022ae-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->