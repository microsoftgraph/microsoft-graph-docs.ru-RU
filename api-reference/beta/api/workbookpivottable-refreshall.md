---
title: 'workbookPivotTable: refreshAll'
description: Обновляет сводную таблицу на заданном листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5381c72427d01e1f90ff376f6e054246d8c363dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987343"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="dc6f4-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="dc6f4-103">workbookPivotTable: refreshAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc6f4-104">Обновляет сводную таблицу на заданном листе.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc6f4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc6f4-105">Permissions</span></span>
<span data-ttu-id="dc6f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc6f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc6f4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc6f4-108">Permission type</span></span>      | <span data-ttu-id="dc6f4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc6f4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc6f4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc6f4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc6f4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc6f4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc6f4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc6f4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc6f4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc6f4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc6f4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc6f4-114">Application</span></span> | <span data-ttu-id="dc6f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc6f4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc6f4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="dc6f4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc6f4-117">Request headers</span></span>
| <span data-ttu-id="dc6f4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dc6f4-118">Name</span></span>       | <span data-ttu-id="dc6f4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dc6f4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc6f4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc6f4-120">Authorization</span></span>  | <span data-ttu-id="dc6f4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc6f4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc6f4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc6f4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc6f4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc6f4-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dc6f4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc6f4-127">Response</span></span>

<span data-ttu-id="dc6f4-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc6f4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dc6f4-130">Example</span></span>
<span data-ttu-id="dc6f4-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc6f4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc6f4-132">Request</span></span>
<span data-ttu-id="dc6f4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc6f4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc6f4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc6f4-135">C#</span><span class="sxs-lookup"><span data-stu-id="dc6f4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc6f4-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc6f4-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc6f4-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dc6f4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc6f4-138">Java</span><span class="sxs-lookup"><span data-stu-id="dc6f4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refreshall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc6f4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc6f4-139">Response</span></span>
<span data-ttu-id="dc6f4-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc6f4-140">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
