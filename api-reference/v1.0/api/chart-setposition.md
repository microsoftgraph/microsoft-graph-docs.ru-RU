---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 060eb647910ba90e47b6c1943309e71208876ca6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882140"
---
# <a name="chart-setposition"></a><span data-ttu-id="55fbb-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="55fbb-103">Chart: setPosition</span></span>

<span data-ttu-id="55fbb-104">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="55fbb-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="55fbb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55fbb-105">Permissions</span></span>
<span data-ttu-id="55fbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55fbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55fbb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55fbb-108">Permission type</span></span>      | <span data-ttu-id="55fbb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55fbb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55fbb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55fbb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55fbb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55fbb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="55fbb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55fbb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55fbb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55fbb-113">Not supported.</span></span>    |
|<span data-ttu-id="55fbb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55fbb-114">Application</span></span> | <span data-ttu-id="55fbb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55fbb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55fbb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55fbb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="55fbb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55fbb-117">Request headers</span></span>
| <span data-ttu-id="55fbb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="55fbb-118">Name</span></span>       | <span data-ttu-id="55fbb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="55fbb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="55fbb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55fbb-120">Authorization</span></span>  | <span data-ttu-id="55fbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55fbb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55fbb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="55fbb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="55fbb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="55fbb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55fbb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55fbb-126">Request body</span></span>
<span data-ttu-id="55fbb-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="55fbb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55fbb-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="55fbb-128">Parameter</span></span>    | <span data-ttu-id="55fbb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="55fbb-129">Type</span></span>   |<span data-ttu-id="55fbb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="55fbb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55fbb-131">startCell</span><span class="sxs-lookup"><span data-stu-id="55fbb-131">startCell</span></span>|<span data-ttu-id="55fbb-132">Json</span><span class="sxs-lookup"><span data-stu-id="55fbb-132">Json</span></span>|<span data-ttu-id="55fbb-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="55fbb-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="55fbb-136">endCell</span><span class="sxs-lookup"><span data-stu-id="55fbb-136">endCell</span></span>|<span data-ttu-id="55fbb-137">Json</span><span class="sxs-lookup"><span data-stu-id="55fbb-137">Json</span></span>|<span data-ttu-id="55fbb-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="55fbb-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="55fbb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="55fbb-141">Response</span></span>

<span data-ttu-id="55fbb-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="55fbb-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55fbb-144">Пример</span><span class="sxs-lookup"><span data-stu-id="55fbb-144">Example</span></span>
<span data-ttu-id="55fbb-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="55fbb-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="55fbb-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="55fbb-146">Request</span></span>
<span data-ttu-id="55fbb-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55fbb-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="55fbb-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="55fbb-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55fbb-149">C#</span><span class="sxs-lookup"><span data-stu-id="55fbb-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55fbb-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="55fbb-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55fbb-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="55fbb-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="55fbb-152">Java</span><span class="sxs-lookup"><span data-stu-id="55fbb-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55fbb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="55fbb-153">Response</span></span>
<span data-ttu-id="55fbb-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55fbb-154">Here is an example of the response.</span></span> 
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
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
