---
title: 'Букингбусинесс: Отмена публикации'
description: Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd34e752ef303c6aacb5bc8257e2b73d2050c6b5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439156"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="430f9-103">Букингбусинесс: Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="430f9-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="430f9-104">Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="430f9-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="430f9-105">Задайте для \*\*\*\* свойства publishs значение false, а свойству **публикурл** — значение null.</span><span class="sxs-lookup"><span data-stu-id="430f9-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="430f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="430f9-106">Permissions</span></span>
<span data-ttu-id="430f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="430f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="430f9-109">Permission type</span></span>      | <span data-ttu-id="430f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="430f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="430f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="430f9-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="430f9-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="430f9-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="430f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="430f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="430f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430f9-114">Not supported.</span></span>   |
|<span data-ttu-id="430f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="430f9-115">Application</span></span> | <span data-ttu-id="430f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430f9-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="430f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="430f9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="430f9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="430f9-118">Request headers</span></span>
| <span data-ttu-id="430f9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="430f9-119">Name</span></span>       | <span data-ttu-id="430f9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="430f9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="430f9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="430f9-121">Authorization</span></span>  | <span data-ttu-id="430f9-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="430f9-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="430f9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="430f9-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="430f9-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="430f9-124">Response</span></span>
<span data-ttu-id="430f9-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="430f9-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430f9-127">Пример</span><span class="sxs-lookup"><span data-stu-id="430f9-127">Example</span></span>
<span data-ttu-id="430f9-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="430f9-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="430f9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="430f9-129">Request</span></span>
<span data-ttu-id="430f9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="430f9-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="430f9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="430f9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="430f9-132">C#</span><span class="sxs-lookup"><span data-stu-id="430f9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="430f9-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="430f9-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="430f9-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="430f9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="430f9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="430f9-135">Response</span></span>
<span data-ttu-id="430f9-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="430f9-136">The following is an example of the response.</span></span>
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
