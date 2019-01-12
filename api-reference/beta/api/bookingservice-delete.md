---
title: Удаление bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7616e04c25aefedde084fc47c06d22410f9f0fee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991225"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="9712d-104">Удаление bookingService</span><span class="sxs-lookup"><span data-stu-id="9712d-104">Delete bookingService</span></span>

 > <span data-ttu-id="9712d-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9712d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9712d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9712d-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9712d-107">Удаление объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="9712d-107">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9712d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9712d-108">Permissions</span></span>
<span data-ttu-id="9712d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9712d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9712d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9712d-111">Permission type</span></span>      | <span data-ttu-id="9712d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9712d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9712d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9712d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9712d-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="9712d-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9712d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9712d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9712d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9712d-116">Not supported.</span></span>   |
|<span data-ttu-id="9712d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9712d-117">Application</span></span> | <span data-ttu-id="9712d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9712d-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9712d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9712d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9712d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9712d-120">Request headers</span></span>
| <span data-ttu-id="9712d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9712d-121">Name</span></span>       | <span data-ttu-id="9712d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9712d-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9712d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9712d-123">Authorization</span></span>  | <span data-ttu-id="9712d-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9712d-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9712d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9712d-125">Request body</span></span>
<span data-ttu-id="9712d-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9712d-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9712d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9712d-127">Response</span></span>
<span data-ttu-id="9712d-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9712d-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9712d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9712d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9712d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9712d-131">Request</span></span>
<span data-ttu-id="9712d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9712d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="9712d-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9712d-133">Response</span></span>
<span data-ttu-id="9712d-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9712d-134">The following is an example of the response.</span></span> <span data-ttu-id="9712d-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9712d-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9712d-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9712d-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
