---
title: Обновление объекта chartAxis
description: Обновление свойств объекта chartaxis.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0b6d30befd31d36ddaad25270126ef98f9d8402f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048836"
---
# <a name="update-chartaxis"></a><span data-ttu-id="4ea3a-103">Обновление объекта chartAxis</span><span class="sxs-lookup"><span data-stu-id="4ea3a-103">Update chartaxis</span></span>

<span data-ttu-id="4ea3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea3a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ea3a-105">Обновление свойств объекта chartaxis.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-105">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ea3a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea3a-106">Permissions</span></span>
<span data-ttu-id="4ea3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea3a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea3a-109">Permission type</span></span>      | <span data-ttu-id="4ea3a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ea3a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ea3a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ea3a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ea3a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ea3a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ea3a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ea3a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ea3a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-114">Not supported.</span></span>    |
|<span data-ttu-id="4ea3a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ea3a-115">Application</span></span> | <span data-ttu-id="4ea3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ea3a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ea3a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="4ea3a-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ea3a-118">Optional request headers</span></span>
| <span data-ttu-id="4ea3a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4ea3a-119">Name</span></span>       | <span data-ttu-id="4ea3a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea3a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4ea3a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ea3a-121">Authorization</span></span>  | <span data-ttu-id="4ea3a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ea3a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4ea3a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4ea3a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ea3a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ea3a-127">Request body</span></span>
<span data-ttu-id="4ea3a-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4ea3a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ea3a-131">Property</span></span>     | <span data-ttu-id="4ea3a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4ea3a-132">Type</span></span>   |<span data-ttu-id="4ea3a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea3a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ea3a-134">majorUnit</span><span class="sxs-lookup"><span data-stu-id="4ea3a-134">majorUnit</span></span>|<span data-ttu-id="4ea3a-135">Json</span><span class="sxs-lookup"><span data-stu-id="4ea3a-135">Json</span></span>|<span data-ttu-id="4ea3a-p105">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="4ea3a-139">maximum</span><span class="sxs-lookup"><span data-stu-id="4ea3a-139">maximum</span></span>|<span data-ttu-id="4ea3a-140">Json</span><span class="sxs-lookup"><span data-stu-id="4ea3a-140">Json</span></span>|<span data-ttu-id="4ea3a-p106">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="4ea3a-144">minimum</span><span class="sxs-lookup"><span data-stu-id="4ea3a-144">minimum</span></span>|<span data-ttu-id="4ea3a-145">Json</span><span class="sxs-lookup"><span data-stu-id="4ea3a-145">Json</span></span>|<span data-ttu-id="4ea3a-p107">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="4ea3a-149">minorUnit</span><span class="sxs-lookup"><span data-stu-id="4ea3a-149">minorUnit</span></span>|<span data-ttu-id="4ea3a-150">Json</span><span class="sxs-lookup"><span data-stu-id="4ea3a-150">Json</span></span>|<span data-ttu-id="4ea3a-p108">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="4ea3a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ea3a-154">Response</span></span>

<span data-ttu-id="4ea3a-155">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [WorkbookChartAxis](../resources/chartaxis.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-155">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ea3a-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4ea3a-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ea3a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ea3a-157">Request</span></span>
<span data-ttu-id="4ea3a-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ea3a-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea3a-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4ea3a-160">C#</span><span class="sxs-lookup"><span data-stu-id="4ea3a-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ea3a-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ea3a-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ea3a-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ea3a-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ea3a-163">Java</span><span class="sxs-lookup"><span data-stu-id="4ea3a-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartaxis-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4ea3a-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ea3a-164">Response</span></span>
<span data-ttu-id="4ea3a-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-165">Here is an example of the response.</span></span> <span data-ttu-id="4ea3a-166">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4ea3a-166">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

