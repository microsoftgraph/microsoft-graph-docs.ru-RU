---
title: Создание Букингкустомер
description: Создание нового объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 5fa56ce58e148bb0edbb1a6ad9b83b9947cda7d8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439191"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="f7c46-103">Создание Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="f7c46-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c46-104">Создание нового объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="f7c46-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7c46-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c46-105">Permissions</span></span>
<span data-ttu-id="f7c46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7c46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c46-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7c46-108">Permission type</span></span>      | <span data-ttu-id="f7c46-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7c46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7c46-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7c46-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f7c46-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="f7c46-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f7c46-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7c46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7c46-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c46-113">Not supported.</span></span>   |
|<span data-ttu-id="f7c46-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7c46-114">Application</span></span> | <span data-ttu-id="f7c46-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7c46-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f7c46-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7c46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="f7c46-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7c46-117">Request headers</span></span>
| <span data-ttu-id="f7c46-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f7c46-118">Name</span></span>       | <span data-ttu-id="f7c46-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f7c46-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7c46-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7c46-120">Authorization</span></span>  | <span data-ttu-id="f7c46-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f7c46-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c46-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7c46-122">Request body</span></span>
<span data-ttu-id="f7c46-123">В тексте запроса добавьте представление объекта [букингкустомер](../resources/bookingcustomer.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7c46-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f7c46-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c46-124">Response</span></span>
<span data-ttu-id="f7c46-125">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c46-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c46-126">Пример</span><span class="sxs-lookup"><span data-stu-id="f7c46-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7c46-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7c46-127">Request</span></span>
<span data-ttu-id="f7c46-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7c46-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7c46-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7c46-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7c46-130">C#</span><span class="sxs-lookup"><span data-stu-id="f7c46-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7c46-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7c46-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7c46-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f7c46-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f7c46-133">В тексте запроса добавьте представление объекта [букингкустомер](../resources/bookingcustomer.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7c46-133">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f7c46-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7c46-134">Response</span></span>
<span data-ttu-id="f7c46-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7c46-135">The following is an example of the response.</span></span> <span data-ttu-id="f7c46-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f7c46-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7c46-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7c46-137">All of the properties will be returned from an actual call.</span></span>
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
