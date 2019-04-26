---
title: Обновление букингкустомер
description: Обновление свойств объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 2b634b99ce9a3940f80e0ef8f296e7f96184fdba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322461"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="59726-103">Обновление букингкустомер</span><span class="sxs-lookup"><span data-stu-id="59726-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59726-104">Обновление свойств объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="59726-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="59726-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59726-105">Permissions</span></span>
<span data-ttu-id="59726-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59726-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59726-108">Permission type</span></span>      | <span data-ttu-id="59726-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59726-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59726-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59726-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59726-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="59726-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="59726-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59726-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59726-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59726-113">Not supported.</span></span>   |
|<span data-ttu-id="59726-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59726-114">Application</span></span> | <span data-ttu-id="59726-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59726-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="59726-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59726-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="59726-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59726-117">Optional request headers</span></span>
| <span data-ttu-id="59726-118">Имя</span><span class="sxs-lookup"><span data-stu-id="59726-118">Name</span></span>       | <span data-ttu-id="59726-119">Описание</span><span class="sxs-lookup"><span data-stu-id="59726-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="59726-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59726-120">Authorization</span></span>  | <span data-ttu-id="59726-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="59726-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="59726-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59726-122">Request body</span></span>
<span data-ttu-id="59726-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="59726-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="59726-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="59726-126">Property</span></span>     | <span data-ttu-id="59726-127">Тип</span><span class="sxs-lookup"><span data-stu-id="59726-127">Type</span></span>   |<span data-ttu-id="59726-128">Описание</span><span class="sxs-lookup"><span data-stu-id="59726-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59726-129">displayName</span><span class="sxs-lookup"><span data-stu-id="59726-129">displayName</span></span>|<span data-ttu-id="59726-130">String</span><span class="sxs-lookup"><span data-stu-id="59726-130">String</span></span>|<span data-ttu-id="59726-131">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="59726-131">The name of the customer.</span></span>|
|<span data-ttu-id="59726-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="59726-132">emailAddress</span></span>|<span data-ttu-id="59726-133">String</span><span class="sxs-lookup"><span data-stu-id="59726-133">String</span></span>|<span data-ttu-id="59726-134">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="59726-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="59726-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="59726-135">Response</span></span>
<span data-ttu-id="59726-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59726-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59726-137">Пример</span><span class="sxs-lookup"><span data-stu-id="59726-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59726-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="59726-138">Request</span></span>
<span data-ttu-id="59726-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59726-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="59726-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="59726-140">Response</span></span>
<span data-ttu-id="59726-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="59726-141">The following is an example of the response.</span></span> <span data-ttu-id="59726-142">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="59726-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="59726-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59726-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
