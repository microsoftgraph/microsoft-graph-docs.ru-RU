---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 29666544e46e9879313fa0593b15ef83f1fb7f25
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024582"
---
# <a name="table-converttorange"></a><span data-ttu-id="c1c07-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="c1c07-104">Table: convertToRange</span></span>

<span data-ttu-id="c1c07-p102">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="c1c07-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1c07-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1c07-107">Permissions</span></span>
<span data-ttu-id="c1c07-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1c07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1c07-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1c07-110">Permission type</span></span>      | <span data-ttu-id="c1c07-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1c07-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1c07-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1c07-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1c07-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1c07-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1c07-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1c07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1c07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c07-115">Not supported.</span></span>    |
|<span data-ttu-id="c1c07-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1c07-116">Application</span></span> | <span data-ttu-id="c1c07-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c07-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1c07-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1c07-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="c1c07-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1c07-119">Request headers</span></span>
| <span data-ttu-id="c1c07-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c1c07-120">Name</span></span>       | <span data-ttu-id="c1c07-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c07-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1c07-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1c07-122">Authorization</span></span>  | <span data-ttu-id="c1c07-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1c07-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1c07-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c1c07-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c1c07-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c1c07-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1c07-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1c07-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c1c07-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1c07-129">Response</span></span>

<span data-ttu-id="c1c07-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1c07-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1c07-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c1c07-131">Example</span></span>
<span data-ttu-id="c1c07-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c1c07-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1c07-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1c07-133">Request</span></span>
<span data-ttu-id="c1c07-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1c07-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1c07-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1c07-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1c07-136">C#</span><span class="sxs-lookup"><span data-stu-id="c1c07-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-converttorange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1c07-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1c07-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-converttorange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1c07-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1c07-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-converttorange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c1c07-139">Java</span><span class="sxs-lookup"><span data-stu-id="c1c07-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-converttorange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c1c07-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1c07-140">Response</span></span>
<span data-ttu-id="c1c07-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1c07-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
