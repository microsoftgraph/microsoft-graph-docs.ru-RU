---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 07e3fe1c3a867015acc6430b8d5fc71a63498126
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983160"
---
# <a name="chart-setposition"></a><span data-ttu-id="4ca0a-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="4ca0a-103">Chart: setPosition</span></span>

<span data-ttu-id="4ca0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ca0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ca0a-105">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-105">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ca0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ca0a-106">Permissions</span></span>
<span data-ttu-id="4ca0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ca0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ca0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ca0a-109">Permission type</span></span>      | <span data-ttu-id="4ca0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ca0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ca0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ca0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ca0a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ca0a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ca0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ca0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ca0a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ca0a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ca0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ca0a-115">Application</span></span> | <span data-ttu-id="4ca0a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ca0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ca0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="4ca0a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ca0a-118">Request headers</span></span>
| <span data-ttu-id="4ca0a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4ca0a-119">Name</span></span>       | <span data-ttu-id="4ca0a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ca0a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ca0a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ca0a-121">Authorization</span></span>  | <span data-ttu-id="4ca0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ca0a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4ca0a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="4ca0a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ca0a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ca0a-127">Request body</span></span>
<span data-ttu-id="4ca0a-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4ca0a-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="4ca0a-129">Parameter</span></span>    | <span data-ttu-id="4ca0a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4ca0a-130">Type</span></span>   |<span data-ttu-id="4ca0a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4ca0a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ca0a-132">startCell</span><span class="sxs-lookup"><span data-stu-id="4ca0a-132">startCell</span></span>|<span data-ttu-id="4ca0a-133">string</span><span class="sxs-lookup"><span data-stu-id="4ca0a-133">string</span></span>|<span data-ttu-id="4ca0a-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="4ca0a-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="4ca0a-137">endCell</span><span class="sxs-lookup"><span data-stu-id="4ca0a-137">endCell</span></span>|<span data-ttu-id="4ca0a-138">string</span><span class="sxs-lookup"><span data-stu-id="4ca0a-138">string</span></span>|<span data-ttu-id="4ca0a-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="4ca0a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ca0a-142">Response</span></span>

<span data-ttu-id="4ca0a-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca0a-145">Пример</span><span class="sxs-lookup"><span data-stu-id="4ca0a-145">Example</span></span>
<span data-ttu-id="4ca0a-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ca0a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ca0a-147">Request</span></span>
<span data-ttu-id="4ca0a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ca0a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ca0a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4ca0a-150">C#</span><span class="sxs-lookup"><span data-stu-id="4ca0a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ca0a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ca0a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ca0a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ca0a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ca0a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ca0a-153">Response</span></span>
<span data-ttu-id="4ca0a-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ca0a-154">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


