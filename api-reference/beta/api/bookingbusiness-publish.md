---
title: 'Букингбусинесс: публикация'
description: Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b8ee635da938a53dff4603bb50f4903f0a000253
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441167"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="d9f41-103">Букингбусинесс: публикация</span><span class="sxs-lookup"><span data-stu-id="d9f41-103">bookingBusiness: publish</span></span>

<span data-ttu-id="d9f41-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d9f41-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9f41-105">Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.</span><span class="sxs-lookup"><span data-stu-id="d9f41-105">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="d9f41-106">Задайте для свойства **публикации** значение true, а свойству **публикурл** — URL-адрес страницы планирования.</span><span class="sxs-lookup"><span data-stu-id="d9f41-106">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9f41-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f41-107">Permissions</span></span>
<span data-ttu-id="d9f41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9f41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f41-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f41-110">Permission type</span></span>      | <span data-ttu-id="d9f41-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9f41-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9f41-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9f41-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9f41-113">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="d9f41-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d9f41-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9f41-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f41-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9f41-115">Not supported.</span></span>   |
|<span data-ttu-id="d9f41-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9f41-116">Application</span></span> | <span data-ttu-id="d9f41-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9f41-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d9f41-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9f41-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="d9f41-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9f41-119">Request headers</span></span>
| <span data-ttu-id="d9f41-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d9f41-120">Name</span></span>       | <span data-ttu-id="d9f41-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9f41-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9f41-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9f41-122">Authorization</span></span>  | <span data-ttu-id="d9f41-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d9f41-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9f41-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9f41-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d9f41-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9f41-125">Response</span></span>
<span data-ttu-id="d9f41-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d9f41-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9f41-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d9f41-128">Example</span></span>
<span data-ttu-id="d9f41-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d9f41-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9f41-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9f41-130">Request</span></span>
<span data-ttu-id="d9f41-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9f41-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9f41-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9f41-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="c"></a>[<span data-ttu-id="d9f41-133">C#</span><span class="sxs-lookup"><span data-stu-id="d9f41-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9f41-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9f41-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9f41-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9f41-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d9f41-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9f41-136">Response</span></span>
<span data-ttu-id="d9f41-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d9f41-137">The following is an example of the response.</span></span>
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
