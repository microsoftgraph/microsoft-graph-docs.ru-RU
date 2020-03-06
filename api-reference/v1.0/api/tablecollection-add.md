---
title: 'TableCollection: add'
description: Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 909750ea3655c9af630b8e9bd6f7e170c0861e8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509614"
---
# <a name="tablecollection-add"></a><span data-ttu-id="5e45f-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="5e45f-105">TableCollection: add</span></span>

<span data-ttu-id="5e45f-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e45f-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e45f-p102">Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5e45f-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="5e45f-110">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="5e45f-110">Error Handling</span></span>

<span data-ttu-id="5e45f-111">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="5e45f-111">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="5e45f-112">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="5e45f-112">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e45f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e45f-113">Permissions</span></span>
<span data-ttu-id="5e45f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e45f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e45f-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e45f-116">Permission type</span></span>      | <span data-ttu-id="5e45f-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e45f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e45f-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e45f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5e45f-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e45f-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e45f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e45f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e45f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e45f-121">Not supported.</span></span>    |
|<span data-ttu-id="5e45f-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e45f-122">Application</span></span> | <span data-ttu-id="5e45f-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e45f-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e45f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e45f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="5e45f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e45f-125">Request headers</span></span>
| <span data-ttu-id="5e45f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="5e45f-126">Name</span></span>       | <span data-ttu-id="5e45f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5e45f-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5e45f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e45f-128">Authorization</span></span>  | <span data-ttu-id="5e45f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e45f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e45f-131">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5e45f-131">Workbook-Session-Id</span></span>  | <span data-ttu-id="5e45f-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5e45f-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e45f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e45f-134">Request body</span></span>
<span data-ttu-id="5e45f-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5e45f-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e45f-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="5e45f-136">Parameter</span></span>    | <span data-ttu-id="5e45f-137">Тип</span><span class="sxs-lookup"><span data-stu-id="5e45f-137">Type</span></span>   |<span data-ttu-id="5e45f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="5e45f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e45f-139">address</span><span class="sxs-lookup"><span data-stu-id="5e45f-139">address</span></span>|<span data-ttu-id="5e45f-140">string</span><span class="sxs-lookup"><span data-stu-id="5e45f-140">string</span></span>|<span data-ttu-id="5e45f-p107">Адрес или имя объекта range, представляющего источник данных. Если адрес не содержит имя листа, используется текущий активный лист.</span><span class="sxs-lookup"><span data-stu-id="5e45f-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="5e45f-143">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="5e45f-143">hasHeaders</span></span>|<span data-ttu-id="5e45f-144">boolean</span><span class="sxs-lookup"><span data-stu-id="5e45f-144">boolean</span></span>|<span data-ttu-id="5e45f-p108">Логическое значение, указывающее, имеют ли импортируемые данные метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="5e45f-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="5e45f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e45f-148">Response</span></span>

<span data-ttu-id="5e45f-149">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбуктабле](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e45f-149">If successful, this method returns `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e45f-150">Пример</span><span class="sxs-lookup"><span data-stu-id="5e45f-150">Example</span></span>
<span data-ttu-id="5e45f-151">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5e45f-151">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5e45f-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e45f-152">Request</span></span>
<span data-ttu-id="5e45f-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e45f-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e45f-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e45f-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5e45f-155">C#</span><span class="sxs-lookup"><span data-stu-id="5e45f-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e45f-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e45f-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e45f-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e45f-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e45f-158">Java</span><span class="sxs-lookup"><span data-stu-id="5e45f-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5e45f-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e45f-159">Response</span></span>
<span data-ttu-id="5e45f-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e45f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
