---
title: 'Букингбусинесс: публикация'
description: Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 75f831870d0dee616c3d902db4321abc729a3682
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419480"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="01caa-103">Букингбусинесс: публикация</span><span class="sxs-lookup"><span data-stu-id="01caa-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01caa-104">Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.</span><span class="sxs-lookup"><span data-stu-id="01caa-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="01caa-105">Задайте для свойства **публикации** значение true, а свойству **публикурл** — URL-адрес страницы планирования.</span><span class="sxs-lookup"><span data-stu-id="01caa-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="01caa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01caa-106">Permissions</span></span>
<span data-ttu-id="01caa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01caa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01caa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01caa-109">Permission type</span></span>      | <span data-ttu-id="01caa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01caa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01caa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01caa-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="01caa-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="01caa-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="01caa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01caa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01caa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01caa-114">Not supported.</span></span>   |
|<span data-ttu-id="01caa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01caa-115">Application</span></span> | <span data-ttu-id="01caa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01caa-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="01caa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01caa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="01caa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01caa-118">Request headers</span></span>
| <span data-ttu-id="01caa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="01caa-119">Name</span></span>       | <span data-ttu-id="01caa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="01caa-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01caa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01caa-121">Authorization</span></span>  | <span data-ttu-id="01caa-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="01caa-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="01caa-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01caa-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="01caa-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="01caa-124">Response</span></span>
<span data-ttu-id="01caa-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="01caa-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01caa-127">Пример</span><span class="sxs-lookup"><span data-stu-id="01caa-127">Example</span></span>
<span data-ttu-id="01caa-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="01caa-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01caa-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="01caa-129">Request</span></span>
<span data-ttu-id="01caa-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01caa-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01caa-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="01caa-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01caa-132">C#</span><span class="sxs-lookup"><span data-stu-id="01caa-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01caa-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01caa-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01caa-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="01caa-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="01caa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="01caa-135">Response</span></span>
<span data-ttu-id="01caa-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="01caa-136">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
