---
title: 'WorksheetCollection: add'
description: .activate() на нем.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: afb5f118ad467c769df2ae59b082e95e2d8a9ce2
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573601"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="28e57-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="28e57-103">WorksheetCollection: add</span></span>

<span data-ttu-id="28e57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e57-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28e57-105">Добавляет новый лист в книгу.</span><span class="sxs-lookup"><span data-stu-id="28e57-105">Adds a new worksheet to the workbook.</span></span> <span data-ttu-id="28e57-106">Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="28e57-106">The worksheet will be added at the end of existing worksheets.</span></span> <span data-ttu-id="28e57-107">Если вы хотите активировать только что добавленный таблицу, позвоните .activate() на нем.</span><span class="sxs-lookup"><span data-stu-id="28e57-107">If you wish to activate the newly added worksheet, call .activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="28e57-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28e57-108">Permissions</span></span>
<span data-ttu-id="28e57-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28e57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28e57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28e57-111">Permission type</span></span>      | <span data-ttu-id="28e57-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28e57-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28e57-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28e57-113">Delegated (work or school account)</span></span> | <span data-ttu-id="28e57-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28e57-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="28e57-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28e57-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28e57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28e57-116">Not supported.</span></span>    |
|<span data-ttu-id="28e57-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28e57-117">Application</span></span> | <span data-ttu-id="28e57-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28e57-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28e57-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28e57-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/
POST /me/drive/root:/{item-path}:/workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="28e57-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28e57-120">Request headers</span></span>
| <span data-ttu-id="28e57-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28e57-121">Name</span></span>       | <span data-ttu-id="28e57-122">Описание</span><span class="sxs-lookup"><span data-stu-id="28e57-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28e57-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28e57-123">Authorization</span></span>  | <span data-ttu-id="28e57-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28e57-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28e57-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="28e57-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="28e57-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="28e57-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28e57-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28e57-129">Request body</span></span>
<span data-ttu-id="28e57-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="28e57-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="28e57-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="28e57-131">Parameter</span></span>    | <span data-ttu-id="28e57-132">Тип</span><span class="sxs-lookup"><span data-stu-id="28e57-132">Type</span></span>   |<span data-ttu-id="28e57-133">Описание</span><span class="sxs-lookup"><span data-stu-id="28e57-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28e57-134">name</span><span class="sxs-lookup"><span data-stu-id="28e57-134">name</span></span>|<span data-ttu-id="28e57-135">string</span><span class="sxs-lookup"><span data-stu-id="28e57-135">string</span></span>|<span data-ttu-id="28e57-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="28e57-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="28e57-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="28e57-140">Response</span></span>

<span data-ttu-id="28e57-141">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект WorkbookWorksheet](../resources/worksheet.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="28e57-141">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e57-142">Пример</span><span class="sxs-lookup"><span data-stu-id="28e57-142">Example</span></span>
<span data-ttu-id="28e57-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="28e57-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="28e57-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="28e57-144">Request</span></span>
<span data-ttu-id="28e57-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28e57-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28e57-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="28e57-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="28e57-147">C#</span><span class="sxs-lookup"><span data-stu-id="28e57-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28e57-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28e57-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28e57-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28e57-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28e57-150">Java</span><span class="sxs-lookup"><span data-stu-id="28e57-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="28e57-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="28e57-151">Response</span></span>
<span data-ttu-id="28e57-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28e57-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

