---
title: 'Букингбусинесс: Отмена публикации'
description: Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ce60406347dbf6e0d0964976929614c696fd04b7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960572"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="42c91-103">Букингбусинесс: Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="42c91-103">bookingBusiness: unpublish</span></span>

<span data-ttu-id="42c91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42c91-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42c91-105">Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="42c91-105">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="42c91-106">Задайте для свойства **publishs** значение false, а свойству **публикурл** — значение null.</span><span class="sxs-lookup"><span data-stu-id="42c91-106">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="42c91-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42c91-107">Permissions</span></span>
<span data-ttu-id="42c91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42c91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42c91-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42c91-110">Permission type</span></span>      | <span data-ttu-id="42c91-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42c91-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42c91-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42c91-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="42c91-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="42c91-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="42c91-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42c91-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42c91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42c91-115">Not supported.</span></span>   |
|<span data-ttu-id="42c91-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42c91-116">Application</span></span> | <span data-ttu-id="42c91-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42c91-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="42c91-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42c91-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="42c91-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42c91-119">Request headers</span></span>
| <span data-ttu-id="42c91-120">Имя</span><span class="sxs-lookup"><span data-stu-id="42c91-120">Name</span></span>       | <span data-ttu-id="42c91-121">Описание</span><span class="sxs-lookup"><span data-stu-id="42c91-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42c91-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42c91-122">Authorization</span></span>  | <span data-ttu-id="42c91-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="42c91-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="42c91-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42c91-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="42c91-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="42c91-125">Response</span></span>
<span data-ttu-id="42c91-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="42c91-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42c91-128">Пример</span><span class="sxs-lookup"><span data-stu-id="42c91-128">Example</span></span>
<span data-ttu-id="42c91-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="42c91-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="42c91-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="42c91-130">Request</span></span>
<span data-ttu-id="42c91-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42c91-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42c91-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="42c91-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="c"></a>[<span data-ttu-id="42c91-133">C#</span><span class="sxs-lookup"><span data-stu-id="42c91-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42c91-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42c91-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42c91-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42c91-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42c91-136">Java</span><span class="sxs-lookup"><span data-stu-id="42c91-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="42c91-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="42c91-137">Response</span></span>
<span data-ttu-id="42c91-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42c91-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


