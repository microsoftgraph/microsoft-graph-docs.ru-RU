---
title: 'Букингбусинесс: Отмена публикации'
description: Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 8d84d2b11895cd29b997a9049b31035956535426
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441153"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="a5a52-103">Букингбусинесс: Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="a5a52-103">bookingBusiness: unpublish</span></span>

<span data-ttu-id="a5a52-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a5a52-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5a52-105">Сделайте страницу планирования этого бизнеса недоступной для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="a5a52-105">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="a5a52-106">Задайте для свойства **publishs** значение false, а свойству **публикурл** — значение null.</span><span class="sxs-lookup"><span data-stu-id="a5a52-106">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5a52-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a52-107">Permissions</span></span>
<span data-ttu-id="a5a52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5a52-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a52-110">Permission type</span></span>      | <span data-ttu-id="a5a52-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5a52-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5a52-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5a52-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5a52-113">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="a5a52-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a5a52-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5a52-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5a52-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a52-115">Not supported.</span></span>   |
|<span data-ttu-id="a5a52-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5a52-116">Application</span></span> | <span data-ttu-id="a5a52-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a52-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a5a52-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5a52-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="a5a52-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5a52-119">Request headers</span></span>
| <span data-ttu-id="a5a52-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a5a52-120">Name</span></span>       | <span data-ttu-id="a5a52-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a52-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a5a52-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5a52-122">Authorization</span></span>  | <span data-ttu-id="a5a52-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a5a52-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5a52-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5a52-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a5a52-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a52-125">Response</span></span>
<span data-ttu-id="a5a52-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a5a52-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5a52-128">Пример</span><span class="sxs-lookup"><span data-stu-id="a5a52-128">Example</span></span>
<span data-ttu-id="a5a52-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a5a52-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a5a52-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5a52-130">Request</span></span>
<span data-ttu-id="a5a52-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5a52-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5a52-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5a52-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="c"></a>[<span data-ttu-id="a5a52-133">C#</span><span class="sxs-lookup"><span data-stu-id="a5a52-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5a52-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5a52-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5a52-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5a52-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5a52-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a52-136">Response</span></span>
<span data-ttu-id="a5a52-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a52-137">The following is an example of the response.</span></span>
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
