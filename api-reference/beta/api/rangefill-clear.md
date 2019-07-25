---
title: 'RangeFill: clear'
description: Сбрасывает фон диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cad516285a80dc482e87418b13db6d76d6314446
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874587"
---
# <a name="rangefill-clear"></a><span data-ttu-id="be623-103">RangeFill: clear</span><span class="sxs-lookup"><span data-stu-id="be623-103">RangeFill: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be623-104">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="be623-104">Resets the range background.</span></span>
## <a name="permissions"></a><span data-ttu-id="be623-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be623-105">Permissions</span></span>
<span data-ttu-id="be623-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be623-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be623-108">Permission type</span></span>      | <span data-ttu-id="be623-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be623-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be623-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be623-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be623-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be623-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be623-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be623-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be623-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be623-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be623-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be623-114">Application</span></span> | <span data-ttu-id="be623-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be623-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be623-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be623-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/fill/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/fill/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="be623-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be623-117">Request headers</span></span>
| <span data-ttu-id="be623-118">Имя</span><span class="sxs-lookup"><span data-stu-id="be623-118">Name</span></span>       | <span data-ttu-id="be623-119">Описание</span><span class="sxs-lookup"><span data-stu-id="be623-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be623-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be623-120">Authorization</span></span>  | <span data-ttu-id="be623-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be623-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be623-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be623-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="be623-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="be623-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be623-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be623-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="be623-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="be623-127">Response</span></span>

<span data-ttu-id="be623-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="be623-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be623-130">Пример</span><span class="sxs-lookup"><span data-stu-id="be623-130">Example</span></span>
<span data-ttu-id="be623-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="be623-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="be623-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be623-132">Request</span></span>
<span data-ttu-id="be623-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be623-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be623-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="be623-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangefill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="be623-135">C#</span><span class="sxs-lookup"><span data-stu-id="be623-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rangefill-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be623-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="be623-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangefill-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be623-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="be623-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rangefill-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="be623-138">Java</span><span class="sxs-lookup"><span data-stu-id="be623-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rangefill-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="be623-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="be623-139">Response</span></span>
<span data-ttu-id="be623-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be623-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
