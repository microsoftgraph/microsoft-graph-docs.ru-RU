---
title: Обновление bookingcustomer
description: Обновление свойств объекта bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 476c827474026914a7839947d7a88a9c10b8a917
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047821"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="ddb51-103">Обновление bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="ddb51-103">Update bookingcustomer</span></span>

<span data-ttu-id="ddb51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb51-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb51-105">Обновление свойств объекта [bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="ddb51-105">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ddb51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb51-106">Permissions</span></span>
<span data-ttu-id="ddb51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb51-109">Permission type</span></span>      | <span data-ttu-id="ddb51-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddb51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddb51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddb51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ddb51-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ddb51-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ddb51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddb51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb51-114">Not supported.</span></span>   |
|<span data-ttu-id="ddb51-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddb51-115">Application</span></span> | <span data-ttu-id="ddb51-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb51-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ddb51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddb51-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ddb51-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddb51-118">Optional request headers</span></span>
| <span data-ttu-id="ddb51-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ddb51-119">Name</span></span>       | <span data-ttu-id="ddb51-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb51-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ddb51-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddb51-121">Authorization</span></span>  | <span data-ttu-id="ddb51-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ddb51-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddb51-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddb51-123">Request body</span></span>
<span data-ttu-id="ddb51-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ddb51-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ddb51-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddb51-127">Property</span></span>     | <span data-ttu-id="ddb51-128">Тип</span><span class="sxs-lookup"><span data-stu-id="ddb51-128">Type</span></span>   |<span data-ttu-id="ddb51-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb51-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddb51-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb51-130">displayName</span></span>|<span data-ttu-id="ddb51-131">String</span><span class="sxs-lookup"><span data-stu-id="ddb51-131">String</span></span>|<span data-ttu-id="ddb51-132">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="ddb51-132">The name of the customer.</span></span>|
|<span data-ttu-id="ddb51-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ddb51-133">emailAddress</span></span>|<span data-ttu-id="ddb51-134">String</span><span class="sxs-lookup"><span data-stu-id="ddb51-134">String</span></span>|<span data-ttu-id="ddb51-135">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="ddb51-135">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="ddb51-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb51-136">Response</span></span>
<span data-ttu-id="ddb51-137">В случае успеха этот метод возвращает код отклика и `200 OK` обновленный [объект bookingCustomer](../resources/bookingcustomer.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ddb51-137">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ddb51-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ddb51-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddb51-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddb51-139">Request</span></span>
<span data-ttu-id="ddb51-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddb51-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddb51-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb51-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ddb51-142">C#</span><span class="sxs-lookup"><span data-stu-id="ddb51-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddb51-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddb51-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddb51-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddb51-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddb51-145">Java</span><span class="sxs-lookup"><span data-stu-id="ddb51-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ddb51-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb51-146">Response</span></span>
<span data-ttu-id="ddb51-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ddb51-147">The following is an example of the response.</span></span> <span data-ttu-id="ddb51-148">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ddb51-148">Note: The response object shown here might be shortened for readability.</span></span>
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


