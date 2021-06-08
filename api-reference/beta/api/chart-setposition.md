---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 03078c00054f2efd683eff85973302319b5a2efb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786540"
---
# <a name="chart-setposition"></a><span data-ttu-id="8b669-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="8b669-103">Chart: setPosition</span></span>

<span data-ttu-id="8b669-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b669-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b669-105">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="8b669-105">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b669-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b669-106">Permissions</span></span>
<span data-ttu-id="8b669-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b669-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b669-109">Permission type</span></span>      | <span data-ttu-id="8b669-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b669-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b669-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b669-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8b669-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b669-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b669-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b669-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b669-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b669-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b669-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b669-115">Application</span></span> | <span data-ttu-id="8b669-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b669-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b669-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b669-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="8b669-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b669-118">Request headers</span></span>
| <span data-ttu-id="8b669-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8b669-119">Name</span></span>       | <span data-ttu-id="8b669-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8b669-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b669-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b669-121">Authorization</span></span>  | <span data-ttu-id="8b669-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b669-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b669-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8b669-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b669-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8b669-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b669-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b669-127">Request body</span></span>
<span data-ttu-id="8b669-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8b669-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b669-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="8b669-129">Parameter</span></span>    | <span data-ttu-id="8b669-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8b669-130">Type</span></span>   |<span data-ttu-id="8b669-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8b669-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b669-132">startCell</span><span class="sxs-lookup"><span data-stu-id="8b669-132">startCell</span></span>|<span data-ttu-id="8b669-133">string</span><span class="sxs-lookup"><span data-stu-id="8b669-133">string</span></span>|<span data-ttu-id="8b669-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="8b669-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="8b669-137">endCell</span><span class="sxs-lookup"><span data-stu-id="8b669-137">endCell</span></span>|<span data-ttu-id="8b669-138">string</span><span class="sxs-lookup"><span data-stu-id="8b669-138">string</span></span>|<span data-ttu-id="8b669-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="8b669-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="8b669-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b669-142">Response</span></span>

<span data-ttu-id="8b669-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8b669-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b669-145">Пример</span><span class="sxs-lookup"><span data-stu-id="8b669-145">Example</span></span>
<span data-ttu-id="8b669-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8b669-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8b669-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b669-147">Request</span></span>
<span data-ttu-id="8b669-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b669-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b669-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b669-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b669-150">C#</span><span class="sxs-lookup"><span data-stu-id="8b669-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chart-setposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b669-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b669-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chart-setposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b669-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b669-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chart-setposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b669-153">Java</span><span class="sxs-lookup"><span data-stu-id="8b669-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chart-setposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8b669-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b669-154">Response</span></span>
<span data-ttu-id="8b669-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b669-155">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


