---
title: Получение объекта ChartAxisTitle
description: Получение свойств и связей объекта chartaxistitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4fdb946267c0ce31df211e7edfb7f1602e079ccb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518513"
---
# <a name="get-chartaxistitle"></a><span data-ttu-id="362ed-103">Получение объекта ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="362ed-103">Get ChartAxisTitle</span></span>

<span data-ttu-id="362ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="362ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="362ed-105">Получение свойств и связей объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="362ed-105">Retrieve the properties and relationships of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="362ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="362ed-106">Permissions</span></span>
<span data-ttu-id="362ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="362ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="362ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="362ed-109">Permission type</span></span>      | <span data-ttu-id="362ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="362ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="362ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="362ed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="362ed-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="362ed-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="362ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="362ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="362ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="362ed-114">Not supported.</span></span>    |
|<span data-ttu-id="362ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="362ed-115">Application</span></span> | <span data-ttu-id="362ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="362ed-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="362ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="362ed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="362ed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="362ed-118">Optional query parameters</span></span>
<span data-ttu-id="362ed-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="362ed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="362ed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="362ed-120">Request headers</span></span>
| <span data-ttu-id="362ed-121">Имя</span><span class="sxs-lookup"><span data-stu-id="362ed-121">Name</span></span>      |<span data-ttu-id="362ed-122">Описание</span><span class="sxs-lookup"><span data-stu-id="362ed-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="362ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="362ed-123">Authorization</span></span>  | <span data-ttu-id="362ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="362ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="362ed-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="362ed-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="362ed-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="362ed-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="362ed-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="362ed-129">Request body</span></span>
<span data-ttu-id="362ed-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="362ed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="362ed-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="362ed-131">Response</span></span>

<span data-ttu-id="362ed-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартаксиститле](../resources/chartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="362ed-132">If successful, this method returns a `200 OK` response code and [WorkbookChartAxisTitle](../resources/chartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="362ed-133">Пример</span><span class="sxs-lookup"><span data-stu-id="362ed-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="362ed-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="362ed-134">Request</span></span>
<span data-ttu-id="362ed-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="362ed-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="362ed-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="362ed-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title
```
# <a name="c"></a>[<span data-ttu-id="362ed-137">C#</span><span class="sxs-lookup"><span data-stu-id="362ed-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="362ed-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="362ed-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="362ed-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="362ed-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="362ed-140">Java</span><span class="sxs-lookup"><span data-stu-id="362ed-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartaxistitle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="362ed-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="362ed-141">Response</span></span>
<span data-ttu-id="362ed-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="362ed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
