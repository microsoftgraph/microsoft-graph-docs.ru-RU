---
title: Обновление объекта RangeBorder
description: Обновление свойств объекта rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: df26b12d69cb781a2064b088271dcb7c37667b4f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988386"
---
# <a name="update-rangeborder"></a><span data-ttu-id="d6379-103">Обновление объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d6379-103">Update rangeborder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6379-104">Обновление свойств объекта rangeborder.</span><span class="sxs-lookup"><span data-stu-id="d6379-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6379-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6379-105">Permissions</span></span>
<span data-ttu-id="d6379-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6379-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6379-108">Permission type</span></span>      | <span data-ttu-id="d6379-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6379-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6379-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6379-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6379-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6379-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6379-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6379-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6379-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6379-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6379-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6379-114">Application</span></span> | <span data-ttu-id="d6379-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6379-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6379-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6379-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="d6379-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6379-117">Optional request headers</span></span>
| <span data-ttu-id="d6379-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d6379-118">Name</span></span>       | <span data-ttu-id="d6379-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d6379-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d6379-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6379-120">Authorization</span></span>  | <span data-ttu-id="d6379-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6379-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6379-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d6379-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d6379-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d6379-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6379-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6379-126">Request body</span></span>
<span data-ttu-id="d6379-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d6379-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d6379-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6379-130">Property</span></span>     | <span data-ttu-id="d6379-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6379-131">Type</span></span>   |<span data-ttu-id="d6379-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6379-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6379-133">color</span><span class="sxs-lookup"><span data-stu-id="d6379-133">color</span></span>|<span data-ttu-id="d6379-134">строка</span><span class="sxs-lookup"><span data-stu-id="d6379-134">string</span></span>|<span data-ttu-id="d6379-135">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="d6379-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="d6379-136">style</span><span class="sxs-lookup"><span data-stu-id="d6379-136">style</span></span>|<span data-ttu-id="d6379-137">string</span><span class="sxs-lookup"><span data-stu-id="d6379-137">string</span></span>|<span data-ttu-id="d6379-p105">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="d6379-p105">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="d6379-140">weight</span><span class="sxs-lookup"><span data-stu-id="d6379-140">weight</span></span>|<span data-ttu-id="d6379-141">string</span><span class="sxs-lookup"><span data-stu-id="d6379-141">string</span></span>|<span data-ttu-id="d6379-p106">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="d6379-p106">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="d6379-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6379-144">Response</span></span>

<span data-ttu-id="d6379-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжебордер](../resources/workbookrangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6379-145">If successful, this method returns a `200 OK` response code and updated [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6379-146">Пример</span><span class="sxs-lookup"><span data-stu-id="d6379-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6379-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6379-147">Request</span></span>
<span data-ttu-id="d6379-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6379-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6379-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6379-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6379-150">C#</span><span class="sxs-lookup"><span data-stu-id="d6379-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeborder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6379-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6379-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeborder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6379-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d6379-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeborder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6379-153">Java</span><span class="sxs-lookup"><span data-stu-id="d6379-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeborder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6379-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6379-154">Response</span></span>
<span data-ttu-id="d6379-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6379-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
