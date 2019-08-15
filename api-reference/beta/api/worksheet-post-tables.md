---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 93f8951df02bf8fd52673af717c2a250703d1f9e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420975"
---
# <a name="create-table"></a><span data-ttu-id="d416e-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="d416e-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d416e-104">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="d416e-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="d416e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d416e-105">Permissions</span></span>
<span data-ttu-id="d416e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d416e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d416e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d416e-108">Permission type</span></span>      | <span data-ttu-id="d416e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d416e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d416e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d416e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d416e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d416e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d416e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d416e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d416e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d416e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d416e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d416e-114">Application</span></span> | <span data-ttu-id="d416e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d416e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d416e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d416e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="d416e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d416e-117">Request headers</span></span>
| <span data-ttu-id="d416e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d416e-118">Name</span></span>       | <span data-ttu-id="d416e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d416e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d416e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d416e-120">Authorization</span></span>  | <span data-ttu-id="d416e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d416e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d416e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d416e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d416e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d416e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d416e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d416e-126">Request body</span></span>
<span data-ttu-id="d416e-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d416e-127">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="d416e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="d416e-128">Parameter</span></span>       | <span data-ttu-id="d416e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d416e-129">Type</span></span>|<span data-ttu-id="d416e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d416e-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="d416e-131">Адрес</span><span class="sxs-lookup"><span data-stu-id="d416e-131">Address</span></span>  | <span data-ttu-id="d416e-132">string</span><span class="sxs-lookup"><span data-stu-id="d416e-132">string</span></span>| <span data-ttu-id="d416e-133">Адрес диапазона.</span><span class="sxs-lookup"><span data-stu-id="d416e-133">Range address.</span></span> <span data-ttu-id="d416e-134">Если вы вызываете этот API из `worksheets/{id|name}/tables/add` пути, нет необходимости поддерживать префикс имени листа в адресе.</span><span class="sxs-lookup"><span data-stu-id="d416e-134">If you are calling this API off of `worksheets/{id|name}/tables/add` path, there is no need to support the sheet name prefix in the address.</span></span> <span data-ttu-id="d416e-135">Тем не менее, если вы звоните по `workbook/tables/add` адресу, укажите имя листа, на котором необходимо создать таблицу (например: `sheet1!A1:D4`).</span><span class="sxs-lookup"><span data-stu-id="d416e-135">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="d416e-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="d416e-136">hasHeaders</span></span>  | <span data-ttu-id="d416e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d416e-137">boolean</span></span>|<span data-ttu-id="d416e-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="d416e-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="d416e-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="d416e-141">Response</span></span>

<span data-ttu-id="d416e-142">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктабле](../resources/workbooktable.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d416e-142">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d416e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d416e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d416e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d416e-144">Request</span></span>
<span data-ttu-id="d416e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d416e-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d416e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d416e-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d416e-147">C#</span><span class="sxs-lookup"><span data-stu-id="d416e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d416e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d416e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d416e-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d416e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d416e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d416e-150">Response</span></span>
<span data-ttu-id="d416e-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d416e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
