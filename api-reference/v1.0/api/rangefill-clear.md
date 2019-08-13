---
title: 'RangeFill: clear'
description: Сбрасывает фон диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cc9e6306f99cd746160973e81e2b7f58774cd951
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373779"
---
# <a name="rangefill-clear"></a><span data-ttu-id="96825-103">RangeFill: clear</span><span class="sxs-lookup"><span data-stu-id="96825-103">RangeFill: clear</span></span>

<span data-ttu-id="96825-104">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="96825-104">Resets the range background.</span></span>
## <a name="permissions"></a><span data-ttu-id="96825-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96825-105">Permissions</span></span>
<span data-ttu-id="96825-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96825-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96825-108">Permission type</span></span>      | <span data-ttu-id="96825-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96825-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96825-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96825-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96825-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96825-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96825-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96825-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96825-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96825-113">Not supported.</span></span>    |
|<span data-ttu-id="96825-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96825-114">Application</span></span> | <span data-ttu-id="96825-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96825-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96825-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96825-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/fill/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/fill/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="96825-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96825-117">Request headers</span></span>
| <span data-ttu-id="96825-118">Имя</span><span class="sxs-lookup"><span data-stu-id="96825-118">Name</span></span>       | <span data-ttu-id="96825-119">Описание</span><span class="sxs-lookup"><span data-stu-id="96825-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96825-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96825-120">Authorization</span></span>  | <span data-ttu-id="96825-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96825-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96825-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96825-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="96825-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="96825-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96825-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96825-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="96825-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="96825-127">Response</span></span>

<span data-ttu-id="96825-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="96825-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96825-130">Пример</span><span class="sxs-lookup"><span data-stu-id="96825-130">Example</span></span>
<span data-ttu-id="96825-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="96825-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="96825-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96825-132">Request</span></span>
<span data-ttu-id="96825-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96825-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96825-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96825-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangefill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96825-135">C#</span><span class="sxs-lookup"><span data-stu-id="96825-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangefill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96825-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96825-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangefill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96825-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="96825-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangefill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96825-138">Java</span><span class="sxs-lookup"><span data-stu-id="96825-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangefill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96825-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="96825-139">Response</span></span>
<span data-ttu-id="96825-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96825-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
