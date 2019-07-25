---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6703fdb4b5ec10f4d60b370075626a524124a1ec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866152"
---
# <a name="create-table"></a><span data-ttu-id="2c890-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="2c890-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c890-104">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="2c890-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c890-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c890-105">Permissions</span></span>
<span data-ttu-id="2c890-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c890-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c890-108">Permission type</span></span>      | <span data-ttu-id="2c890-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c890-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c890-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c890-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c890-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c890-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c890-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c890-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c890-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c890-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c890-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c890-114">Application</span></span> | <span data-ttu-id="2c890-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c890-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c890-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c890-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="2c890-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c890-117">Request headers</span></span>
| <span data-ttu-id="2c890-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2c890-118">Name</span></span>       | <span data-ttu-id="2c890-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2c890-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2c890-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c890-120">Authorization</span></span>  | <span data-ttu-id="2c890-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c890-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c890-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2c890-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2c890-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2c890-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c890-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c890-126">Request body</span></span>
<span data-ttu-id="2c890-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2c890-127">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="2c890-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="2c890-128">Parameter</span></span>       | <span data-ttu-id="2c890-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2c890-129">Type</span></span>|<span data-ttu-id="2c890-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2c890-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="2c890-131">Адрес</span><span class="sxs-lookup"><span data-stu-id="2c890-131">Address</span></span>  | <span data-ttu-id="2c890-132">string</span><span class="sxs-lookup"><span data-stu-id="2c890-132">string</span></span>| <span data-ttu-id="2c890-133">Адрес диапазона.</span><span class="sxs-lookup"><span data-stu-id="2c890-133">Range address.</span></span> <span data-ttu-id="2c890-134">Если вы вызываете этот API из `worksheets/{id|name}/tables/add` пути, нет необходимости поддерживать префикс имени листа в адресе.</span><span class="sxs-lookup"><span data-stu-id="2c890-134">If you are calling this API off of `worksheets/{id|name}/tables/add` path, there is no need to support the sheet name prefix in the address.</span></span> <span data-ttu-id="2c890-135">Тем не менее, если вы звоните по `workbook/tables/add` адресу, укажите имя листа, на котором необходимо создать таблицу (например: `sheet1!A1:D4`).</span><span class="sxs-lookup"><span data-stu-id="2c890-135">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="2c890-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="2c890-136">hasHeaders</span></span>  | <span data-ttu-id="2c890-137">boolean</span><span class="sxs-lookup"><span data-stu-id="2c890-137">boolean</span></span>|<span data-ttu-id="2c890-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="2c890-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="2c890-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c890-141">Response</span></span>

<span data-ttu-id="2c890-142">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктабле](../resources/workbooktable.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c890-142">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c890-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2c890-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c890-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c890-144">Request</span></span>
<span data-ttu-id="2c890-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c890-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2c890-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c890-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "",
  "hasHeaders": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c890-147">C#</span><span class="sxs-lookup"><span data-stu-id="2c890-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c890-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c890-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c890-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2c890-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2c890-150">Java</span><span class="sxs-lookup"><span data-stu-id="2c890-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2c890-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c890-151">Response</span></span>
<span data-ttu-id="2c890-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c890-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
