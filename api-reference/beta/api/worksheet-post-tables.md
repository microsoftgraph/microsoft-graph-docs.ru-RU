---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 649fb5848a7c30908a87d8ea643aefa19ca5623e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516373"
---
# <a name="create-table"></a><span data-ttu-id="8794e-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="8794e-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8794e-104">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="8794e-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="8794e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8794e-105">Permissions</span></span>
<span data-ttu-id="8794e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8794e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8794e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8794e-108">Permission type</span></span>      | <span data-ttu-id="8794e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8794e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8794e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8794e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8794e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8794e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8794e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8794e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8794e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8794e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8794e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8794e-114">Application</span></span> | <span data-ttu-id="8794e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8794e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8794e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8794e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="8794e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8794e-117">Request headers</span></span>
| <span data-ttu-id="8794e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8794e-118">Name</span></span>       | <span data-ttu-id="8794e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8794e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8794e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8794e-120">Authorization</span></span>  | <span data-ttu-id="8794e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8794e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8794e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8794e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8794e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8794e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8794e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8794e-126">Request body</span></span>
<span data-ttu-id="8794e-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8794e-127">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="8794e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="8794e-128">Parameter</span></span>       | <span data-ttu-id="8794e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8794e-129">Type</span></span>|<span data-ttu-id="8794e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8794e-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="8794e-131">Адрес</span><span class="sxs-lookup"><span data-stu-id="8794e-131">Address</span></span>  | <span data-ttu-id="8794e-132">string</span><span class="sxs-lookup"><span data-stu-id="8794e-132">string</span></span>| <span data-ttu-id="8794e-p104">Адрес диапазона. Если вы отзываете этот API для пути \`worksheets/{id</span><span class="sxs-lookup"><span data-stu-id="8794e-p104">Range address. If you are calling this API off of \`worksheets/{id</span></span>|<span data-ttu-id="8794e-135">Имя} / таблиц и добавления` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `книг и таблиц/добавления` path, then supply the sheet name on which the table needs to be created (example: `sheet1! A1:D4 ")</span><span class="sxs-lookup"><span data-stu-id="8794e-135">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span></span>|
| <span data-ttu-id="8794e-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="8794e-136">hasHeaders</span></span>  | <span data-ttu-id="8794e-137">boolean</span><span class="sxs-lookup"><span data-stu-id="8794e-137">boolean</span></span>|<span data-ttu-id="8794e-p105">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="8794e-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="8794e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8794e-141">Response</span></span>

<span data-ttu-id="8794e-142">В случае успеха этот метод возвращает код ответа `201 Created` и объект [Table](../resources/table.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8794e-142">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8794e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="8794e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8794e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8794e-144">Request</span></span>
<span data-ttu-id="8794e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8794e-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="8794e-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="8794e-146">Response</span></span>
<span data-ttu-id="8794e-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8794e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
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
    "Error: /api-reference/beta/api/worksheet-post-tables.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
