---
title: Получение объекта RangeFont
description: Получение свойств и связей объекта rangefont.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e83019af805a71ad0a75431a518a260a2880594f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978715"
---
# <a name="get-rangefont"></a><span data-ttu-id="4bd62-103">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="4bd62-103">Get RangeFont</span></span>

<span data-ttu-id="4bd62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bd62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4bd62-105">Получение свойств и связей объекта rangefont.</span><span class="sxs-lookup"><span data-stu-id="4bd62-105">Retrieve the properties and relationships of rangefont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bd62-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4bd62-106">Permissions</span></span>
<span data-ttu-id="4bd62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bd62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bd62-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bd62-109">Permission type</span></span>      | <span data-ttu-id="4bd62-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bd62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bd62-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bd62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4bd62-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bd62-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4bd62-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bd62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd62-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bd62-114">Not supported.</span></span>    |
|<span data-ttu-id="4bd62-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bd62-115">Application</span></span> | <span data-ttu-id="4bd62-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bd62-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bd62-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bd62-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/font
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/font
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4bd62-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4bd62-118">Optional query parameters</span></span>
<span data-ttu-id="4bd62-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4bd62-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bd62-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bd62-120">Request headers</span></span>
| <span data-ttu-id="4bd62-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4bd62-121">Name</span></span>      |<span data-ttu-id="4bd62-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4bd62-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4bd62-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bd62-123">Authorization</span></span>  | <span data-ttu-id="4bd62-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bd62-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bd62-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4bd62-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="4bd62-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4bd62-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bd62-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bd62-129">Request body</span></span>
<span data-ttu-id="4bd62-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bd62-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bd62-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bd62-131">Response</span></span>

<span data-ttu-id="4bd62-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукранжефонт](../resources/rangefont.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4bd62-132">If successful, this method returns a `200 OK` response code and [WorkbookRangeFont](../resources/rangefont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bd62-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4bd62-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bd62-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bd62-134">Request</span></span>
<span data-ttu-id="4bd62-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bd62-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4bd62-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bd62-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rangefont"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/font
```
# <a name="c"></a>[<span data-ttu-id="4bd62-137">C#</span><span class="sxs-lookup"><span data-stu-id="4bd62-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rangefont-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bd62-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bd62-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rangefont-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bd62-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bd62-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rangefont-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4bd62-140">Java</span><span class="sxs-lookup"><span data-stu-id="4bd62-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rangefont-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4bd62-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bd62-141">Response</span></span>
<span data-ttu-id="4bd62-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bd62-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "description": "Get RangeFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

