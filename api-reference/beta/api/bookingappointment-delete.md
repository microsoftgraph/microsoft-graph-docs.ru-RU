---
title: Удаление Букингаппоинтмент
description: Удаление объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 44a4b02a00870bf6f9967e9eb8baf33c236f59ec
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415672"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="affd8-103">Удаление Букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="affd8-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="affd8-104">Удаление объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="affd8-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="affd8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="affd8-105">Permissions</span></span>
<span data-ttu-id="affd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="affd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="affd8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="affd8-108">Permission type</span></span>      | <span data-ttu-id="affd8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="affd8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="affd8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="affd8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="affd8-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="affd8-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="affd8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="affd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="affd8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="affd8-113">Not supported.</span></span>   |
|<span data-ttu-id="affd8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="affd8-114">Application</span></span> | <span data-ttu-id="affd8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="affd8-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="affd8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="affd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="affd8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="affd8-117">Request headers</span></span>
| <span data-ttu-id="affd8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="affd8-118">Name</span></span>       | <span data-ttu-id="affd8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="affd8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="affd8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="affd8-120">Authorization</span></span>  | <span data-ttu-id="affd8-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="affd8-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="affd8-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="affd8-122">Request body</span></span>
<span data-ttu-id="affd8-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="affd8-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="affd8-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="affd8-124">Response</span></span>
<span data-ttu-id="affd8-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="affd8-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="affd8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="affd8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="affd8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="affd8-128">Request</span></span>
<span data-ttu-id="affd8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="affd8-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="affd8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="affd8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="affd8-131">C#</span><span class="sxs-lookup"><span data-stu-id="affd8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="affd8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="affd8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="affd8-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="affd8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="affd8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="affd8-134">Response</span></span>
<span data-ttu-id="affd8-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="affd8-135">The following is an example of the response.</span></span> <span data-ttu-id="affd8-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="affd8-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="affd8-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="affd8-137">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
