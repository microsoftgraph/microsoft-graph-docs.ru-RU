---
title: Обновление таблицы
description: Обновление свойств объекта таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a3e544e06519dfd014eb70eec5eb0cf4d84d4996
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509621"
---
# <a name="update-table"></a><span data-ttu-id="e82ee-103">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="e82ee-103">Update table</span></span>

<span data-ttu-id="e82ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e82ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e82ee-105">Обновление свойств объекта таблицы.</span><span class="sxs-lookup"><span data-stu-id="e82ee-105">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e82ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e82ee-106">Permissions</span></span>
<span data-ttu-id="e82ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e82ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e82ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e82ee-109">Permission type</span></span>      | <span data-ttu-id="e82ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e82ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e82ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e82ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e82ee-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e82ee-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e82ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e82ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e82ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e82ee-114">Not supported.</span></span>    |
|<span data-ttu-id="e82ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e82ee-115">Application</span></span> | <span data-ttu-id="e82ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e82ee-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e82ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e82ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e82ee-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e82ee-118">Optional request headers</span></span>
| <span data-ttu-id="e82ee-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e82ee-119">Name</span></span>       | <span data-ttu-id="e82ee-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e82ee-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e82ee-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e82ee-121">Authorization</span></span>  | <span data-ttu-id="e82ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e82ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e82ee-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e82ee-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e82ee-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e82ee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e82ee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e82ee-127">Request body</span></span>
<span data-ttu-id="e82ee-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e82ee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e82ee-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e82ee-131">Property</span></span>     | <span data-ttu-id="e82ee-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e82ee-132">Type</span></span>   |<span data-ttu-id="e82ee-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e82ee-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e82ee-134">name</span><span class="sxs-lookup"><span data-stu-id="e82ee-134">name</span></span>|<span data-ttu-id="e82ee-135">string</span><span class="sxs-lookup"><span data-stu-id="e82ee-135">string</span></span>|<span data-ttu-id="e82ee-136">Имя таблицы.</span><span class="sxs-lookup"><span data-stu-id="e82ee-136">Name of the table.</span></span>|
|<span data-ttu-id="e82ee-137">showHeaders</span><span class="sxs-lookup"><span data-stu-id="e82ee-137">showHeaders</span></span>|<span data-ttu-id="e82ee-138">boolean</span><span class="sxs-lookup"><span data-stu-id="e82ee-138">boolean</span></span>|<span data-ttu-id="e82ee-p105">Указывает, отображается ли строка заголовков. Можно задать это значение, чтобы отобразить или скрыть строку заголовков.</span><span class="sxs-lookup"><span data-stu-id="e82ee-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="e82ee-141">showTotals</span><span class="sxs-lookup"><span data-stu-id="e82ee-141">showTotals</span></span>|<span data-ttu-id="e82ee-142">boolean</span><span class="sxs-lookup"><span data-stu-id="e82ee-142">boolean</span></span>|<span data-ttu-id="e82ee-p106">Указывает, отображается ли строка итогов. Можно задать это значение, чтобы отобразить или скрыть строку итогов.</span><span class="sxs-lookup"><span data-stu-id="e82ee-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="e82ee-145">style</span><span class="sxs-lookup"><span data-stu-id="e82ee-145">style</span></span>|<span data-ttu-id="e82ee-146">string</span><span class="sxs-lookup"><span data-stu-id="e82ee-146">string</span></span>|<span data-ttu-id="e82ee-147">Постоянное значение, представляющее стиль таблицы.</span><span class="sxs-lookup"><span data-stu-id="e82ee-147">Constant value that represents the Table style.</span></span> <span data-ttu-id="e82ee-148">Допустимые значения: от TableStyleLight1 до TableStyleLight21, TableStyleMedium1 до TableStyleMedium28, TableStyleStyleDark1 до TableStyleStyleDark11.</span><span class="sxs-lookup"><span data-stu-id="e82ee-148">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="e82ee-149">Также можно указать настраиваемый пользовательский стиль, имеющийся в книге.</span><span class="sxs-lookup"><span data-stu-id="e82ee-149">A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="e82ee-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e82ee-150">Response</span></span>

<span data-ttu-id="e82ee-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбуктабле](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e82ee-151">If successful, this method returns a `200 OK` response code and updated [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e82ee-152">Пример</span><span class="sxs-lookup"><span data-stu-id="e82ee-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e82ee-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="e82ee-153">Request</span></span>
<span data-ttu-id="e82ee-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e82ee-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e82ee-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="e82ee-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e82ee-156">C#</span><span class="sxs-lookup"><span data-stu-id="e82ee-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e82ee-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e82ee-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e82ee-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e82ee-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e82ee-159">Java</span><span class="sxs-lookup"><span data-stu-id="e82ee-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e82ee-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="e82ee-160">Response</span></span>
<span data-ttu-id="e82ee-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e82ee-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
