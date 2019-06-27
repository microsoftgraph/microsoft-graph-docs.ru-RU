---
title: Получение объекта Chart
description: Получение свойств и связей объекта диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c00e65f794cd06a9d6e103ec95b7d73585bc631c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262043"
---
# <a name="get-workbookchart"></a><span data-ttu-id="afb13-103">Получение воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="afb13-103">Get workbookchart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afb13-104">Получение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="afb13-104">Retrieve the properties and relationships of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="afb13-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afb13-105">Permissions</span></span>
<span data-ttu-id="afb13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afb13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb13-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afb13-108">Permission type</span></span>      | <span data-ttu-id="afb13-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afb13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afb13-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afb13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afb13-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afb13-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="afb13-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afb13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb13-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afb13-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="afb13-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afb13-114">Application</span></span> | <span data-ttu-id="afb13-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afb13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afb13-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afb13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="afb13-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="afb13-117">Optional query parameters</span></span>
<span data-ttu-id="afb13-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="afb13-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afb13-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afb13-119">Request headers</span></span>
| <span data-ttu-id="afb13-120">Имя</span><span class="sxs-lookup"><span data-stu-id="afb13-120">Name</span></span>      |<span data-ttu-id="afb13-121">Описание</span><span class="sxs-lookup"><span data-stu-id="afb13-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afb13-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afb13-122">Authorization</span></span>  | <span data-ttu-id="afb13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afb13-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="afb13-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="afb13-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="afb13-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="afb13-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afb13-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="afb13-128">Request body</span></span>
<span data-ttu-id="afb13-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afb13-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afb13-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="afb13-130">Response</span></span>

<span data-ttu-id="afb13-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчарт](../resources/workbookchart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afb13-131">If successful, this method returns a `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afb13-132">Пример</span><span class="sxs-lookup"><span data-stu-id="afb13-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afb13-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="afb13-133">Request</span></span>
<span data-ttu-id="afb13-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afb13-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chart"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```
##### <a name="response"></a><span data-ttu-id="afb13-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="afb13-135">Response</span></span>
<span data-ttu-id="afb13-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afb13-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="afb13-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="afb13-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="afb13-140">C#</span><span class="sxs-lookup"><span data-stu-id="afb13-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="afb13-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="afb13-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chart-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="afb13-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="afb13-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chart-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chart-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
