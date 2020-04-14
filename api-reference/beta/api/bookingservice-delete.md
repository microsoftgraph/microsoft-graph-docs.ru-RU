---
title: Удаление Букингсервице
description: Удаление объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 72ba3311e1901dfef26459df04107a8a56331cba
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376404"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="96321-103">Удаление Букингсервице</span><span class="sxs-lookup"><span data-stu-id="96321-103">Delete bookingService</span></span>

<span data-ttu-id="96321-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96321-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96321-105">Удаление объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="96321-105">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="96321-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96321-106">Permissions</span></span>
<span data-ttu-id="96321-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96321-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96321-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96321-109">Permission type</span></span>      | <span data-ttu-id="96321-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96321-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96321-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96321-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="96321-112">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="96321-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="96321-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96321-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96321-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96321-114">Not supported.</span></span>   |
|<span data-ttu-id="96321-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96321-115">Application</span></span> | <span data-ttu-id="96321-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96321-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="96321-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96321-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="96321-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96321-118">Request headers</span></span>
| <span data-ttu-id="96321-119">Имя</span><span class="sxs-lookup"><span data-stu-id="96321-119">Name</span></span>       | <span data-ttu-id="96321-120">Описание</span><span class="sxs-lookup"><span data-stu-id="96321-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96321-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96321-121">Authorization</span></span>  | <span data-ttu-id="96321-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="96321-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="96321-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96321-123">Request body</span></span>
<span data-ttu-id="96321-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96321-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="96321-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="96321-125">Response</span></span>
<span data-ttu-id="96321-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="96321-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96321-128">Пример</span><span class="sxs-lookup"><span data-stu-id="96321-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96321-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="96321-129">Request</span></span>
<span data-ttu-id="96321-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96321-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96321-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="96321-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="c"></a>[<span data-ttu-id="96321-132">C#</span><span class="sxs-lookup"><span data-stu-id="96321-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96321-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96321-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96321-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96321-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96321-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="96321-135">Response</span></span>
<span data-ttu-id="96321-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96321-136">The following is an example of the response.</span></span> <span data-ttu-id="96321-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="96321-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="96321-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96321-138">All of the properties will be returned from an actual call.</span></span>
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
