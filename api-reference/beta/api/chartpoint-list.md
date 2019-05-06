---
title: Список ChartPointsCollection
description: Получение списка объектов chartpoint.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 923d549ef485d2e0c1965d7bc8ac651cad12289c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592054"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="dfa40-103">Список ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="dfa40-103">List ChartPointsCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa40-104">Получение списка объектов chartpoint.</span><span class="sxs-lookup"><span data-stu-id="dfa40-104">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="dfa40-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa40-105">Permissions</span></span>
<span data-ttu-id="dfa40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa40-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa40-108">Permission type</span></span>      | <span data-ttu-id="dfa40-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfa40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfa40-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfa40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dfa40-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfa40-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dfa40-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfa40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa40-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfa40-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dfa40-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfa40-114">Application</span></span> | <span data-ttu-id="dfa40-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa40-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfa40-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfa40-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dfa40-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfa40-117">Optional query parameters</span></span>
<span data-ttu-id="dfa40-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfa40-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfa40-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfa40-119">Request headers</span></span>
| <span data-ttu-id="dfa40-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dfa40-120">Name</span></span>      |<span data-ttu-id="dfa40-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa40-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfa40-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfa40-122">Authorization</span></span>  | <span data-ttu-id="dfa40-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa40-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfa40-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dfa40-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dfa40-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dfa40-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfa40-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfa40-128">Request body</span></span>
<span data-ttu-id="dfa40-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfa40-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfa40-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfa40-130">Response</span></span>

<span data-ttu-id="dfa40-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукчартпоинт](../resources/workbookchartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa40-131">If successful, this method returns a `200 OK` response code and collection of [workbookChartPoint](../resources/workbookchartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfa40-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dfa40-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfa40-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa40-133">Request</span></span>
<span data-ttu-id="dfa40-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa40-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
```
##### <a name="response"></a><span data-ttu-id="dfa40-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa40-135">Response</span></span>
<span data-ttu-id="dfa40-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfa40-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 57

{
  "value": [
    {
      "value": {
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfa40-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="dfa40-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfa40-140">Языках</span><span class="sxs-lookup"><span data-stu-id="dfa40-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chartpointscollection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfa40-141">Язык</span><span class="sxs-lookup"><span data-stu-id="dfa40-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chartpointscollection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartpoint-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartpoint-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
