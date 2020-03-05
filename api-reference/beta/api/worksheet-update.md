---
title: Обновление листа
description: Обновление свойств объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cf3c19ec56b9d4da0efbc2e99fc208bb378a6008
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451178"
---
# <a name="update-worksheet"></a><span data-ttu-id="99bf4-103">Обновление листа</span><span class="sxs-lookup"><span data-stu-id="99bf4-103">Update worksheet</span></span>

<span data-ttu-id="99bf4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="99bf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99bf4-105">Обновление свойств объекта листа.</span><span class="sxs-lookup"><span data-stu-id="99bf4-105">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="99bf4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99bf4-106">Permissions</span></span>
<span data-ttu-id="99bf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99bf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99bf4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99bf4-109">Permission type</span></span>      | <span data-ttu-id="99bf4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99bf4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99bf4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99bf4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99bf4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99bf4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99bf4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99bf4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99bf4-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99bf4-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99bf4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99bf4-115">Application</span></span> | <span data-ttu-id="99bf4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99bf4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99bf4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99bf4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="99bf4-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99bf4-118">Optional request headers</span></span>
| <span data-ttu-id="99bf4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="99bf4-119">Name</span></span>       | <span data-ttu-id="99bf4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="99bf4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="99bf4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99bf4-121">Authorization</span></span>  | <span data-ttu-id="99bf4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99bf4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99bf4-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99bf4-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="99bf4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="99bf4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99bf4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99bf4-127">Request body</span></span>
<span data-ttu-id="99bf4-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="99bf4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="99bf4-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="99bf4-131">Property</span></span>     | <span data-ttu-id="99bf4-132">Тип</span><span class="sxs-lookup"><span data-stu-id="99bf4-132">Type</span></span>   |<span data-ttu-id="99bf4-133">Описание</span><span class="sxs-lookup"><span data-stu-id="99bf4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99bf4-134">name</span><span class="sxs-lookup"><span data-stu-id="99bf4-134">name</span></span>|<span data-ttu-id="99bf4-135">string</span><span class="sxs-lookup"><span data-stu-id="99bf4-135">string</span></span>|<span data-ttu-id="99bf4-136">Отображаемое имя листа.</span><span class="sxs-lookup"><span data-stu-id="99bf4-136">The display name of the worksheet.</span></span>|
|<span data-ttu-id="99bf4-137">position</span><span class="sxs-lookup"><span data-stu-id="99bf4-137">position</span></span>|<span data-ttu-id="99bf4-138">int</span><span class="sxs-lookup"><span data-stu-id="99bf4-138">int</span></span>|<span data-ttu-id="99bf4-139">Положение листа (начиная с нуля) в книге.</span><span class="sxs-lookup"><span data-stu-id="99bf4-139">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="99bf4-140">visibility</span><span class="sxs-lookup"><span data-stu-id="99bf4-140">visibility</span></span>|<span data-ttu-id="99bf4-141">string</span><span class="sxs-lookup"><span data-stu-id="99bf4-141">string</span></span>|<span data-ttu-id="99bf4-p105">Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="99bf4-p105">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="99bf4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="99bf4-144">Response</span></span>

<span data-ttu-id="99bf4-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукворкшит](../resources/workbookworksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99bf4-145">If successful, this method returns a `200 OK` response code and updated [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99bf4-146">Пример</span><span class="sxs-lookup"><span data-stu-id="99bf4-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99bf4-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="99bf4-147">Request</span></span>
<span data-ttu-id="99bf4-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99bf4-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99bf4-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="99bf4-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="99bf4-150">C#</span><span class="sxs-lookup"><span data-stu-id="99bf4-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99bf4-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99bf4-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99bf4-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99bf4-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99bf4-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="99bf4-153">Response</span></span>
<span data-ttu-id="99bf4-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99bf4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
