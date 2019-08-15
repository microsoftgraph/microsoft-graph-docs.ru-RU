---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 54e35816906b969d7ce1d0aefb8abd11c5bc8caf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418602"
---
# <a name="chart-setposition"></a><span data-ttu-id="81593-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="81593-103">Chart: setPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81593-104">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="81593-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="81593-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81593-105">Permissions</span></span>
<span data-ttu-id="81593-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81593-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81593-108">Permission type</span></span>      | <span data-ttu-id="81593-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81593-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81593-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81593-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81593-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81593-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81593-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81593-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81593-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81593-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81593-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81593-114">Application</span></span> | <span data-ttu-id="81593-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81593-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81593-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81593-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="81593-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81593-117">Request headers</span></span>
| <span data-ttu-id="81593-118">Имя</span><span class="sxs-lookup"><span data-stu-id="81593-118">Name</span></span>       | <span data-ttu-id="81593-119">Описание</span><span class="sxs-lookup"><span data-stu-id="81593-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81593-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81593-120">Authorization</span></span>  | <span data-ttu-id="81593-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81593-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81593-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="81593-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="81593-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="81593-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81593-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81593-126">Request body</span></span>
<span data-ttu-id="81593-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="81593-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81593-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="81593-128">Parameter</span></span>    | <span data-ttu-id="81593-129">Тип</span><span class="sxs-lookup"><span data-stu-id="81593-129">Type</span></span>   |<span data-ttu-id="81593-130">Описание</span><span class="sxs-lookup"><span data-stu-id="81593-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81593-131">startCell</span><span class="sxs-lookup"><span data-stu-id="81593-131">startCell</span></span>|<span data-ttu-id="81593-132">string</span><span class="sxs-lookup"><span data-stu-id="81593-132">string</span></span>|<span data-ttu-id="81593-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="81593-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="81593-136">endCell</span><span class="sxs-lookup"><span data-stu-id="81593-136">endCell</span></span>|<span data-ttu-id="81593-137">string</span><span class="sxs-lookup"><span data-stu-id="81593-137">string</span></span>|<span data-ttu-id="81593-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="81593-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="81593-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="81593-141">Response</span></span>

<span data-ttu-id="81593-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="81593-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81593-144">Пример</span><span class="sxs-lookup"><span data-stu-id="81593-144">Example</span></span>
<span data-ttu-id="81593-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="81593-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81593-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="81593-146">Request</span></span>
<span data-ttu-id="81593-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81593-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81593-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="81593-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="81593-149">C#</span><span class="sxs-lookup"><span data-stu-id="81593-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81593-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81593-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81593-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="81593-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81593-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="81593-152">Response</span></span>
<span data-ttu-id="81593-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81593-153">Here is an example of the response.</span></span> 
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
