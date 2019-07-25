---
title: 'Букингбусинесс: Отмена публикации'
description: Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: df4f9fb74ab0cc82394a90b938f1b7478c99cd07
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865521"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="c066d-103">Букингбусинесс: Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="c066d-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c066d-104">Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="c066d-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="c066d-105">Задайте для \*\*\*\* свойства publishs значение false, а свойству **публикурл** — значение null.</span><span class="sxs-lookup"><span data-stu-id="c066d-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="c066d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c066d-106">Permissions</span></span>
<span data-ttu-id="c066d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c066d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c066d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c066d-109">Permission type</span></span>      | <span data-ttu-id="c066d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c066d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c066d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c066d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c066d-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="c066d-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c066d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c066d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c066d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c066d-114">Not supported.</span></span>   |
|<span data-ttu-id="c066d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c066d-115">Application</span></span> | <span data-ttu-id="c066d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c066d-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c066d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c066d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="c066d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c066d-118">Request headers</span></span>
| <span data-ttu-id="c066d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c066d-119">Name</span></span>       | <span data-ttu-id="c066d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c066d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c066d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c066d-121">Authorization</span></span>  | <span data-ttu-id="c066d-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c066d-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c066d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c066d-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c066d-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="c066d-124">Response</span></span>
<span data-ttu-id="c066d-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c066d-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c066d-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c066d-127">Example</span></span>
<span data-ttu-id="c066d-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c066d-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c066d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c066d-129">Request</span></span>
<span data-ttu-id="c066d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c066d-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c066d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c066d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c066d-132">C#</span><span class="sxs-lookup"><span data-stu-id="c066d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c066d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c066d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c066d-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c066d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c066d-135">Java</span><span class="sxs-lookup"><span data-stu-id="c066d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c066d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c066d-136">Response</span></span>
<span data-ttu-id="c066d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c066d-137">The following is an example of the response.</span></span>
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
