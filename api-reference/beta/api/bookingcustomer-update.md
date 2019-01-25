---
title: Обновление bookingcustomer
description: Обновление свойства объекта bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 90de81666335c1825e1d134f9b898ee4b6561664
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525313"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="0a999-103">Обновление bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="0a999-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a999-104">Обновление свойства объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="0a999-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a999-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a999-105">Permissions</span></span>
<span data-ttu-id="0a999-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a999-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a999-108">Permission type</span></span>      | <span data-ttu-id="0a999-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a999-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a999-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a999-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0a999-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0a999-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0a999-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a999-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a999-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a999-113">Not supported.</span></span>   |
|<span data-ttu-id="0a999-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a999-114">Application</span></span> | <span data-ttu-id="0a999-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a999-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0a999-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a999-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0a999-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a999-117">Optional request headers</span></span>
| <span data-ttu-id="0a999-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0a999-118">Name</span></span>       | <span data-ttu-id="0a999-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0a999-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0a999-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a999-120">Authorization</span></span>  | <span data-ttu-id="0a999-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0a999-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a999-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a999-122">Request body</span></span>
<span data-ttu-id="0a999-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0a999-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0a999-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a999-126">Property</span></span>     | <span data-ttu-id="0a999-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0a999-127">Type</span></span>   |<span data-ttu-id="0a999-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0a999-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a999-129">displayName</span><span class="sxs-lookup"><span data-stu-id="0a999-129">displayName</span></span>|<span data-ttu-id="0a999-130">Строка</span><span class="sxs-lookup"><span data-stu-id="0a999-130">String</span></span>|<span data-ttu-id="0a999-131">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="0a999-131">The name of the customer.</span></span>|
|<span data-ttu-id="0a999-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0a999-132">emailAddress</span></span>|<span data-ttu-id="0a999-133">String</span><span class="sxs-lookup"><span data-stu-id="0a999-133">String</span></span>|<span data-ttu-id="0a999-134">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="0a999-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="0a999-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a999-135">Response</span></span>
<span data-ttu-id="0a999-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [bookingCustomer](../resources/bookingcustomer.md) объект в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a999-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a999-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0a999-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a999-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a999-138">Request</span></span>
<span data-ttu-id="0a999-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a999-139">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0a999-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a999-140">Response</span></span>
<span data-ttu-id="0a999-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a999-141">The following is an example of the response.</span></span> <span data-ttu-id="0a999-142">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0a999-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a999-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a999-143">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingcustomer-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
