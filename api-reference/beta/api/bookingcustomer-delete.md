---
title: Удаление bookingCustomer
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1e2c303733b850d45b8c805f40fc42bc835cc313
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941550"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="c6c23-104">Удаление bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="c6c23-104">Delete bookingCustomer</span></span>

 > <span data-ttu-id="c6c23-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6c23-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6c23-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6c23-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c6c23-107">Удаление указанного [bookingCustomer](../resources/bookingcustomer.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="c6c23-107">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6c23-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6c23-108">Permissions</span></span>
<span data-ttu-id="c6c23-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6c23-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6c23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6c23-111">Permission type</span></span>      | <span data-ttu-id="c6c23-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6c23-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6c23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6c23-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6c23-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c6c23-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c6c23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6c23-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6c23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6c23-116">Not supported.</span></span>   |
|<span data-ttu-id="c6c23-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6c23-117">Application</span></span> | <span data-ttu-id="c6c23-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6c23-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c6c23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6c23-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c6c23-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6c23-120">Request headers</span></span>
| <span data-ttu-id="c6c23-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c6c23-121">Name</span></span>       | <span data-ttu-id="c6c23-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c6c23-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6c23-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6c23-123">Authorization</span></span>  | <span data-ttu-id="c6c23-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c6c23-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6c23-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6c23-125">Request body</span></span>
<span data-ttu-id="c6c23-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6c23-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c6c23-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6c23-127">Response</span></span>
<span data-ttu-id="c6c23-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c6c23-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6c23-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c6c23-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6c23-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6c23-131">Request</span></span>
<span data-ttu-id="c6c23-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6c23-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="c6c23-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6c23-133">Response</span></span>
<span data-ttu-id="c6c23-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6c23-134">The following is an example of the response.</span></span> <span data-ttu-id="c6c23-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c6c23-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c6c23-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6c23-136">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
