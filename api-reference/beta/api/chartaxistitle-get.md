---
title: Получение Воркбукчартаксиститле
description: Получение свойств и связей объекта воркбукчартаксиститле.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 259a072b0daadd56c67e298510e6fc701c368f28
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418549"
---
# <a name="get-workbookchartaxistitle"></a><span data-ttu-id="dc9df-103">Получение Воркбукчартаксиститле</span><span class="sxs-lookup"><span data-stu-id="dc9df-103">Get workbookChartAxisTitle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc9df-104">Получение свойств и связей объекта chartaxistitle.</span><span class="sxs-lookup"><span data-stu-id="dc9df-104">Retrieve the properties and relationships of chartaxistitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc9df-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc9df-105">Permissions</span></span>
<span data-ttu-id="dc9df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc9df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc9df-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc9df-108">Permission type</span></span>      | <span data-ttu-id="dc9df-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc9df-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc9df-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc9df-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc9df-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc9df-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc9df-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc9df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc9df-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc9df-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc9df-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc9df-114">Application</span></span> | <span data-ttu-id="dc9df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc9df-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc9df-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc9df-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/title
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/title
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc9df-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc9df-117">Optional query parameters</span></span>
<span data-ttu-id="dc9df-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dc9df-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc9df-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc9df-119">Request headers</span></span>
| <span data-ttu-id="dc9df-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dc9df-120">Name</span></span>      |<span data-ttu-id="dc9df-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dc9df-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dc9df-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc9df-122">Authorization</span></span>  | <span data-ttu-id="dc9df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc9df-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc9df-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc9df-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc9df-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc9df-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc9df-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc9df-128">Request body</span></span>
<span data-ttu-id="dc9df-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc9df-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc9df-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc9df-130">Response</span></span>

<span data-ttu-id="dc9df-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартаксиститле](../resources/workbookchartaxistitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc9df-131">If successful, this method returns a `200 OK` response code and [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc9df-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dc9df-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc9df-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc9df-133">Request</span></span>
<span data-ttu-id="dc9df-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc9df-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc9df-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc9df-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartaxistitle"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc9df-136">C#</span><span class="sxs-lookup"><span data-stu-id="dc9df-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartaxistitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc9df-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc9df-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartaxistitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc9df-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dc9df-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartaxistitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc9df-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc9df-139">Response</span></span>
<span data-ttu-id="dc9df-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc9df-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartAxisTitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
