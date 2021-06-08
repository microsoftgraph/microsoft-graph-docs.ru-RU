---
title: 'bookingBusiness: публикация'
description: Сделайте страницу планирования этого бизнеса доступной для внешних клиентов.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d60a88324cd86cd599fc9986dfa3b6d1a4f737ea
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786589"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="ed331-103">bookingBusiness: публикация</span><span class="sxs-lookup"><span data-stu-id="ed331-103">bookingBusiness: publish</span></span>

<span data-ttu-id="ed331-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed331-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed331-105">Сделайте страницу планирования этого бизнеса доступной для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="ed331-105">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="ed331-106">Установите **свойство isPublished** для true и **publicUrl** на URL-адрес страницы планирования.</span><span class="sxs-lookup"><span data-stu-id="ed331-106">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed331-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed331-107">Permissions</span></span>
<span data-ttu-id="ed331-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed331-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed331-110">Permission type</span></span>      | <span data-ttu-id="ed331-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed331-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed331-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed331-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ed331-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ed331-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ed331-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed331-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed331-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed331-115">Not supported.</span></span>   |
|<span data-ttu-id="ed331-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed331-116">Application</span></span> | <span data-ttu-id="ed331-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed331-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ed331-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed331-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="ed331-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed331-119">Request headers</span></span>
| <span data-ttu-id="ed331-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ed331-120">Name</span></span>       | <span data-ttu-id="ed331-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ed331-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed331-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed331-122">Authorization</span></span>  | <span data-ttu-id="ed331-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ed331-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed331-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed331-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ed331-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed331-125">Response</span></span>
<span data-ttu-id="ed331-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ed331-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed331-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ed331-128">Example</span></span>
<span data-ttu-id="ed331-129">Ниже приводится пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ed331-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ed331-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed331-130">Request</span></span>
<span data-ttu-id="ed331-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed331-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed331-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed331-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="c"></a>[<span data-ttu-id="ed331-133">C#</span><span class="sxs-lookup"><span data-stu-id="ed331-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed331-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed331-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed331-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed331-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed331-136">Java</span><span class="sxs-lookup"><span data-stu-id="ed331-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed331-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed331-137">Response</span></span>
<span data-ttu-id="ed331-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ed331-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


