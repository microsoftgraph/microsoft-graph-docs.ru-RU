---
title: Создание bookingCustomer
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ea534616c35f2ca43c7fb5b0b5169cc935aef1d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819455"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="19b51-104">Создание bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="19b51-104">Create bookingCustomer</span></span>

 > <span data-ttu-id="19b51-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19b51-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19b51-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b51-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="19b51-107">Создание нового объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="19b51-107">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="19b51-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19b51-108">Permissions</span></span>
<span data-ttu-id="19b51-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b51-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19b51-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19b51-111">Permission type</span></span>      | <span data-ttu-id="19b51-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19b51-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19b51-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19b51-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="19b51-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="19b51-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="19b51-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19b51-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19b51-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b51-116">Not supported.</span></span>   |
|<span data-ttu-id="19b51-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19b51-117">Application</span></span> | <span data-ttu-id="19b51-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b51-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="19b51-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19b51-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="19b51-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19b51-120">Request headers</span></span>
| <span data-ttu-id="19b51-121">Имя</span><span class="sxs-lookup"><span data-stu-id="19b51-121">Name</span></span>       | <span data-ttu-id="19b51-122">Описание</span><span class="sxs-lookup"><span data-stu-id="19b51-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19b51-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19b51-123">Authorization</span></span>  | <span data-ttu-id="19b51-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="19b51-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b51-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19b51-125">Request body</span></span>
<span data-ttu-id="19b51-126">В тексте запроса укажите представление JSON объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="19b51-126">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="19b51-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="19b51-127">Response</span></span>
<span data-ttu-id="19b51-128">Успешно завершена, этот метод возвращает `201, Created` объект [bookingCustomer](../resources/bookingcustomer.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19b51-128">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b51-129">Пример</span><span class="sxs-lookup"><span data-stu-id="19b51-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19b51-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="19b51-130">Request</span></span>
<span data-ttu-id="19b51-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19b51-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="19b51-132">В тексте запроса укажите представление JSON объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="19b51-132">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="19b51-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="19b51-133">Response</span></span>
<span data-ttu-id="19b51-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="19b51-134">The following is an example of the response.</span></span> <span data-ttu-id="19b51-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="19b51-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="19b51-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19b51-136">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
