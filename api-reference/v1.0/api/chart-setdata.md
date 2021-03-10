---
title: 'Chart: setData'
description: Сбрасывает исходные данные для диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d944b58d46a6a5d1ec32b02b052b2f9db80e5d3f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575625"
---
# <a name="chart-setdata"></a><span data-ttu-id="4e558-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="4e558-103">Chart: setData</span></span>

<span data-ttu-id="4e558-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e558-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e558-105">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="4e558-105">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e558-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e558-106">Permissions</span></span>
<span data-ttu-id="4e558-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e558-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e558-109">Permission type</span></span>      | <span data-ttu-id="4e558-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e558-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e558-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e558-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4e558-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e558-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e558-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e558-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e558-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e558-114">Not supported.</span></span>    |
|<span data-ttu-id="4e558-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e558-115">Application</span></span> | <span data-ttu-id="4e558-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e558-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e558-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e558-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="4e558-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e558-118">Request headers</span></span>
| <span data-ttu-id="4e558-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4e558-119">Name</span></span>       | <span data-ttu-id="4e558-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4e558-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e558-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e558-121">Authorization</span></span>  | <span data-ttu-id="4e558-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e558-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e558-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4e558-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4e558-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e558-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e558-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e558-127">Request body</span></span>
<span data-ttu-id="4e558-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4e558-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e558-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="4e558-129">Parameter</span></span>    | <span data-ttu-id="4e558-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4e558-130">Type</span></span>   |<span data-ttu-id="4e558-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4e558-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e558-132">sourceData</span><span class="sxs-lookup"><span data-stu-id="4e558-132">sourceData</span></span>|<span data-ttu-id="4e558-133">Json</span><span class="sxs-lookup"><span data-stu-id="4e558-133">Json</span></span>|<span data-ttu-id="4e558-134">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="4e558-134">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="4e558-135">seriesBy</span><span class="sxs-lookup"><span data-stu-id="4e558-135">seriesBy</span></span>|<span data-ttu-id="4e558-136">string</span><span class="sxs-lookup"><span data-stu-id="4e558-136">string</span></span>|<span data-ttu-id="4e558-137">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4e558-137">Optional.</span></span> <span data-ttu-id="4e558-138">Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="4e558-138">Specifies the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="4e558-139">Может иметь одно из следующих значений: Auto (по умолчанию), Rows, Columns.</span><span class="sxs-lookup"><span data-stu-id="4e558-139">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="4e558-140">Допустимые значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="4e558-140">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="4e558-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e558-141">Response</span></span>

<span data-ttu-id="4e558-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4e558-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e558-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4e558-144">Example</span></span>
<span data-ttu-id="4e558-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4e558-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e558-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e558-146">Request</span></span>
<span data-ttu-id="4e558-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e558-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e558-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e558-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4e558-149">C#</span><span class="sxs-lookup"><span data-stu-id="4e558-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e558-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e558-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e558-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e558-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e558-152">Java</span><span class="sxs-lookup"><span data-stu-id="4e558-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e558-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e558-153">Response</span></span>
<span data-ttu-id="4e558-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e558-154">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

