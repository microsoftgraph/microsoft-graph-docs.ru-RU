---
title: Обновление букингкустомер
description: Обновление свойств объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 56d0b4bf1c4ef7dbfc8a6878833afc4c9ebba5da
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439051"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="c048e-103">Обновление букингкустомер</span><span class="sxs-lookup"><span data-stu-id="c048e-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c048e-104">Обновление свойств объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="c048e-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c048e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c048e-105">Permissions</span></span>
<span data-ttu-id="c048e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c048e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c048e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c048e-108">Permission type</span></span>      | <span data-ttu-id="c048e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c048e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c048e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c048e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c048e-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="c048e-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c048e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c048e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c048e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c048e-113">Not supported.</span></span>   |
|<span data-ttu-id="c048e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c048e-114">Application</span></span> | <span data-ttu-id="c048e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c048e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c048e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c048e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c048e-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c048e-117">Optional request headers</span></span>
| <span data-ttu-id="c048e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c048e-118">Name</span></span>       | <span data-ttu-id="c048e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c048e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c048e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c048e-120">Authorization</span></span>  | <span data-ttu-id="c048e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c048e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c048e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c048e-122">Request body</span></span>
<span data-ttu-id="c048e-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c048e-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c048e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c048e-126">Property</span></span>     | <span data-ttu-id="c048e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c048e-127">Type</span></span>   |<span data-ttu-id="c048e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c048e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c048e-129">displayName</span><span class="sxs-lookup"><span data-stu-id="c048e-129">displayName</span></span>|<span data-ttu-id="c048e-130">String</span><span class="sxs-lookup"><span data-stu-id="c048e-130">String</span></span>|<span data-ttu-id="c048e-131">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="c048e-131">The name of the customer.</span></span>|
|<span data-ttu-id="c048e-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c048e-132">emailAddress</span></span>|<span data-ttu-id="c048e-133">String</span><span class="sxs-lookup"><span data-stu-id="c048e-133">String</span></span>|<span data-ttu-id="c048e-134">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="c048e-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="c048e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c048e-135">Response</span></span>
<span data-ttu-id="c048e-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c048e-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c048e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c048e-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c048e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c048e-138">Request</span></span>
<span data-ttu-id="c048e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c048e-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c048e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c048e-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c048e-141">C#</span><span class="sxs-lookup"><span data-stu-id="c048e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c048e-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="c048e-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c048e-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c048e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c048e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c048e-144">Response</span></span>
<span data-ttu-id="c048e-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c048e-145">The following is an example of the response.</span></span> <span data-ttu-id="c048e-146">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c048e-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c048e-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c048e-147">All of the properties will be returned from an actual call.</span></span>
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
