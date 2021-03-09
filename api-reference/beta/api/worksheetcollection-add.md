---
title: 'WorksheetCollection: add'
description: .activate() на нем.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a4c587117beeb6e06e7a683dd119d8199c3e940c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578166"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="33fd1-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="33fd1-103">WorksheetCollection: add</span></span>

<span data-ttu-id="33fd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33fd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33fd1-p101">Добавляет новый лист в книгу. Лист будет добавлен в конец набора имеющихся листов. Если вы хотите активировать только что добавленный лист, вызовите команду .activate().</span><span class="sxs-lookup"><span data-stu-id="33fd1-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="33fd1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33fd1-108">Permissions</span></span>
<span data-ttu-id="33fd1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33fd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33fd1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33fd1-111">Permission type</span></span>      | <span data-ttu-id="33fd1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33fd1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33fd1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33fd1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="33fd1-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33fd1-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33fd1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33fd1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33fd1-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33fd1-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33fd1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33fd1-117">Application</span></span> | <span data-ttu-id="33fd1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33fd1-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33fd1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33fd1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/
POST /me/drive/root:/{item-path}:/workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="33fd1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33fd1-120">Request headers</span></span>
| <span data-ttu-id="33fd1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="33fd1-121">Name</span></span>       | <span data-ttu-id="33fd1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="33fd1-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="33fd1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33fd1-123">Authorization</span></span>  | <span data-ttu-id="33fd1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33fd1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33fd1-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="33fd1-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="33fd1-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="33fd1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33fd1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33fd1-129">Request body</span></span>
<span data-ttu-id="33fd1-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="33fd1-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33fd1-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="33fd1-131">Parameter</span></span>    | <span data-ttu-id="33fd1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="33fd1-132">Type</span></span>   |<span data-ttu-id="33fd1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="33fd1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33fd1-134">name</span><span class="sxs-lookup"><span data-stu-id="33fd1-134">name</span></span>|<span data-ttu-id="33fd1-135">string</span><span class="sxs-lookup"><span data-stu-id="33fd1-135">string</span></span>|<span data-ttu-id="33fd1-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="33fd1-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="33fd1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="33fd1-140">Response</span></span>

<span data-ttu-id="33fd1-141">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [workbookWorksheet](../resources/workbookworksheet.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="33fd1-141">If successful, this method returns `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33fd1-142">Пример</span><span class="sxs-lookup"><span data-stu-id="33fd1-142">Example</span></span>
<span data-ttu-id="33fd1-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="33fd1-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33fd1-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="33fd1-144">Request</span></span>
<span data-ttu-id="33fd1-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33fd1-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33fd1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="33fd1-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="33fd1-147">C#</span><span class="sxs-lookup"><span data-stu-id="33fd1-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheetcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33fd1-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33fd1-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheetcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33fd1-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33fd1-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheetcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33fd1-150">Java</span><span class="sxs-lookup"><span data-stu-id="33fd1-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheetcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33fd1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="33fd1-151">Response</span></span>
<span data-ttu-id="33fd1-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33fd1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


