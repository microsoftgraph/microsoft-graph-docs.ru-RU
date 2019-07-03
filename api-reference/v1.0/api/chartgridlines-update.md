---
title: Обновление объекта chartgridlines
description: Обновление свойств объекта chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b8aab64a94cdf41805be80fa8c5ca6e897e9b61f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443408"
---
# <a name="update-chartgridlines"></a><span data-ttu-id="b94e2-103">Обновление объекта chartgridlines</span><span class="sxs-lookup"><span data-stu-id="b94e2-103">Update chartgridlines</span></span>

<span data-ttu-id="b94e2-104">Обновление свойств объекта chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="b94e2-104">Update the properties of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b94e2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b94e2-105">Permissions</span></span>
<span data-ttu-id="b94e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b94e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b94e2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b94e2-108">Permission type</span></span>      | <span data-ttu-id="b94e2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b94e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b94e2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b94e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b94e2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b94e2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b94e2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b94e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b94e2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b94e2-113">Not supported.</span></span>    |
|<span data-ttu-id="b94e2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b94e2-114">Application</span></span> | <span data-ttu-id="b94e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b94e2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b94e2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b94e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/majorGridlines
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorGridlines
```
## <a name="request-headers"></a><span data-ttu-id="b94e2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b94e2-117">Request headers</span></span>
| <span data-ttu-id="b94e2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b94e2-118">Name</span></span>       | <span data-ttu-id="b94e2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b94e2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b94e2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b94e2-120">Authorization</span></span>  | <span data-ttu-id="b94e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b94e2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b94e2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b94e2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b94e2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b94e2-126">Request body</span></span>
<span data-ttu-id="b94e2-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b94e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b94e2-130">Property</span></span>     | <span data-ttu-id="b94e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b94e2-131">Type</span></span>   |<span data-ttu-id="b94e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b94e2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b94e2-133">visible</span><span class="sxs-lookup"><span data-stu-id="b94e2-133">visible</span></span>|<span data-ttu-id="b94e2-134">boolean</span><span class="sxs-lookup"><span data-stu-id="b94e2-134">boolean</span></span>|<span data-ttu-id="b94e2-135">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="b94e2-135">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="b94e2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b94e2-136">Response</span></span>

<span data-ttu-id="b94e2-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартгридлинес](../resources/chartgridlines.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b94e2-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartGridlines](../resources/chartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b94e2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b94e2-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b94e2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b94e2-139">Request</span></span>
<span data-ttu-id="b94e2-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b94e2-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b94e2-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b94e2-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartgridlines"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b94e2-142">C#</span><span class="sxs-lookup"><span data-stu-id="b94e2-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b94e2-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="b94e2-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b94e2-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b94e2-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b94e2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b94e2-145">Response</span></span>
<span data-ttu-id="b94e2-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b94e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartgridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
