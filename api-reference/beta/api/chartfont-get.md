---
title: Получение Воркбукчартфонт
description: Получение свойств и связей объекта Воркбукчартфонт.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c882a469123d2db0289375ca494ed4e4ca446762
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958731"
---
# <a name="get-workbookchartfont"></a><span data-ttu-id="c6ca2-103">Получение Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="c6ca2-103">Get workbookChartFont</span></span>

<span data-ttu-id="c6ca2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6ca2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6ca2-105">Получение свойств и связей объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-105">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6ca2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ca2-106">Permissions</span></span>
<span data-ttu-id="c6ca2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6ca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6ca2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ca2-109">Permission type</span></span>      | <span data-ttu-id="c6ca2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6ca2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6ca2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6ca2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6ca2-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6ca2-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6ca2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6ca2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6ca2-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6ca2-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c6ca2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6ca2-115">Application</span></span> | <span data-ttu-id="c6ca2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6ca2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6ca2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6ca2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c6ca2-118">Optional query parameters</span></span>
<span data-ttu-id="c6ca2-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6ca2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6ca2-120">Request headers</span></span>
| <span data-ttu-id="c6ca2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c6ca2-121">Name</span></span>      |<span data-ttu-id="c6ca2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ca2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6ca2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6ca2-123">Authorization</span></span>  | <span data-ttu-id="c6ca2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6ca2-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c6ca2-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="c6ca2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6ca2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6ca2-129">Request body</span></span>
<span data-ttu-id="c6ca2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6ca2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ca2-131">Response</span></span>

<span data-ttu-id="c6ca2-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартфонт](../resources/workbookchartfont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-132">If successful, this method returns a `200 OK` response code and [workbookChartFont](../resources/workbookchartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6ca2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c6ca2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6ca2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6ca2-134">Request</span></span>
<span data-ttu-id="c6ca2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6ca2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6ca2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font
```
# <a name="c"></a>[<span data-ttu-id="c6ca2-137">C#</span><span class="sxs-lookup"><span data-stu-id="c6ca2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6ca2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6ca2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6ca2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6ca2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6ca2-140">Java</span><span class="sxs-lookup"><span data-stu-id="c6ca2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c6ca2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ca2-141">Response</span></span>
<span data-ttu-id="c6ca2-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6ca2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
