---
title: Обновление букингкустомер
description: Обновление свойств объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 779c2bbc647612455113a2f218ab7b0efc58de3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318133"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="13a42-103">Обновление букингкустомер</span><span class="sxs-lookup"><span data-stu-id="13a42-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13a42-104">Обновление свойств объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="13a42-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="13a42-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13a42-105">Permissions</span></span>
<span data-ttu-id="13a42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13a42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a42-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13a42-108">Permission type</span></span>      | <span data-ttu-id="13a42-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13a42-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13a42-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13a42-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13a42-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="13a42-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="13a42-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13a42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13a42-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13a42-113">Not supported.</span></span>   |
|<span data-ttu-id="13a42-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13a42-114">Application</span></span> | <span data-ttu-id="13a42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13a42-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="13a42-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13a42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="13a42-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13a42-117">Optional request headers</span></span>
| <span data-ttu-id="13a42-118">Имя</span><span class="sxs-lookup"><span data-stu-id="13a42-118">Name</span></span>       | <span data-ttu-id="13a42-119">Описание</span><span class="sxs-lookup"><span data-stu-id="13a42-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="13a42-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13a42-120">Authorization</span></span>  | <span data-ttu-id="13a42-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="13a42-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="13a42-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13a42-122">Request body</span></span>
<span data-ttu-id="13a42-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="13a42-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="13a42-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="13a42-126">Property</span></span>     | <span data-ttu-id="13a42-127">Тип</span><span class="sxs-lookup"><span data-stu-id="13a42-127">Type</span></span>   |<span data-ttu-id="13a42-128">Описание</span><span class="sxs-lookup"><span data-stu-id="13a42-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13a42-129">displayName</span><span class="sxs-lookup"><span data-stu-id="13a42-129">displayName</span></span>|<span data-ttu-id="13a42-130">String</span><span class="sxs-lookup"><span data-stu-id="13a42-130">String</span></span>|<span data-ttu-id="13a42-131">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="13a42-131">The name of the customer.</span></span>|
|<span data-ttu-id="13a42-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="13a42-132">emailAddress</span></span>|<span data-ttu-id="13a42-133">String</span><span class="sxs-lookup"><span data-stu-id="13a42-133">String</span></span>|<span data-ttu-id="13a42-134">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="13a42-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="13a42-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="13a42-135">Response</span></span>
<span data-ttu-id="13a42-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13a42-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13a42-137">Пример</span><span class="sxs-lookup"><span data-stu-id="13a42-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13a42-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="13a42-138">Request</span></span>
<span data-ttu-id="13a42-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13a42-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="13a42-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="13a42-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="13a42-141">C#</span><span class="sxs-lookup"><span data-stu-id="13a42-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13a42-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13a42-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13a42-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="13a42-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="13a42-144">Java</span><span class="sxs-lookup"><span data-stu-id="13a42-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13a42-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="13a42-145">Response</span></span>
<span data-ttu-id="13a42-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13a42-146">The following is an example of the response.</span></span> <span data-ttu-id="13a42-147">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="13a42-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="13a42-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13a42-148">All of the properties will be returned from an actual call.</span></span>
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
