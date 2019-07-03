---
title: 'Chart: setData'
description: Сбрасывает исходные данные для диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ef1f973cae35b2d908c060475b9c2bd04b982525
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443583"
---
# <a name="chart-setdata"></a><span data-ttu-id="6bcd6-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="6bcd6-103">Chart: setData</span></span>

<span data-ttu-id="6bcd6-104">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="6bcd6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bcd6-105">Permissions</span></span>
<span data-ttu-id="6bcd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bcd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bcd6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bcd6-108">Permission type</span></span>      | <span data-ttu-id="6bcd6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bcd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bcd6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bcd6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6bcd6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bcd6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6bcd6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bcd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bcd6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-113">Not supported.</span></span>    |
|<span data-ttu-id="6bcd6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bcd6-114">Application</span></span> | <span data-ttu-id="6bcd6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bcd6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bcd6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="6bcd6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bcd6-117">Request headers</span></span>
| <span data-ttu-id="6bcd6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6bcd6-118">Name</span></span>       | <span data-ttu-id="6bcd6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6bcd6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6bcd6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6bcd6-120">Authorization</span></span>  | <span data-ttu-id="6bcd6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6bcd6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6bcd6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6bcd6-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bcd6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6bcd6-126">Request body</span></span>
<span data-ttu-id="6bcd6-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6bcd6-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="6bcd6-128">Parameter</span></span>    | <span data-ttu-id="6bcd6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6bcd6-129">Type</span></span>   |<span data-ttu-id="6bcd6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6bcd6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bcd6-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="6bcd6-131">sourceData</span></span>|<span data-ttu-id="6bcd6-132">Json</span><span class="sxs-lookup"><span data-stu-id="6bcd6-132">Json</span></span>|<span data-ttu-id="6bcd6-133">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="6bcd6-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="6bcd6-134">seriesBy</span></span>|<span data-ttu-id="6bcd6-135">string</span><span class="sxs-lookup"><span data-stu-id="6bcd6-135">string</span></span>|<span data-ttu-id="6bcd6-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-136">Optional.</span></span> <span data-ttu-id="6bcd6-137">Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-137">Specifies the way columns or rows are used as data series on the chart.</span></span> <span data-ttu-id="6bcd6-138">Может иметь одно из следующих значений: Auto (по умолчанию), Rows, Columns.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-138">Can be one of the following: Auto (default), Rows, Columns.</span></span>  <span data-ttu-id="6bcd6-139">Допустимые значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-139">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="6bcd6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bcd6-140">Response</span></span>

<span data-ttu-id="6bcd6-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bcd6-143">Пример</span><span class="sxs-lookup"><span data-stu-id="6bcd6-143">Example</span></span>
<span data-ttu-id="6bcd6-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6bcd6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bcd6-145">Request</span></span>
<span data-ttu-id="6bcd6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-146">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6bcd6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bcd6-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6bcd6-148">C#</span><span class="sxs-lookup"><span data-stu-id="6bcd6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6bcd6-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="6bcd6-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6bcd6-150">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6bcd6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6bcd6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bcd6-151">Response</span></span>
<span data-ttu-id="6bcd6-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6bcd6-152">Here is an example of the response.</span></span> 
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
