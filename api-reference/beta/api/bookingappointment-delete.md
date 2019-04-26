---
title: Удаление Букингаппоинтмент
description: Удаление объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 56fb3ad67736a1a754c979ba01aaf647af3992d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322534"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="30a2e-103">Удаление Букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="30a2e-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a2e-104">Удаление объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="30a2e-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="30a2e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30a2e-105">Permissions</span></span>
<span data-ttu-id="30a2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a2e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30a2e-108">Permission type</span></span>      | <span data-ttu-id="30a2e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30a2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30a2e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30a2e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="30a2e-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="30a2e-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="30a2e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30a2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30a2e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a2e-113">Not supported.</span></span>   |
|<span data-ttu-id="30a2e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30a2e-114">Application</span></span> | <span data-ttu-id="30a2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a2e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="30a2e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30a2e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="30a2e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30a2e-117">Request headers</span></span>
| <span data-ttu-id="30a2e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="30a2e-118">Name</span></span>       | <span data-ttu-id="30a2e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="30a2e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="30a2e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30a2e-120">Authorization</span></span>  | <span data-ttu-id="30a2e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="30a2e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="30a2e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30a2e-122">Request body</span></span>
<span data-ttu-id="30a2e-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30a2e-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="30a2e-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="30a2e-124">Response</span></span>
<span data-ttu-id="30a2e-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="30a2e-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30a2e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="30a2e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30a2e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a2e-128">Request</span></span>
<span data-ttu-id="30a2e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30a2e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a><span data-ttu-id="30a2e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a2e-130">Response</span></span>
<span data-ttu-id="30a2e-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30a2e-131">The following is an example of the response.</span></span> <span data-ttu-id="30a2e-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="30a2e-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="30a2e-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30a2e-133">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
