---
title: Получение списка pivotTables
description: Получение списка объектов workbookpivottable.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c9240c83d509d947cf73187e1e03107ef44e1b64
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578824"
---
# <a name="list-pivottables"></a><span data-ttu-id="85c58-103">Получение списка pivotTables</span><span class="sxs-lookup"><span data-stu-id="85c58-103">List pivotTables</span></span>

<span data-ttu-id="85c58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85c58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85c58-105">Получение списка объектов workbookpivottable.</span><span class="sxs-lookup"><span data-stu-id="85c58-105">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="85c58-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85c58-106">Permissions</span></span>
<span data-ttu-id="85c58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85c58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="85c58-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85c58-109">Permission type</span></span>      | <span data-ttu-id="85c58-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85c58-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85c58-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85c58-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85c58-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85c58-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85c58-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85c58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85c58-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85c58-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="85c58-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85c58-115">Application</span></span> | <span data-ttu-id="85c58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85c58-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85c58-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85c58-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/pivotTables
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85c58-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85c58-118">Optional query parameters</span></span>
<span data-ttu-id="85c58-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85c58-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85c58-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85c58-120">Request headers</span></span>
| <span data-ttu-id="85c58-121">Имя</span><span class="sxs-lookup"><span data-stu-id="85c58-121">Name</span></span>      |<span data-ttu-id="85c58-122">Описание</span><span class="sxs-lookup"><span data-stu-id="85c58-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85c58-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85c58-123">Authorization</span></span>  | <span data-ttu-id="85c58-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85c58-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85c58-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="85c58-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="85c58-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="85c58-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85c58-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85c58-129">Request body</span></span>
<span data-ttu-id="85c58-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85c58-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85c58-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="85c58-131">Response</span></span>

<span data-ttu-id="85c58-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85c58-132">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85c58-133">Пример</span><span class="sxs-lookup"><span data-stu-id="85c58-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85c58-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="85c58-134">Request</span></span>
<span data-ttu-id="85c58-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85c58-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85c58-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="85c58-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables
```
# <a name="c"></a>[<span data-ttu-id="85c58-137">C#</span><span class="sxs-lookup"><span data-stu-id="85c58-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-pivottables-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85c58-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85c58-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-pivottables-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85c58-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85c58-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-pivottables-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85c58-140">Java</span><span class="sxs-lookup"><span data-stu-id="85c58-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-pivottables-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85c58-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="85c58-141">Response</span></span>
<span data-ttu-id="85c58-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85c58-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
