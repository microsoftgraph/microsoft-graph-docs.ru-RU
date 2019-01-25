---
title: Удаление bookingAppointment
description: Удалите bookingAppointment в указанном bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a8abe1961be7e3caf36c9d690497347f42c83fde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513720"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="6a69f-103">Удаление bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="6a69f-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a69f-104">Удалите [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6a69f-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6a69f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a69f-105">Permissions</span></span>
<span data-ttu-id="6a69f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a69f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a69f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a69f-108">Permission type</span></span>      | <span data-ttu-id="6a69f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a69f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a69f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a69f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6a69f-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6a69f-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6a69f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a69f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a69f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a69f-113">Not supported.</span></span>   |
|<span data-ttu-id="6a69f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a69f-114">Application</span></span> | <span data-ttu-id="6a69f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a69f-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6a69f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a69f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6a69f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a69f-117">Request headers</span></span>
| <span data-ttu-id="6a69f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6a69f-118">Name</span></span>       | <span data-ttu-id="6a69f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6a69f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6a69f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a69f-120">Authorization</span></span>  | <span data-ttu-id="6a69f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6a69f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a69f-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a69f-122">Request body</span></span>
<span data-ttu-id="6a69f-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a69f-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6a69f-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a69f-124">Response</span></span>
<span data-ttu-id="6a69f-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6a69f-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a69f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6a69f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a69f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a69f-128">Request</span></span>
<span data-ttu-id="6a69f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a69f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="6a69f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a69f-130">Response</span></span>
<span data-ttu-id="6a69f-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a69f-131">The following is an example of the response.</span></span> <span data-ttu-id="6a69f-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6a69f-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6a69f-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a69f-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
