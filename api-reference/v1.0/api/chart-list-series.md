---
title: Список рядов
description: Получение списка объектов chartseries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cabc5ce6038a0a3c5ce98540afc7cc346171c13c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003821"
---
# <a name="list-series"></a><span data-ttu-id="b07da-103">Список рядов</span><span class="sxs-lookup"><span data-stu-id="b07da-103">List series</span></span>

<span data-ttu-id="b07da-104">Получение списка объектов chartseries.</span><span class="sxs-lookup"><span data-stu-id="b07da-104">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b07da-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b07da-105">Permissions</span></span>
<span data-ttu-id="b07da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b07da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b07da-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b07da-108">Permission type</span></span>      | <span data-ttu-id="b07da-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b07da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b07da-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b07da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b07da-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b07da-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b07da-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b07da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b07da-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b07da-113">Not supported.</span></span>    |
|<span data-ttu-id="b07da-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b07da-114">Application</span></span> | <span data-ttu-id="b07da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b07da-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b07da-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b07da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b07da-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b07da-117">Optional query parameters</span></span>
<span data-ttu-id="b07da-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b07da-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b07da-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b07da-119">Request headers</span></span>
| <span data-ttu-id="b07da-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b07da-120">Name</span></span>      |<span data-ttu-id="b07da-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b07da-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b07da-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b07da-122">Authorization</span></span>  | <span data-ttu-id="b07da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b07da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b07da-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b07da-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b07da-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b07da-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b07da-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b07da-128">Request body</span></span>
<span data-ttu-id="b07da-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b07da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b07da-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b07da-130">Response</span></span>

<span data-ttu-id="b07da-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукчартсериес](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b07da-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b07da-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b07da-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b07da-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b07da-133">Request</span></span>
<span data-ttu-id="b07da-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b07da-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b07da-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b07da-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_series"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b07da-136">C#</span><span class="sxs-lookup"><span data-stu-id="b07da-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-series-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b07da-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b07da-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-series-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b07da-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b07da-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-series-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b07da-139">Java</span><span class="sxs-lookup"><span data-stu-id="b07da-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-series-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b07da-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b07da-140">Response</span></span>
<span data-ttu-id="b07da-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b07da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List series",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
