---
title: 'Букингбусинесс: Отмена публикации'
description: Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b56397200ffa0d450db6099540a4cfccb4c4339f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257934"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="f36c2-103">Букингбусинесс: Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="f36c2-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f36c2-104">Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="f36c2-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="f36c2-105">Задайте для \*\*\*\* свойства publishs значение false, а свойству **публикурл** — значение null.</span><span class="sxs-lookup"><span data-stu-id="f36c2-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="f36c2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f36c2-106">Permissions</span></span>
<span data-ttu-id="f36c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f36c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f36c2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f36c2-109">Permission type</span></span>      | <span data-ttu-id="f36c2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f36c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f36c2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f36c2-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f36c2-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="f36c2-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f36c2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f36c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f36c2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f36c2-114">Not supported.</span></span>   |
|<span data-ttu-id="f36c2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f36c2-115">Application</span></span> | <span data-ttu-id="f36c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f36c2-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f36c2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f36c2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="f36c2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f36c2-118">Request headers</span></span>
| <span data-ttu-id="f36c2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f36c2-119">Name</span></span>       | <span data-ttu-id="f36c2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f36c2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f36c2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f36c2-121">Authorization</span></span>  | <span data-ttu-id="f36c2-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f36c2-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f36c2-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f36c2-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f36c2-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="f36c2-124">Response</span></span>
<span data-ttu-id="f36c2-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f36c2-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f36c2-127">Пример</span><span class="sxs-lookup"><span data-stu-id="f36c2-127">Example</span></span>
<span data-ttu-id="f36c2-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f36c2-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f36c2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f36c2-129">Request</span></span>
<span data-ttu-id="f36c2-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f36c2-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="f36c2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f36c2-131">Response</span></span>
<span data-ttu-id="f36c2-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f36c2-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f36c2-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f36c2-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f36c2-134">C#</span><span class="sxs-lookup"><span data-stu-id="f36c2-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f36c2-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="f36c2-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f36c2-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f36c2-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
