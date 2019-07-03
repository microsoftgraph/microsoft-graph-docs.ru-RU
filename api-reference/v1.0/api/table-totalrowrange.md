---
title: 'Table: TotalRowRange'
description: Получает объект диапазона, связанный со строкой итогов таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4aa4d326515d31e8bda92339d6accd1492983734
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445585"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="1f42b-103">Table: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="1f42b-103">Table: TotalRowRange</span></span>

<span data-ttu-id="1f42b-104">Получает объект диапазона, связанный со строкой итогов таблицы.</span><span class="sxs-lookup"><span data-stu-id="1f42b-104">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f42b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f42b-105">Permissions</span></span>
<span data-ttu-id="1f42b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f42b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f42b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f42b-108">Permission type</span></span>      | <span data-ttu-id="1f42b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f42b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f42b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f42b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f42b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f42b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f42b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f42b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f42b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f42b-113">Not supported.</span></span>    |
|<span data-ttu-id="1f42b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f42b-114">Application</span></span> | <span data-ttu-id="1f42b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f42b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f42b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f42b-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f42b-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f42b-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/totalRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/totalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="1f42b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f42b-118">Request headers</span></span>
| <span data-ttu-id="1f42b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1f42b-119">Name</span></span>       | <span data-ttu-id="1f42b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1f42b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1f42b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f42b-121">Authorization</span></span>  | <span data-ttu-id="1f42b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f42b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f42b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1f42b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f42b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1f42b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f42b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f42b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1f42b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f42b-128">Response</span></span>

<span data-ttu-id="1f42b-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f42b-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f42b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1f42b-130">Example</span></span>
<span data-ttu-id="1f42b-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1f42b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1f42b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f42b-132">Request</span></span>
<span data-ttu-id="1f42b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f42b-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_totalrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/totalRowRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f42b-134">C#</span><span class="sxs-lookup"><span data-stu-id="1f42b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-totalrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f42b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1f42b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-totalrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f42b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1f42b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-totalrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1f42b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f42b-137">Response</span></span>
<span data-ttu-id="1f42b-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f42b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
