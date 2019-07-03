---
title: Получение Воркбукчартфонт
description: Получение свойств и связей объекта Воркбукчартфонт.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 587a5e1f8dcb6750d65e117e5694fd3ff37f93cf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438120"
---
# <a name="get-workbookchartfont"></a><span data-ttu-id="69264-103">Получение Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="69264-103">Get workbookChartFont</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69264-104">Получение свойств и связей объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="69264-104">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="69264-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69264-105">Permissions</span></span>
<span data-ttu-id="69264-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69264-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69264-108">Permission type</span></span>      | <span data-ttu-id="69264-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69264-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69264-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69264-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69264-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69264-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="69264-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69264-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69264-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69264-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="69264-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69264-114">Application</span></span> | <span data-ttu-id="69264-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69264-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69264-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69264-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69264-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="69264-117">Optional query parameters</span></span>
<span data-ttu-id="69264-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="69264-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69264-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69264-119">Request headers</span></span>
| <span data-ttu-id="69264-120">Имя</span><span class="sxs-lookup"><span data-stu-id="69264-120">Name</span></span>      |<span data-ttu-id="69264-121">Описание</span><span class="sxs-lookup"><span data-stu-id="69264-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="69264-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69264-122">Authorization</span></span>  | <span data-ttu-id="69264-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69264-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69264-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="69264-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="69264-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="69264-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69264-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69264-128">Request body</span></span>
<span data-ttu-id="69264-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69264-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69264-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="69264-130">Response</span></span>

<span data-ttu-id="69264-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартфонт](../resources/workbookchartfont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69264-131">If successful, this method returns a `200 OK` response code and [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69264-132">Пример</span><span class="sxs-lookup"><span data-stu-id="69264-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69264-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="69264-133">Request</span></span>
<span data-ttu-id="69264-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69264-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="69264-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="69264-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69264-136">C#</span><span class="sxs-lookup"><span data-stu-id="69264-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69264-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="69264-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69264-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="69264-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="69264-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="69264-139">Response</span></span>
<span data-ttu-id="69264-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69264-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
