---
title: Получение объекта ChartFont
description: Получение свойств и связей объекта chartfont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d8b3df5df670e02b71a1e0fff4922daec52bc0d0
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459426"
---
# <a name="get-chartfont"></a><span data-ttu-id="3720e-103">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="3720e-103">Get ChartFont</span></span>

<span data-ttu-id="3720e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3720e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3720e-105">Получение свойств и связей объекта chartfont.</span><span class="sxs-lookup"><span data-stu-id="3720e-105">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3720e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3720e-106">Permissions</span></span>
<span data-ttu-id="3720e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3720e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3720e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3720e-109">Permission type</span></span>      | <span data-ttu-id="3720e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3720e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3720e-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3720e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3720e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3720e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3720e-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3720e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3720e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3720e-114">Not supported.</span></span>    |
|<span data-ttu-id="3720e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3720e-115">Application</span></span> | <span data-ttu-id="3720e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3720e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3720e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3720e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3720e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3720e-118">Optional query parameters</span></span>
<span data-ttu-id="3720e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3720e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3720e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3720e-120">Request headers</span></span>
| <span data-ttu-id="3720e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3720e-121">Name</span></span>      |<span data-ttu-id="3720e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3720e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3720e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3720e-123">Authorization</span></span>  | <span data-ttu-id="3720e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3720e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3720e-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3720e-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="3720e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3720e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3720e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3720e-129">Request body</span></span>
<span data-ttu-id="3720e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3720e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3720e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3720e-131">Response</span></span>

<span data-ttu-id="3720e-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукчартфонт](../resources/chartfont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3720e-132">If successful, this method returns a `200 OK` response code and [WorkbookChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3720e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3720e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3720e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3720e-134">Request</span></span>
<span data-ttu-id="3720e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3720e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3720e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3720e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
```
# <a name="c"></a>[<span data-ttu-id="3720e-137">C#</span><span class="sxs-lookup"><span data-stu-id="3720e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chartfont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3720e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3720e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chartfont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3720e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3720e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chartfont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3720e-140">Java</span><span class="sxs-lookup"><span data-stu-id="3720e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chartfont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3720e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3720e-141">Response</span></span>
<span data-ttu-id="3720e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3720e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
