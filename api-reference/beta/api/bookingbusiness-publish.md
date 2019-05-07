---
title: 'Букингбусинесс: публикация'
description: Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a9c5cafec51b1e1c6826f308255e7c4c76756f87
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636207"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="bea5e-103">Букингбусинесс: публикация</span><span class="sxs-lookup"><span data-stu-id="bea5e-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bea5e-104">Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.</span><span class="sxs-lookup"><span data-stu-id="bea5e-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="bea5e-105">Задайте для свойства **публикации** значение true, а свойству **ПУБЛИКУРЛ** — URL-адрес страницы планирования.</span><span class="sxs-lookup"><span data-stu-id="bea5e-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="bea5e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bea5e-106">Permissions</span></span>
<span data-ttu-id="bea5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea5e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bea5e-109">Permission type</span></span>      | <span data-ttu-id="bea5e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bea5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bea5e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bea5e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="bea5e-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="bea5e-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bea5e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bea5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bea5e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea5e-114">Not supported.</span></span>   |
|<span data-ttu-id="bea5e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bea5e-115">Application</span></span> | <span data-ttu-id="bea5e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea5e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bea5e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bea5e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="bea5e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bea5e-118">Request headers</span></span>
| <span data-ttu-id="bea5e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bea5e-119">Name</span></span>       | <span data-ttu-id="bea5e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bea5e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bea5e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bea5e-121">Authorization</span></span>  | <span data-ttu-id="bea5e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bea5e-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bea5e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bea5e-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bea5e-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea5e-124">Response</span></span>
<span data-ttu-id="bea5e-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bea5e-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bea5e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="bea5e-127">Example</span></span>
<span data-ttu-id="bea5e-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bea5e-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bea5e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bea5e-129">Request</span></span>
<span data-ttu-id="bea5e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bea5e-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="bea5e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea5e-131">Response</span></span>
<span data-ttu-id="bea5e-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bea5e-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bea5e-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="bea5e-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bea5e-134">Языках</span><span class="sxs-lookup"><span data-stu-id="bea5e-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bea5e-135">Язык</span><span class="sxs-lookup"><span data-stu-id="bea5e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
