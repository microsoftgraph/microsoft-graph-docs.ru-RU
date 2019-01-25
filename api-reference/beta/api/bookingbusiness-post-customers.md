---
title: Создание bookingCustomer
description: Создание нового объекта bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4557d65edf4727659fdae94599c0796fc940ed1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523962"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="74800-103">Создание bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="74800-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74800-104">Создание нового объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="74800-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="74800-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74800-105">Permissions</span></span>
<span data-ttu-id="74800-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74800-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74800-108">Permission type</span></span>      | <span data-ttu-id="74800-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74800-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74800-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74800-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="74800-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="74800-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="74800-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74800-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74800-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74800-113">Not supported.</span></span>   |
|<span data-ttu-id="74800-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74800-114">Application</span></span> | <span data-ttu-id="74800-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74800-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="74800-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74800-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="74800-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74800-117">Request headers</span></span>
| <span data-ttu-id="74800-118">Имя</span><span class="sxs-lookup"><span data-stu-id="74800-118">Name</span></span>       | <span data-ttu-id="74800-119">Описание</span><span class="sxs-lookup"><span data-stu-id="74800-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74800-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="74800-120">Authorization</span></span>  | <span data-ttu-id="74800-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="74800-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="74800-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74800-122">Request body</span></span>
<span data-ttu-id="74800-123">В тексте запроса укажите представление JSON объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="74800-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="74800-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="74800-124">Response</span></span>
<span data-ttu-id="74800-125">Успешно завершена, этот метод возвращает `201, Created` объект [bookingCustomer](../resources/bookingcustomer.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74800-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74800-126">Пример</span><span class="sxs-lookup"><span data-stu-id="74800-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74800-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="74800-127">Request</span></span>
<span data-ttu-id="74800-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74800-128">The following is an example of the request.</span></span>
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
<span data-ttu-id="74800-129">В тексте запроса укажите представление JSON объекта [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="74800-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="74800-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="74800-130">Response</span></span>
<span data-ttu-id="74800-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="74800-131">The following is an example of the response.</span></span> <span data-ttu-id="74800-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="74800-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="74800-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74800-133">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
