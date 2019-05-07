---
title: Обновление таблицы
description: Обновление свойств объекта таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3bdb9de76a51f89552e388addbe352fa4b5c49c8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602814"
---
# <a name="update-table"></a><span data-ttu-id="b4a56-103">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="b4a56-103">Update table</span></span>

<span data-ttu-id="b4a56-104">Обновление свойств объекта таблицы.</span><span class="sxs-lookup"><span data-stu-id="b4a56-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b4a56-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a56-105">Permissions</span></span>
<span data-ttu-id="b4a56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4a56-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a56-108">Permission type</span></span>      | <span data-ttu-id="b4a56-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4a56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4a56-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4a56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4a56-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4a56-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b4a56-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4a56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4a56-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a56-113">Not supported.</span></span>    |
|<span data-ttu-id="b4a56-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4a56-114">Application</span></span> | <span data-ttu-id="b4a56-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a56-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4a56-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4a56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b4a56-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4a56-117">Optional request headers</span></span>
| <span data-ttu-id="b4a56-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b4a56-118">Name</span></span>       | <span data-ttu-id="b4a56-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b4a56-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b4a56-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4a56-120">Authorization</span></span>  | <span data-ttu-id="b4a56-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4a56-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4a56-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b4a56-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b4a56-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b4a56-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4a56-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4a56-126">Request body</span></span>
<span data-ttu-id="b4a56-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b4a56-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4a56-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4a56-130">Property</span></span>     | <span data-ttu-id="b4a56-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4a56-131">Type</span></span>   |<span data-ttu-id="b4a56-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4a56-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4a56-133">name</span><span class="sxs-lookup"><span data-stu-id="b4a56-133">name</span></span>|<span data-ttu-id="b4a56-134">string</span><span class="sxs-lookup"><span data-stu-id="b4a56-134">string</span></span>|<span data-ttu-id="b4a56-135">Имя таблицы.</span><span class="sxs-lookup"><span data-stu-id="b4a56-135">Name of the table.</span></span>|
|<span data-ttu-id="b4a56-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="b4a56-136">showHeaders</span></span>|<span data-ttu-id="b4a56-137">boolean</span><span class="sxs-lookup"><span data-stu-id="b4a56-137">boolean</span></span>|<span data-ttu-id="b4a56-p105">Указывает, отображается ли строка заголовков. Можно задать это значение, чтобы отобразить или скрыть строку заголовков.</span><span class="sxs-lookup"><span data-stu-id="b4a56-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="b4a56-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="b4a56-140">showTotals</span></span>|<span data-ttu-id="b4a56-141">boolean</span><span class="sxs-lookup"><span data-stu-id="b4a56-141">boolean</span></span>|<span data-ttu-id="b4a56-p106">Указывает, отображается ли строка итогов. Можно задать это значение, чтобы отобразить или скрыть строку итогов.</span><span class="sxs-lookup"><span data-stu-id="b4a56-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="b4a56-144">style</span><span class="sxs-lookup"><span data-stu-id="b4a56-144">style</span></span>|<span data-ttu-id="b4a56-145">string</span><span class="sxs-lookup"><span data-stu-id="b4a56-145">string</span></span>|<span data-ttu-id="b4a56-146">Постоянное значение, представляющее стиль таблицы.</span><span class="sxs-lookup"><span data-stu-id="b4a56-146">Constant value that represents the Table style.</span></span> <span data-ttu-id="b4a56-147">Допустимые значения: от TableStyleLight1 до TableStyleLight21, TableStyleMedium1 до TableStyleMedium28, TableStyleStyleDark1 до TableStyleStyleDark11.</span><span class="sxs-lookup"><span data-stu-id="b4a56-147">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="b4a56-148">Также можно указать настраиваемый пользовательский стиль, имеющийся в книге.</span><span class="sxs-lookup"><span data-stu-id="b4a56-148">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="b4a56-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a56-149">Response</span></span>

<span data-ttu-id="b4a56-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбуктабле](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4a56-150">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4a56-151">Пример</span><span class="sxs-lookup"><span data-stu-id="b4a56-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4a56-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4a56-152">Request</span></span>
<span data-ttu-id="b4a56-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4a56-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="b4a56-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a56-154">Response</span></span>
<span data-ttu-id="b4a56-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4a56-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b4a56-158">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b4a56-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b4a56-159">Языках</span><span class="sxs-lookup"><span data-stu-id="b4a56-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_table-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4a56-160">Язык</span><span class="sxs-lookup"><span data-stu-id="b4a56-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_table-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
