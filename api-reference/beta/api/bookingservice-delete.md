---
title: Удаление bookingService
description: Удаление объекта bookingService в указанном bookingbusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: c7ba9cb20e7f9f401d7b9651d408549272b32875
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047814"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="0aa47-103">Удаление bookingService</span><span class="sxs-lookup"><span data-stu-id="0aa47-103">Delete bookingService</span></span>

<span data-ttu-id="0aa47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aa47-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aa47-105">Удаление объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="0aa47-105">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0aa47-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0aa47-106">Permissions</span></span>
<span data-ttu-id="0aa47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aa47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aa47-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0aa47-109">Permission type</span></span>      | <span data-ttu-id="0aa47-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0aa47-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aa47-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0aa47-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0aa47-112">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0aa47-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0aa47-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0aa47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aa47-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aa47-114">Not supported.</span></span>   |
|<span data-ttu-id="0aa47-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0aa47-115">Application</span></span> | <span data-ttu-id="0aa47-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0aa47-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0aa47-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0aa47-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0aa47-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0aa47-118">Request headers</span></span>
| <span data-ttu-id="0aa47-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0aa47-119">Name</span></span>       | <span data-ttu-id="0aa47-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0aa47-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0aa47-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0aa47-121">Authorization</span></span>  | <span data-ttu-id="0aa47-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0aa47-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aa47-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0aa47-123">Request body</span></span>
<span data-ttu-id="0aa47-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0aa47-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0aa47-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0aa47-125">Response</span></span>
<span data-ttu-id="0aa47-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0aa47-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aa47-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0aa47-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0aa47-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0aa47-129">Request</span></span>
<span data-ttu-id="0aa47-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0aa47-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0aa47-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0aa47-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="c"></a>[<span data-ttu-id="0aa47-132">C#</span><span class="sxs-lookup"><span data-stu-id="0aa47-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0aa47-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0aa47-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0aa47-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0aa47-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0aa47-135">Java</span><span class="sxs-lookup"><span data-stu-id="0aa47-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0aa47-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0aa47-136">Response</span></span>
<span data-ttu-id="0aa47-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0aa47-137">The following is an example of the response.</span></span> <span data-ttu-id="0aa47-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0aa47-138">Note: The response object shown here might be shortened for readability.</span></span>
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


