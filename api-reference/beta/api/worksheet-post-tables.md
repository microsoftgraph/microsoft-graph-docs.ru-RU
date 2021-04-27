---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 133b57c66cd0333c4dec1cd37895369749889bbb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050705"
---
# <a name="create-table"></a><span data-ttu-id="49f4c-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="49f4c-103">Create table</span></span>

<span data-ttu-id="49f4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49f4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f4c-105">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="49f4c-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="49f4c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49f4c-106">Permissions</span></span>
<span data-ttu-id="49f4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49f4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f4c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49f4c-109">Permission type</span></span>      | <span data-ttu-id="49f4c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49f4c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49f4c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49f4c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49f4c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49f4c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49f4c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49f4c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49f4c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49f4c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49f4c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49f4c-115">Application</span></span> | <span data-ttu-id="49f4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49f4c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49f4c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49f4c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="49f4c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49f4c-118">Request headers</span></span>
| <span data-ttu-id="49f4c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="49f4c-119">Name</span></span>       | <span data-ttu-id="49f4c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="49f4c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49f4c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49f4c-121">Authorization</span></span>  | <span data-ttu-id="49f4c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49f4c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49f4c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49f4c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="49f4c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="49f4c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f4c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49f4c-127">Request body</span></span>
<span data-ttu-id="49f4c-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="49f4c-128">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="49f4c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="49f4c-129">Parameter</span></span>       | <span data-ttu-id="49f4c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="49f4c-130">Type</span></span>|<span data-ttu-id="49f4c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="49f4c-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="49f4c-132">Адрес</span><span class="sxs-lookup"><span data-stu-id="49f4c-132">Address</span></span>  | <span data-ttu-id="49f4c-133">string</span><span class="sxs-lookup"><span data-stu-id="49f4c-133">string</span></span>| <span data-ttu-id="49f4c-134">Адрес диапазона.</span><span class="sxs-lookup"><span data-stu-id="49f4c-134">Range address.</span></span> <span data-ttu-id="49f4c-135">Если этот API отключен от пути, нет необходимости поддерживать префикс имени листа `worksheets/{id|name}/tables/add` в адресе.</span><span class="sxs-lookup"><span data-stu-id="49f4c-135">If you are calling this API off of `worksheets/{id|name}/tables/add` path, there is no need to support the sheet name prefix in the address.</span></span> <span data-ttu-id="49f4c-136">Однако, если вы вызываете это отключение пути, затем поставляют имя листа, на котором должна быть создана таблица `workbook/tables/add` (пример: `sheet1!A1:D4` )</span><span class="sxs-lookup"><span data-stu-id="49f4c-136">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="49f4c-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="49f4c-137">hasHeaders</span></span>  | <span data-ttu-id="49f4c-138">boolean</span><span class="sxs-lookup"><span data-stu-id="49f4c-138">boolean</span></span>|<span data-ttu-id="49f4c-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="49f4c-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="49f4c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="49f4c-142">Response</span></span>

<span data-ttu-id="49f4c-143">В случае успеха этот метод возвращает код отклика и `201 Created` [объект workbookTable](../resources/workbooktable.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49f4c-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f4c-144">Пример</span><span class="sxs-lookup"><span data-stu-id="49f4c-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49f4c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="49f4c-145">Request</span></span>
<span data-ttu-id="49f4c-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49f4c-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49f4c-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="49f4c-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="49f4c-148">C#</span><span class="sxs-lookup"><span data-stu-id="49f4c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49f4c-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49f4c-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49f4c-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49f4c-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49f4c-151">Java</span><span class="sxs-lookup"><span data-stu-id="49f4c-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49f4c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="49f4c-152">Response</span></span>
<span data-ttu-id="49f4c-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49f4c-153">Here is an example of the response.</span></span> <span data-ttu-id="49f4c-154">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49f4c-154">Note: The response object shown here might be shortened for readability.</span></span>
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


