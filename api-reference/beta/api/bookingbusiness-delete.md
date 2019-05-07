---
title: Удаление Букингбусинесс
description: Удаление объекта Букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f296796d42e8d8461b91cdb0950149690b227eb6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636347"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="9e420-103">Удаление Букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="9e420-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e420-104">Удаление объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="9e420-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e420-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e420-105">Permissions</span></span>
<span data-ttu-id="9e420-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e420-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e420-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e420-108">Permission type</span></span>      | <span data-ttu-id="9e420-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e420-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e420-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e420-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9e420-111">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="9e420-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9e420-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e420-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e420-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e420-113">Not supported.</span></span>   |
|<span data-ttu-id="9e420-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e420-114">Application</span></span> | <span data-ttu-id="9e420-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e420-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9e420-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e420-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="9e420-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e420-117">Request headers</span></span>
| <span data-ttu-id="9e420-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9e420-118">Name</span></span>       | <span data-ttu-id="9e420-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9e420-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e420-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e420-120">Authorization</span></span>  | <span data-ttu-id="9e420-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9e420-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e420-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e420-122">Request body</span></span>
<span data-ttu-id="9e420-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e420-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9e420-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e420-124">Response</span></span>
<span data-ttu-id="9e420-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9e420-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e420-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9e420-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e420-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e420-128">Request</span></span>
<span data-ttu-id="9e420-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e420-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="9e420-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e420-130">Response</span></span>
<span data-ttu-id="9e420-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e420-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9e420-132">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9e420-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9e420-133">Языках</span><span class="sxs-lookup"><span data-stu-id="9e420-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e420-134">Язык</span><span class="sxs-lookup"><span data-stu-id="9e420-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingbusiness-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
