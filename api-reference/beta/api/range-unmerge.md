---
title: 'Range: unmerge'
description: Разъединяет ячейки диапазона на отдельные ячейки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d0230892eda37fb3a5d1d18342085da8b779c415
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874712"
---
# <a name="range-unmerge"></a><span data-ttu-id="e5d53-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="e5d53-103">Range: unmerge</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5d53-104">Разъединяет ячейки диапазона на отдельные ячейки.</span><span class="sxs-lookup"><span data-stu-id="e5d53-104">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5d53-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5d53-105">Permissions</span></span>
<span data-ttu-id="e5d53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5d53-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5d53-108">Permission type</span></span>      | <span data-ttu-id="e5d53-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5d53-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5d53-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5d53-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5d53-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5d53-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5d53-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5d53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5d53-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5d53-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5d53-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5d53-114">Application</span></span> | <span data-ttu-id="e5d53-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d53-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5d53-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5d53-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="e5d53-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5d53-117">Request headers</span></span>
| <span data-ttu-id="e5d53-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e5d53-118">Name</span></span>       | <span data-ttu-id="e5d53-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d53-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5d53-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5d53-120">Authorization</span></span>  | <span data-ttu-id="e5d53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5d53-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5d53-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5d53-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5d53-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e5d53-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5d53-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5d53-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e5d53-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5d53-127">Response</span></span>

<span data-ttu-id="e5d53-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e5d53-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5d53-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5d53-130">Example</span></span>
<span data-ttu-id="e5d53-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e5d53-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5d53-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5d53-132">Request</span></span>
<span data-ttu-id="e5d53-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5d53-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e5d53-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5d53-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e5d53-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5d53-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-unmerge-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5d53-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e5d53-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-unmerge-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5d53-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e5d53-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-unmerge-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e5d53-138">Java</span><span class="sxs-lookup"><span data-stu-id="e5d53-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-unmerge-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5d53-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5d53-139">Response</span></span>
<span data-ttu-id="e5d53-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5d53-140">Here is an example of the response.</span></span> 
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
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
