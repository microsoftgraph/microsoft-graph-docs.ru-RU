---
title: 'TableCollection: add'
description: Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f5c078c90133490e216756b23643751b65cac934
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278887"
---
# <a name="tablecollection-add"></a><span data-ttu-id="bcc2d-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="bcc2d-105">TableCollection: add</span></span>

<span data-ttu-id="bcc2d-p102">Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="bcc2d-109">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="bcc2d-109">Error Handling</span></span>

<span data-ttu-id="bcc2d-110">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-110">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="bcc2d-111">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-111">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcc2d-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc2d-112">Permissions</span></span>
<span data-ttu-id="bcc2d-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc2d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc2d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc2d-115">Permission type</span></span>      | <span data-ttu-id="bcc2d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcc2d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcc2d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcc2d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="bcc2d-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcc2d-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bcc2d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcc2d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcc2d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-120">Not supported.</span></span>    |
|<span data-ttu-id="bcc2d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcc2d-121">Application</span></span> | <span data-ttu-id="bcc2d-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcc2d-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcc2d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="bcc2d-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcc2d-124">Request headers</span></span>
| <span data-ttu-id="bcc2d-125">Имя</span><span class="sxs-lookup"><span data-stu-id="bcc2d-125">Name</span></span>       | <span data-ttu-id="bcc2d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc2d-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bcc2d-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcc2d-127">Authorization</span></span>  | <span data-ttu-id="bcc2d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bcc2d-130">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bcc2d-130">Workbook-Session-Id</span></span>  | <span data-ttu-id="bcc2d-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcc2d-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcc2d-133">Request body</span></span>
<span data-ttu-id="bcc2d-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bcc2d-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="bcc2d-135">Parameter</span></span>    | <span data-ttu-id="bcc2d-136">Тип</span><span class="sxs-lookup"><span data-stu-id="bcc2d-136">Type</span></span>   |<span data-ttu-id="bcc2d-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc2d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcc2d-138">address</span><span class="sxs-lookup"><span data-stu-id="bcc2d-138">address</span></span>|<span data-ttu-id="bcc2d-139">string</span><span class="sxs-lookup"><span data-stu-id="bcc2d-139">string</span></span>|<span data-ttu-id="bcc2d-p107">Адрес или имя объекта range, представляющего источник данных. Если адрес не содержит имя листа, используется текущий активный лист.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="bcc2d-142">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="bcc2d-142">hasHeaders</span></span>|<span data-ttu-id="bcc2d-143">boolean</span><span class="sxs-lookup"><span data-stu-id="bcc2d-143">boolean</span></span>|<span data-ttu-id="bcc2d-p108">Логическое значение, указывающее, имеют ли импортируемые данные метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="bcc2d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc2d-147">Response</span></span>

<span data-ttu-id="bcc2d-148">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктабле](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-148">If successful, this method returns `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcc2d-149">Пример</span><span class="sxs-lookup"><span data-stu-id="bcc2d-149">Example</span></span>
<span data-ttu-id="bcc2d-150">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bcc2d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc2d-151">Request</span></span>
<span data-ttu-id="bcc2d-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="bcc2d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc2d-153">Response</span></span>
<span data-ttu-id="bcc2d-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcc2d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bcc2d-157">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="bcc2d-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bcc2d-158">C#</span><span class="sxs-lookup"><span data-stu-id="bcc2d-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcc2d-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="bcc2d-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecollection_add-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bcc2d-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bcc2d-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecollection_add-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablecollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
