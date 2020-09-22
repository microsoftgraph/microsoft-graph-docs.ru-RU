---
title: 'WorksheetCollection: add'
description: . Активируйте ().
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4eb8b914d44bf9f92fa3951d4e935ba1afa58ed2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041731"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="e24be-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="e24be-103">WorksheetCollection: add</span></span>

<span data-ttu-id="e24be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e24be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e24be-105">Добавляет новый лист в книгу.</span><span class="sxs-lookup"><span data-stu-id="e24be-105">Adds a new worksheet to the workbook.</span></span> <span data-ttu-id="e24be-106">Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="e24be-106">The worksheet will be added at the end of existing worksheets.</span></span> <span data-ttu-id="e24be-107">Если вы хотите активировать недавно добавленный лист, вызовите. Activate ().</span><span class="sxs-lookup"><span data-stu-id="e24be-107">If you wish to activate the newly added worksheet, call .activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="e24be-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e24be-108">Permissions</span></span>
<span data-ttu-id="e24be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e24be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e24be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e24be-111">Permission type</span></span>      | <span data-ttu-id="e24be-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e24be-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e24be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e24be-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e24be-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e24be-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e24be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e24be-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e24be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e24be-116">Not supported.</span></span>    |
|<span data-ttu-id="e24be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e24be-117">Application</span></span> | <span data-ttu-id="e24be-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e24be-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e24be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e24be-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="e24be-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e24be-120">Request headers</span></span>
| <span data-ttu-id="e24be-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e24be-121">Name</span></span>       | <span data-ttu-id="e24be-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e24be-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e24be-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e24be-123">Authorization</span></span>  | <span data-ttu-id="e24be-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e24be-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e24be-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e24be-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e24be-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e24be-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e24be-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e24be-129">Request body</span></span>
<span data-ttu-id="e24be-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e24be-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e24be-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="e24be-131">Parameter</span></span>    | <span data-ttu-id="e24be-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e24be-132">Type</span></span>   |<span data-ttu-id="e24be-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e24be-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e24be-134">name</span><span class="sxs-lookup"><span data-stu-id="e24be-134">name</span></span>|<span data-ttu-id="e24be-135">string</span><span class="sxs-lookup"><span data-stu-id="e24be-135">string</span></span>|<span data-ttu-id="e24be-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="e24be-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="e24be-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e24be-140">Response</span></span>

<span data-ttu-id="e24be-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукворкшит](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e24be-141">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e24be-142">Пример</span><span class="sxs-lookup"><span data-stu-id="e24be-142">Example</span></span>
<span data-ttu-id="e24be-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e24be-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e24be-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e24be-144">Request</span></span>
<span data-ttu-id="e24be-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e24be-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e24be-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e24be-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e24be-147">C#</span><span class="sxs-lookup"><span data-stu-id="e24be-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e24be-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e24be-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e24be-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e24be-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e24be-150">Java</span><span class="sxs-lookup"><span data-stu-id="e24be-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e24be-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e24be-151">Response</span></span>
<span data-ttu-id="e24be-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e24be-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

