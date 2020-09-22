---
title: Обновление букингкустомер
description: Обновление свойств объекта Букингкустомер.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 98450dfbbcdad378cfb700fdb6d7c443c88696b6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987887"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="6b80b-103">Обновление букингкустомер</span><span class="sxs-lookup"><span data-stu-id="6b80b-103">Update bookingcustomer</span></span>

<span data-ttu-id="6b80b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b80b-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b80b-105">Обновление свойств объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="6b80b-105">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b80b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b80b-106">Permissions</span></span>
<span data-ttu-id="6b80b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b80b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b80b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b80b-109">Permission type</span></span>      | <span data-ttu-id="6b80b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b80b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b80b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b80b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b80b-112">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="6b80b-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6b80b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b80b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b80b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b80b-114">Not supported.</span></span>   |
|<span data-ttu-id="6b80b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b80b-115">Application</span></span> | <span data-ttu-id="6b80b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b80b-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6b80b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b80b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="6b80b-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b80b-118">Optional request headers</span></span>
| <span data-ttu-id="6b80b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6b80b-119">Name</span></span>       | <span data-ttu-id="6b80b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6b80b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6b80b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b80b-121">Authorization</span></span>  | <span data-ttu-id="6b80b-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6b80b-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b80b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b80b-123">Request body</span></span>
<span data-ttu-id="6b80b-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6b80b-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6b80b-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b80b-127">Property</span></span>     | <span data-ttu-id="6b80b-128">Тип</span><span class="sxs-lookup"><span data-stu-id="6b80b-128">Type</span></span>   |<span data-ttu-id="6b80b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6b80b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b80b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="6b80b-130">displayName</span></span>|<span data-ttu-id="6b80b-131">String</span><span class="sxs-lookup"><span data-stu-id="6b80b-131">String</span></span>|<span data-ttu-id="6b80b-132">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="6b80b-132">The name of the customer.</span></span>|
|<span data-ttu-id="6b80b-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6b80b-133">emailAddress</span></span>|<span data-ttu-id="6b80b-134">String</span><span class="sxs-lookup"><span data-stu-id="6b80b-134">String</span></span>|<span data-ttu-id="6b80b-135">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="6b80b-135">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="6b80b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b80b-136">Response</span></span>
<span data-ttu-id="6b80b-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b80b-137">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b80b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6b80b-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b80b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b80b-139">Request</span></span>
<span data-ttu-id="6b80b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b80b-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b80b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b80b-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6b80b-142">C#</span><span class="sxs-lookup"><span data-stu-id="6b80b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b80b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b80b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b80b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b80b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b80b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b80b-145">Response</span></span>
<span data-ttu-id="6b80b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b80b-146">The following is an example of the response.</span></span> <span data-ttu-id="6b80b-147">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6b80b-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6b80b-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b80b-148">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->


