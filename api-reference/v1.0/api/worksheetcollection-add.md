---
title: 'WorksheetCollection: add'
description: . Активируйте ().
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 49ba6dbe849cf027e123f5540a72b7b1da11f7f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508613"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="70a41-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="70a41-103">WorksheetCollection: add</span></span>

<span data-ttu-id="70a41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70a41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70a41-105">Добавляет новый лист в книгу.</span><span class="sxs-lookup"><span data-stu-id="70a41-105">Adds a new worksheet to the workbook.</span></span> <span data-ttu-id="70a41-106">Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="70a41-106">The worksheet will be added at the end of existing worksheets.</span></span> <span data-ttu-id="70a41-107">Если вы хотите активировать недавно добавленный лист, вызовите. Activate ().</span><span class="sxs-lookup"><span data-stu-id="70a41-107">If you wish to activate the newly added worksheet, call .activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="70a41-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70a41-108">Permissions</span></span>
<span data-ttu-id="70a41-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70a41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70a41-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70a41-111">Permission type</span></span>      | <span data-ttu-id="70a41-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70a41-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70a41-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70a41-113">Delegated (work or school account)</span></span> | <span data-ttu-id="70a41-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70a41-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70a41-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70a41-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70a41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70a41-116">Not supported.</span></span>    |
|<span data-ttu-id="70a41-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70a41-117">Application</span></span> | <span data-ttu-id="70a41-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70a41-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70a41-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70a41-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="70a41-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70a41-120">Request headers</span></span>
| <span data-ttu-id="70a41-121">Имя</span><span class="sxs-lookup"><span data-stu-id="70a41-121">Name</span></span>       | <span data-ttu-id="70a41-122">Описание</span><span class="sxs-lookup"><span data-stu-id="70a41-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="70a41-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70a41-123">Authorization</span></span>  | <span data-ttu-id="70a41-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70a41-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70a41-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="70a41-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="70a41-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="70a41-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70a41-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70a41-129">Request body</span></span>
<span data-ttu-id="70a41-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="70a41-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="70a41-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="70a41-131">Parameter</span></span>    | <span data-ttu-id="70a41-132">Тип</span><span class="sxs-lookup"><span data-stu-id="70a41-132">Type</span></span>   |<span data-ttu-id="70a41-133">Описание</span><span class="sxs-lookup"><span data-stu-id="70a41-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70a41-134">name</span><span class="sxs-lookup"><span data-stu-id="70a41-134">name</span></span>|<span data-ttu-id="70a41-135">string</span><span class="sxs-lookup"><span data-stu-id="70a41-135">string</span></span>|<span data-ttu-id="70a41-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="70a41-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="70a41-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a41-140">Response</span></span>

<span data-ttu-id="70a41-141">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукворкшит](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70a41-141">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70a41-142">Пример</span><span class="sxs-lookup"><span data-stu-id="70a41-142">Example</span></span>
<span data-ttu-id="70a41-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="70a41-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="70a41-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="70a41-144">Request</span></span>
<span data-ttu-id="70a41-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70a41-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70a41-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="70a41-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="70a41-147">C#</span><span class="sxs-lookup"><span data-stu-id="70a41-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70a41-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70a41-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70a41-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70a41-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70a41-150">Java</span><span class="sxs-lookup"><span data-stu-id="70a41-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="70a41-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a41-151">Response</span></span>
<span data-ttu-id="70a41-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70a41-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
