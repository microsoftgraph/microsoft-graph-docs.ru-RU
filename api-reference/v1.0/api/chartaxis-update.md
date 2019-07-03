---
title: Обновление объекта chartAxis
description: Обновление свойств объекта chartaxis.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9b494c13be480a00537ebc515c9ee1e65d477d5c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443513"
---
# <a name="update-chartaxis"></a><span data-ttu-id="8f4aa-103">Обновление объекта chartAxis</span><span class="sxs-lookup"><span data-stu-id="8f4aa-103">Update chartaxis</span></span>

<span data-ttu-id="8f4aa-104">Обновление свойств объекта chartaxis.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-104">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f4aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f4aa-105">Permissions</span></span>
<span data-ttu-id="8f4aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f4aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f4aa-108">Permission type</span></span>      | <span data-ttu-id="8f4aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f4aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f4aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f4aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f4aa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4aa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f4aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f4aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f4aa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-113">Not supported.</span></span>    |
|<span data-ttu-id="8f4aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f4aa-114">Application</span></span> | <span data-ttu-id="8f4aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f4aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f4aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="8f4aa-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f4aa-117">Optional request headers</span></span>
| <span data-ttu-id="8f4aa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8f4aa-118">Name</span></span>       | <span data-ttu-id="8f4aa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8f4aa-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8f4aa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f4aa-120">Authorization</span></span>  | <span data-ttu-id="8f4aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f4aa-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f4aa-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f4aa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f4aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f4aa-126">Request body</span></span>
<span data-ttu-id="8f4aa-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8f4aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f4aa-130">Property</span></span>     | <span data-ttu-id="8f4aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f4aa-131">Type</span></span>   |<span data-ttu-id="8f4aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f4aa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f4aa-133">majorUnit</span><span class="sxs-lookup"><span data-stu-id="8f4aa-133">majorUnit</span></span>|<span data-ttu-id="8f4aa-134">Json</span><span class="sxs-lookup"><span data-stu-id="8f4aa-134">Json</span></span>|<span data-ttu-id="8f4aa-p105">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="8f4aa-138">maximum</span><span class="sxs-lookup"><span data-stu-id="8f4aa-138">maximum</span></span>|<span data-ttu-id="8f4aa-139">Json</span><span class="sxs-lookup"><span data-stu-id="8f4aa-139">Json</span></span>|<span data-ttu-id="8f4aa-p106">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="8f4aa-143">minimum</span><span class="sxs-lookup"><span data-stu-id="8f4aa-143">minimum</span></span>|<span data-ttu-id="8f4aa-144">Json</span><span class="sxs-lookup"><span data-stu-id="8f4aa-144">Json</span></span>|<span data-ttu-id="8f4aa-p107">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="8f4aa-148">minorUnit</span><span class="sxs-lookup"><span data-stu-id="8f4aa-148">minorUnit</span></span>|<span data-ttu-id="8f4aa-149">Json</span><span class="sxs-lookup"><span data-stu-id="8f4aa-149">Json</span></span>|<span data-ttu-id="8f4aa-p108">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="8f4aa-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f4aa-153">Response</span></span>

<span data-ttu-id="8f4aa-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчартаксис](../resources/chartaxis.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-154">If successful, this method returns a `200 OK` response code and updated [WorkbookChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f4aa-155">Пример</span><span class="sxs-lookup"><span data-stu-id="8f4aa-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f4aa-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f4aa-156">Request</span></span>
<span data-ttu-id="8f4aa-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f4aa-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f4aa-158">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f4aa-159">C#</span><span class="sxs-lookup"><span data-stu-id="8f4aa-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartaxis-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f4aa-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f4aa-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartaxis-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f4aa-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f4aa-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartaxis-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8f4aa-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f4aa-162">Response</span></span>
<span data-ttu-id="8f4aa-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f4aa-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
