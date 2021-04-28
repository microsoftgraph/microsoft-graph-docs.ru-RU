---
title: Список ChartSeriesCollection
description: Получение списка объектов chartseries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 43cb667ed5204f0f8afe14bc10cdb8e598f216ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054128"
---
# <a name="list-chartseriescollection"></a><span data-ttu-id="45894-103">Список ChartSeriesCollection</span><span class="sxs-lookup"><span data-stu-id="45894-103">List ChartSeriesCollection</span></span>

<span data-ttu-id="45894-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45894-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45894-105">Получение списка объектов chartseries.</span><span class="sxs-lookup"><span data-stu-id="45894-105">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="45894-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45894-106">Permissions</span></span>
<span data-ttu-id="45894-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45894-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45894-109">Permission type</span></span>      | <span data-ttu-id="45894-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45894-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45894-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45894-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45894-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45894-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45894-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45894-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45894-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45894-114">Not supported.</span></span>    |
|<span data-ttu-id="45894-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45894-115">Application</span></span> | <span data-ttu-id="45894-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45894-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45894-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45894-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="45894-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45894-118">Optional query parameters</span></span>
<span data-ttu-id="45894-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45894-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45894-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45894-120">Request headers</span></span>
| <span data-ttu-id="45894-121">Имя</span><span class="sxs-lookup"><span data-stu-id="45894-121">Name</span></span>      |<span data-ttu-id="45894-122">Описание</span><span class="sxs-lookup"><span data-stu-id="45894-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45894-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45894-123">Authorization</span></span>  | <span data-ttu-id="45894-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45894-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45894-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="45894-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="45894-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="45894-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45894-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45894-129">Request body</span></span>
<span data-ttu-id="45894-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45894-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45894-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="45894-131">Response</span></span>

<span data-ttu-id="45894-132">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [WorkbookChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45894-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45894-133">Пример</span><span class="sxs-lookup"><span data-stu-id="45894-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45894-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="45894-134">Request</span></span>
<span data-ttu-id="45894-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45894-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45894-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="45894-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartseriescollection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
```
# <a name="c"></a>[<span data-ttu-id="45894-137">C#</span><span class="sxs-lookup"><span data-stu-id="45894-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartseriescollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45894-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45894-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartseriescollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45894-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45894-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartseriescollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45894-140">Java</span><span class="sxs-lookup"><span data-stu-id="45894-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartseriescollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="45894-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="45894-141">Response</span></span>
<span data-ttu-id="45894-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45894-142">Here is an example of the response.</span></span> <span data-ttu-id="45894-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="45894-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 59

{
  "value": [
    {
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ChartSeriesCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
