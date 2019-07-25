---
title: Обновление листа
description: Обновление свойств объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 365ec4c2b3e13fa72c0925ff35c10bc1a85b6c45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884234"
---
# <a name="update-worksheet"></a><span data-ttu-id="75638-103">Обновление листа</span><span class="sxs-lookup"><span data-stu-id="75638-103">Update worksheet</span></span>

<span data-ttu-id="75638-104">Обновление свойств объекта листа.</span><span class="sxs-lookup"><span data-stu-id="75638-104">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="75638-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75638-105">Permissions</span></span>
<span data-ttu-id="75638-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75638-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75638-108">Permission type</span></span>      | <span data-ttu-id="75638-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75638-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75638-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75638-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75638-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75638-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75638-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75638-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75638-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75638-113">Not supported.</span></span>    |
|<span data-ttu-id="75638-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75638-114">Application</span></span> | <span data-ttu-id="75638-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75638-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75638-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75638-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="75638-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75638-117">Optional request headers</span></span>
| <span data-ttu-id="75638-118">Имя</span><span class="sxs-lookup"><span data-stu-id="75638-118">Name</span></span>       | <span data-ttu-id="75638-119">Описание</span><span class="sxs-lookup"><span data-stu-id="75638-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="75638-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75638-120">Authorization</span></span>  | <span data-ttu-id="75638-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75638-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75638-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75638-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="75638-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="75638-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75638-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75638-126">Request body</span></span>
<span data-ttu-id="75638-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="75638-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="75638-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75638-130">Property</span></span>     | <span data-ttu-id="75638-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75638-131">Type</span></span>   |<span data-ttu-id="75638-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75638-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75638-133">name</span><span class="sxs-lookup"><span data-stu-id="75638-133">name</span></span>|<span data-ttu-id="75638-134">string</span><span class="sxs-lookup"><span data-stu-id="75638-134">string</span></span>|<span data-ttu-id="75638-135">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="75638-135">The display name of the worksheet.</span></span>|
|<span data-ttu-id="75638-136">position</span><span class="sxs-lookup"><span data-stu-id="75638-136">position</span></span>|<span data-ttu-id="75638-137">int</span><span class="sxs-lookup"><span data-stu-id="75638-137">int</span></span>|<span data-ttu-id="75638-138">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="75638-138">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="75638-139">visibility</span><span class="sxs-lookup"><span data-stu-id="75638-139">visibility</span></span>|<span data-ttu-id="75638-140">string</span><span class="sxs-lookup"><span data-stu-id="75638-140">string</span></span>|<span data-ttu-id="75638-141">Видимость листа.</span><span class="sxs-lookup"><span data-stu-id="75638-141">The Visibility of the worksheet.</span></span> <span data-ttu-id="75638-142">Допустимые значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="75638-142">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="75638-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="75638-143">Response</span></span>

<span data-ttu-id="75638-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукворкшит](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75638-144">If successful, this method returns a `200 OK` response code and updated [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75638-145">Пример</span><span class="sxs-lookup"><span data-stu-id="75638-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75638-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="75638-146">Request</span></span>
<span data-ttu-id="75638-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75638-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="75638-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="75638-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="75638-149">C#</span><span class="sxs-lookup"><span data-stu-id="75638-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75638-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="75638-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="75638-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="75638-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="75638-152">Java</span><span class="sxs-lookup"><span data-stu-id="75638-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75638-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="75638-153">Response</span></span>
<span data-ttu-id="75638-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75638-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
