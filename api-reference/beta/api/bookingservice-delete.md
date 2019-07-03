---
title: Удаление Букингсервице
description: Удаление объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b570263eca174522cac0e2069909619b2e348057
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439072"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="ccefa-103">Удаление Букингсервице</span><span class="sxs-lookup"><span data-stu-id="ccefa-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccefa-104">Удаление объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="ccefa-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ccefa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccefa-105">Permissions</span></span>
<span data-ttu-id="ccefa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccefa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccefa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccefa-108">Permission type</span></span>      | <span data-ttu-id="ccefa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccefa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccefa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccefa-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ccefa-111">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="ccefa-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ccefa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccefa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccefa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccefa-113">Not supported.</span></span>   |
|<span data-ttu-id="ccefa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccefa-114">Application</span></span> | <span data-ttu-id="ccefa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccefa-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ccefa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccefa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ccefa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccefa-117">Request headers</span></span>
| <span data-ttu-id="ccefa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ccefa-118">Name</span></span>       | <span data-ttu-id="ccefa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ccefa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ccefa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccefa-120">Authorization</span></span>  | <span data-ttu-id="ccefa-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ccefa-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccefa-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccefa-122">Request body</span></span>
<span data-ttu-id="ccefa-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccefa-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ccefa-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccefa-124">Response</span></span>
<span data-ttu-id="ccefa-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ccefa-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccefa-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ccefa-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccefa-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccefa-128">Request</span></span>
<span data-ttu-id="ccefa-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccefa-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ccefa-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccefa-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ccefa-131">C#</span><span class="sxs-lookup"><span data-stu-id="ccefa-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ccefa-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="ccefa-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ccefa-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ccefa-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ccefa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccefa-134">Response</span></span>
<span data-ttu-id="ccefa-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccefa-135">The following is an example of the response.</span></span> <span data-ttu-id="ccefa-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ccefa-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ccefa-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccefa-137">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
