---
title: Обновление объекта RangeBorder
description: Обновление свойств объекта rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0c6f6d53cddacc5e54031aaa9830f15b1573814d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454646"
---
# <a name="update-rangeborder"></a><span data-ttu-id="66504-103">Обновление объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="66504-103">Update rangeborder</span></span>

<span data-ttu-id="66504-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="66504-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66504-105">Обновление свойств объекта rangeborder.</span><span class="sxs-lookup"><span data-stu-id="66504-105">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="66504-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66504-106">Permissions</span></span>
<span data-ttu-id="66504-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66504-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66504-109">Permission type</span></span>      | <span data-ttu-id="66504-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66504-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66504-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66504-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66504-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66504-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66504-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66504-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66504-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66504-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66504-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66504-115">Application</span></span> | <span data-ttu-id="66504-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66504-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66504-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66504-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="66504-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66504-118">Optional request headers</span></span>
| <span data-ttu-id="66504-119">Имя</span><span class="sxs-lookup"><span data-stu-id="66504-119">Name</span></span>       | <span data-ttu-id="66504-120">Описание</span><span class="sxs-lookup"><span data-stu-id="66504-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="66504-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66504-121">Authorization</span></span>  | <span data-ttu-id="66504-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66504-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66504-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="66504-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="66504-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="66504-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66504-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66504-127">Request body</span></span>
<span data-ttu-id="66504-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="66504-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="66504-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="66504-131">Property</span></span>     | <span data-ttu-id="66504-132">Тип</span><span class="sxs-lookup"><span data-stu-id="66504-132">Type</span></span>   |<span data-ttu-id="66504-133">Описание</span><span class="sxs-lookup"><span data-stu-id="66504-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66504-134">color</span><span class="sxs-lookup"><span data-stu-id="66504-134">color</span></span>|<span data-ttu-id="66504-135">строка</span><span class="sxs-lookup"><span data-stu-id="66504-135">string</span></span>|<span data-ttu-id="66504-136">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="66504-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="66504-137">style</span><span class="sxs-lookup"><span data-stu-id="66504-137">style</span></span>|<span data-ttu-id="66504-138">string</span><span class="sxs-lookup"><span data-stu-id="66504-138">string</span></span>|<span data-ttu-id="66504-p105">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="66504-p105">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="66504-141">weight</span><span class="sxs-lookup"><span data-stu-id="66504-141">weight</span></span>|<span data-ttu-id="66504-142">string</span><span class="sxs-lookup"><span data-stu-id="66504-142">string</span></span>|<span data-ttu-id="66504-p106">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="66504-p106">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="66504-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="66504-145">Response</span></span>

<span data-ttu-id="66504-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжебордер](../resources/workbookrangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66504-146">If successful, this method returns a `200 OK` response code and updated [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66504-147">Пример</span><span class="sxs-lookup"><span data-stu-id="66504-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66504-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="66504-148">Request</span></span>
<span data-ttu-id="66504-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66504-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66504-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="66504-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="66504-151">C#</span><span class="sxs-lookup"><span data-stu-id="66504-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeborder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66504-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66504-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeborder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66504-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66504-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeborder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="66504-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="66504-154">Response</span></span>
<span data-ttu-id="66504-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66504-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
