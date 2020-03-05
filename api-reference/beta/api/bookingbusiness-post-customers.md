---
title: Создание Букингкустомер
description: Создание нового объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ec605f55935f18fff3f2c6042090af51571e4258
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441188"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="aebe1-103">Создание Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="aebe1-103">Create bookingCustomer</span></span>

<span data-ttu-id="aebe1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aebe1-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aebe1-105">Создание нового объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="aebe1-105">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aebe1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aebe1-106">Permissions</span></span>
<span data-ttu-id="aebe1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aebe1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aebe1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aebe1-109">Permission type</span></span>      | <span data-ttu-id="aebe1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aebe1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aebe1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aebe1-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="aebe1-112">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="aebe1-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="aebe1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aebe1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aebe1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aebe1-114">Not supported.</span></span>   |
|<span data-ttu-id="aebe1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aebe1-115">Application</span></span> | <span data-ttu-id="aebe1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aebe1-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="aebe1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aebe1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="aebe1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aebe1-118">Request headers</span></span>
| <span data-ttu-id="aebe1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aebe1-119">Name</span></span>       | <span data-ttu-id="aebe1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aebe1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aebe1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aebe1-121">Authorization</span></span>  | <span data-ttu-id="aebe1-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="aebe1-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="aebe1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aebe1-123">Request body</span></span>
<span data-ttu-id="aebe1-124">В тексте запроса добавьте представление объекта [букингкустомер](../resources/bookingcustomer.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aebe1-124">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="aebe1-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="aebe1-125">Response</span></span>
<span data-ttu-id="aebe1-126">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aebe1-126">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aebe1-127">Пример</span><span class="sxs-lookup"><span data-stu-id="aebe1-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aebe1-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="aebe1-128">Request</span></span>
<span data-ttu-id="aebe1-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aebe1-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aebe1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="aebe1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
# <a name="c"></a>[<span data-ttu-id="aebe1-131">C#</span><span class="sxs-lookup"><span data-stu-id="aebe1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aebe1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aebe1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aebe1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aebe1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="aebe1-134">В тексте запроса добавьте представление объекта [букингкустомер](../resources/bookingcustomer.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aebe1-134">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aebe1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="aebe1-135">Response</span></span>
<span data-ttu-id="aebe1-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aebe1-136">The following is an example of the response.</span></span> <span data-ttu-id="aebe1-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="aebe1-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aebe1-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aebe1-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
