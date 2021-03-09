---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6a772cf10c0442ee53e3843d9d49e98cfeb565e1
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575296"
---
# <a name="create-table"></a><span data-ttu-id="61d1f-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="61d1f-103">Create table</span></span>

<span data-ttu-id="61d1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61d1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61d1f-105">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="61d1f-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="61d1f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61d1f-106">Permissions</span></span>
<span data-ttu-id="61d1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61d1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61d1f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61d1f-109">Permission type</span></span>      | <span data-ttu-id="61d1f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61d1f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61d1f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61d1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="61d1f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61d1f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="61d1f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61d1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61d1f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61d1f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="61d1f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61d1f-115">Application</span></span> | <span data-ttu-id="61d1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61d1f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61d1f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61d1f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/$/add
POST /me/drive/root:/{item-path}:/workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="61d1f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61d1f-118">Request headers</span></span>
| <span data-ttu-id="61d1f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="61d1f-119">Name</span></span>       | <span data-ttu-id="61d1f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="61d1f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="61d1f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61d1f-121">Authorization</span></span>  | <span data-ttu-id="61d1f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61d1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="61d1f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="61d1f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="61d1f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="61d1f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61d1f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61d1f-127">Request body</span></span>
<span data-ttu-id="61d1f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="61d1f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="61d1f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="61d1f-129">Parameter</span></span>           | <span data-ttu-id="61d1f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="61d1f-130">Type</span></span>      |<span data-ttu-id="61d1f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="61d1f-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="61d1f-132">Адрес</span><span class="sxs-lookup"><span data-stu-id="61d1f-132">Address</span></span>  | <span data-ttu-id="61d1f-133">string</span><span class="sxs-lookup"><span data-stu-id="61d1f-133">string</span></span>| <span data-ttu-id="61d1f-p104">Адрес диапазона. При вызове этого API из пути `worksheets/{id or name}/tables/add` не нужно указывать префикс имя листа в адресе. Однако при вызове этого API из пути `workbook/tables/add` нужно указать имя листа, на котором требуется создать таблицу (например: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="61d1f-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="61d1f-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="61d1f-137">hasHeaders</span></span>  | <span data-ttu-id="61d1f-138">boolean</span><span class="sxs-lookup"><span data-stu-id="61d1f-138">boolean</span></span>|<span data-ttu-id="61d1f-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="61d1f-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="61d1f-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="61d1f-142">Response</span></span>

<span data-ttu-id="61d1f-143">В случае успеха этот метод возвращает код отклика и `201 Created` [объект workbookTable](../resources/workbooktable.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="61d1f-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61d1f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="61d1f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61d1f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="61d1f-145">Request</span></span>
<span data-ttu-id="61d1f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61d1f-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61d1f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="61d1f-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="61d1f-148">C#</span><span class="sxs-lookup"><span data-stu-id="61d1f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-workbook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61d1f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61d1f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-workbook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61d1f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61d1f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-workbook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61d1f-151">Java</span><span class="sxs-lookup"><span data-stu-id="61d1f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-workbook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="61d1f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="61d1f-152">Response</span></span>
<span data-ttu-id="61d1f-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61d1f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


