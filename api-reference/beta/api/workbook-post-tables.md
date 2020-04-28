---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 122e7b0af66962eee04d549142291ae53d31ecc0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451471"
---
# <a name="create-table"></a><span data-ttu-id="59c03-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="59c03-103">Create table</span></span>

<span data-ttu-id="59c03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59c03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59c03-105">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="59c03-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="59c03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59c03-106">Permissions</span></span>
<span data-ttu-id="59c03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59c03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59c03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59c03-109">Permission type</span></span>      | <span data-ttu-id="59c03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59c03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59c03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59c03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59c03-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59c03-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59c03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59c03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59c03-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59c03-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59c03-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59c03-115">Application</span></span> | <span data-ttu-id="59c03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59c03-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59c03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59c03-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="59c03-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59c03-118">Request headers</span></span>
| <span data-ttu-id="59c03-119">Имя</span><span class="sxs-lookup"><span data-stu-id="59c03-119">Name</span></span>       | <span data-ttu-id="59c03-120">Описание</span><span class="sxs-lookup"><span data-stu-id="59c03-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59c03-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59c03-121">Authorization</span></span>  | <span data-ttu-id="59c03-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59c03-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59c03-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59c03-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="59c03-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="59c03-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59c03-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59c03-127">Request body</span></span>
<span data-ttu-id="59c03-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="59c03-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59c03-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="59c03-129">Parameter</span></span>           | <span data-ttu-id="59c03-130">Тип</span><span class="sxs-lookup"><span data-stu-id="59c03-130">Type</span></span>      |<span data-ttu-id="59c03-131">Описание</span><span class="sxs-lookup"><span data-stu-id="59c03-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="59c03-132">Адрес</span><span class="sxs-lookup"><span data-stu-id="59c03-132">Address</span></span>  | <span data-ttu-id="59c03-133">string</span><span class="sxs-lookup"><span data-stu-id="59c03-133">string</span></span>| <span data-ttu-id="59c03-p104">Адрес диапазона. При вызове этого API из пути `worksheets/{id or name}/tables/add` не нужно указывать префикс имя листа в адресе. Однако при вызове этого API из пути `workbook/tables/add` нужно указать имя листа, на котором требуется создать таблицу (например: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="59c03-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="59c03-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="59c03-137">hasHeaders</span></span>  | <span data-ttu-id="59c03-138">boolean</span><span class="sxs-lookup"><span data-stu-id="59c03-138">boolean</span></span>|<span data-ttu-id="59c03-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="59c03-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="59c03-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="59c03-142">Response</span></span>

<span data-ttu-id="59c03-143">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктабле](../resources/workbooktable.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59c03-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59c03-144">Пример</span><span class="sxs-lookup"><span data-stu-id="59c03-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59c03-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="59c03-145">Request</span></span>
<span data-ttu-id="59c03-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59c03-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59c03-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="59c03-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
# <a name="c"></a>[<span data-ttu-id="59c03-148">C#</span><span class="sxs-lookup"><span data-stu-id="59c03-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-workbook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59c03-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59c03-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-workbook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59c03-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59c03-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-workbook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59c03-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="59c03-151">Response</span></span>
<span data-ttu-id="59c03-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59c03-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
