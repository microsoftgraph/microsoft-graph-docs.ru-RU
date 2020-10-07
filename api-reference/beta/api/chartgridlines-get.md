---
title: Получение объекта ChartGridlines
description: Получение свойств и связей объекта chartgridlines.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4ec95b063d414f6d81d0aaf6f0141aa7bc47c114
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371939"
---
# <a name="get-chartgridlines"></a><span data-ttu-id="07afa-103">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="07afa-103">Get ChartGridlines</span></span>

<span data-ttu-id="07afa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07afa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07afa-105">Получение свойств и связей объекта chartgridlines.</span><span class="sxs-lookup"><span data-stu-id="07afa-105">Retrieve the properties and relationships of chartgridlines object.</span></span>
## <a name="permissions"></a><span data-ttu-id="07afa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07afa-106">Permissions</span></span>
<span data-ttu-id="07afa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07afa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07afa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07afa-109">Permission type</span></span>      | <span data-ttu-id="07afa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07afa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07afa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07afa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="07afa-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07afa-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07afa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07afa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07afa-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07afa-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="07afa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07afa-115">Application</span></span> | <span data-ttu-id="07afa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07afa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07afa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07afa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/majorgridlines
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07afa-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07afa-118">Optional query parameters</span></span>
<span data-ttu-id="07afa-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07afa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07afa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07afa-120">Request headers</span></span>
| <span data-ttu-id="07afa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="07afa-121">Name</span></span>      |<span data-ttu-id="07afa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="07afa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07afa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07afa-123">Authorization</span></span>  | <span data-ttu-id="07afa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07afa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07afa-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="07afa-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="07afa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="07afa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07afa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07afa-129">Request body</span></span>
<span data-ttu-id="07afa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07afa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07afa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="07afa-131">Response</span></span>

<span data-ttu-id="07afa-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартгридлинес](../resources/workbookchartgridlines.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07afa-132">If successful, this method returns a `200 OK` response code and [workbookChartGridlines](../resources/workbookchartgridlines.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07afa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="07afa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07afa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="07afa-134">Request</span></span>
<span data-ttu-id="07afa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07afa-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07afa-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="07afa-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartgridlines"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines
```
# <a name="c"></a>[<span data-ttu-id="07afa-137">C#</span><span class="sxs-lookup"><span data-stu-id="07afa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartgridlines-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07afa-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07afa-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartgridlines-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07afa-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07afa-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartgridlines-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07afa-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="07afa-140">Response</span></span>
<span data-ttu-id="07afa-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07afa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartGridlines"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartGridlines",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
