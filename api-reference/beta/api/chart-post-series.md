---
title: Создание объекта ChartSeries
description: С помощью этого API можно создать объект ChartSeries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c97e468bdadb1980b168d2f15a4a21f340b88762
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418637"
---
# <a name="create-chartseries"></a><span data-ttu-id="9a690-103">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="9a690-103">Create ChartSeries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a690-104">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="9a690-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a690-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a690-105">Permissions</span></span>
<span data-ttu-id="9a690-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a690-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a690-108">Permission type</span></span>      | <span data-ttu-id="9a690-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a690-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a690-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a690-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a690-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a690-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a690-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a690-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a690-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a690-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a690-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a690-114">Application</span></span> | <span data-ttu-id="9a690-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a690-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a690-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a690-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="9a690-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a690-117">Request headers</span></span>
| <span data-ttu-id="9a690-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9a690-118">Name</span></span>       | <span data-ttu-id="9a690-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9a690-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a690-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a690-120">Authorization</span></span>  | <span data-ttu-id="9a690-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a690-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a690-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a690-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a690-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9a690-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a690-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a690-126">Request body</span></span>
<span data-ttu-id="9a690-127">В тексте запроса добавьте представление объекта [воркбукчартсериес](../resources/workbookchartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a690-127">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9a690-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a690-128">Response</span></span>

<span data-ttu-id="9a690-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбукчартсериес](../resources/workbookchartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a690-129">If successful, this method returns `201 Created` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a690-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9a690-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a690-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a690-131">Request</span></span>
<span data-ttu-id="9a690-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a690-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a690-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a690-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a690-134">C#</span><span class="sxs-lookup"><span data-stu-id="9a690-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a690-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a690-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a690-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9a690-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9a690-137">В тексте запроса добавьте представление объекта [воркбукчартсериес](../resources/workbookchartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a690-137">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9a690-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a690-138">Response</span></span>
<span data-ttu-id="9a690-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a690-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
