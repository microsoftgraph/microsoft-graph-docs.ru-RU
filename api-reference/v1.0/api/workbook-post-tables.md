---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e71cdfbadce6e8a35d698dd0012a8d937ceeef70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026462"
---
# <a name="create-table"></a><span data-ttu-id="948aa-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="948aa-103">Create table</span></span>

<span data-ttu-id="948aa-104">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="948aa-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="948aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="948aa-105">Permissions</span></span>
<span data-ttu-id="948aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="948aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="948aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="948aa-108">Permission type</span></span>      | <span data-ttu-id="948aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="948aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="948aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="948aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="948aa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948aa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="948aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="948aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="948aa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="948aa-113">Not supported.</span></span>    |
|<span data-ttu-id="948aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="948aa-114">Application</span></span> | <span data-ttu-id="948aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="948aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="948aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="948aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{table-id}/add

```
## <a name="request-headers"></a><span data-ttu-id="948aa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="948aa-117">Request headers</span></span>
| <span data-ttu-id="948aa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="948aa-118">Name</span></span>       | <span data-ttu-id="948aa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="948aa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="948aa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="948aa-120">Authorization</span></span>  | <span data-ttu-id="948aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="948aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="948aa-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="948aa-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="948aa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="948aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="948aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="948aa-126">Request body</span></span>
<span data-ttu-id="948aa-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="948aa-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="948aa-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="948aa-128">Parameter</span></span>           | <span data-ttu-id="948aa-129">Тип</span><span class="sxs-lookup"><span data-stu-id="948aa-129">Type</span></span>      |<span data-ttu-id="948aa-130">Описание</span><span class="sxs-lookup"><span data-stu-id="948aa-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="948aa-131">Адрес</span><span class="sxs-lookup"><span data-stu-id="948aa-131">Address</span></span>  | <span data-ttu-id="948aa-132">string</span><span class="sxs-lookup"><span data-stu-id="948aa-132">string</span></span>| <span data-ttu-id="948aa-p104">Адрес диапазона. При вызове этого API из пути `worksheets/{id or name}/tables/add` не нужно указывать префикс имя листа в адресе. Однако при вызове этого API из пути `workbook/tables/add` нужно указать имя листа, на котором требуется создать таблицу (например: `sheet1!A1:D4`)</span><span class="sxs-lookup"><span data-stu-id="948aa-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="948aa-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="948aa-136">hasHeaders</span></span>  | <span data-ttu-id="948aa-137">boolean</span><span class="sxs-lookup"><span data-stu-id="948aa-137">boolean</span></span>|<span data-ttu-id="948aa-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="948aa-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="948aa-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="948aa-141">Response</span></span>

<span data-ttu-id="948aa-142">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктабле](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="948aa-142">If successful, this method returns `201 Created` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="948aa-143">Пример</span><span class="sxs-lookup"><span data-stu-id="948aa-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="948aa-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="948aa-144">Request</span></span>
<span data-ttu-id="948aa-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="948aa-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{table-id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="948aa-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="948aa-146">Response</span></span>
<span data-ttu-id="948aa-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="948aa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
