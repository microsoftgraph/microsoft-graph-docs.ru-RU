---
title: 'WorksheetCollection: add'
description: . Активируйте ().
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3bd363a48c3e99133246b1ab46c0d7fcb4d8aa1b
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645263"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="23f77-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="23f77-103">WorksheetCollection: add</span></span>

<span data-ttu-id="23f77-104">Добавляет новый лист в книгу.</span><span class="sxs-lookup"><span data-stu-id="23f77-104">Adds a new worksheet to the workbook.</span></span> <span data-ttu-id="23f77-105">Лист будет добавлен после существующих листов.</span><span class="sxs-lookup"><span data-stu-id="23f77-105">The worksheet will be added at the end of existing worksheets.</span></span> <span data-ttu-id="23f77-106">Если вы хотите активировать недавно добавленный лист, вызовите. Activate ().</span><span class="sxs-lookup"><span data-stu-id="23f77-106">If you wish to activate the newly added worksheet, call .activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="23f77-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23f77-107">Permissions</span></span>
<span data-ttu-id="23f77-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23f77-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23f77-110">Permission type</span></span>      | <span data-ttu-id="23f77-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23f77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f77-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23f77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23f77-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23f77-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="23f77-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23f77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f77-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f77-115">Not supported.</span></span>    |
|<span data-ttu-id="23f77-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23f77-116">Application</span></span> | <span data-ttu-id="23f77-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f77-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23f77-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23f77-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="23f77-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23f77-119">Request headers</span></span>
| <span data-ttu-id="23f77-120">Имя</span><span class="sxs-lookup"><span data-stu-id="23f77-120">Name</span></span>       | <span data-ttu-id="23f77-121">Описание</span><span class="sxs-lookup"><span data-stu-id="23f77-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="23f77-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23f77-122">Authorization</span></span>  | <span data-ttu-id="23f77-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23f77-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23f77-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="23f77-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="23f77-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="23f77-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23f77-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23f77-128">Request body</span></span>
<span data-ttu-id="23f77-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="23f77-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23f77-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="23f77-130">Parameter</span></span>    | <span data-ttu-id="23f77-131">Тип</span><span class="sxs-lookup"><span data-stu-id="23f77-131">Type</span></span>   |<span data-ttu-id="23f77-132">Описание</span><span class="sxs-lookup"><span data-stu-id="23f77-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23f77-133">name</span><span class="sxs-lookup"><span data-stu-id="23f77-133">name</span></span>|<span data-ttu-id="23f77-134">string</span><span class="sxs-lookup"><span data-stu-id="23f77-134">string</span></span>|<span data-ttu-id="23f77-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="23f77-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="23f77-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f77-139">Response</span></span>

<span data-ttu-id="23f77-140">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукворкшит](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23f77-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23f77-141">Пример</span><span class="sxs-lookup"><span data-stu-id="23f77-141">Example</span></span>
<span data-ttu-id="23f77-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="23f77-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="23f77-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="23f77-143">Request</span></span>
<span data-ttu-id="23f77-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23f77-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23f77-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="23f77-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="23f77-146">C#</span><span class="sxs-lookup"><span data-stu-id="23f77-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23f77-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="23f77-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23f77-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="23f77-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23f77-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f77-149">Response</span></span>
<span data-ttu-id="23f77-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23f77-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
