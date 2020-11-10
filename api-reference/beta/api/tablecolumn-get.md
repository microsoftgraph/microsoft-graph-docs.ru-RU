---
title: Получение объекта TableColumn
description: Получение свойств и связей объекта tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 08cb486afd9d8791d7921de7cc90e570c4193872
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980360"
---
# <a name="get-tablecolumn"></a><span data-ttu-id="b0d55-103">Получение объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="b0d55-103">Get TableColumn</span></span>

<span data-ttu-id="b0d55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0d55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0d55-105">Получение свойств и связей объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="b0d55-105">Retrieve the properties and relationships of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0d55-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0d55-106">Permissions</span></span>
<span data-ttu-id="b0d55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0d55-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0d55-109">Permission type</span></span>      | <span data-ttu-id="b0d55-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0d55-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0d55-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0d55-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0d55-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0d55-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0d55-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0d55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0d55-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0d55-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0d55-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0d55-115">Application</span></span> | <span data-ttu-id="b0d55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0d55-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0d55-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0d55-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0d55-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0d55-118">Optional query parameters</span></span>
<span data-ttu-id="b0d55-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0d55-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0d55-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0d55-120">Request headers</span></span>
| <span data-ttu-id="b0d55-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b0d55-121">Name</span></span>      |<span data-ttu-id="b0d55-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0d55-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0d55-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0d55-123">Authorization</span></span>  | <span data-ttu-id="b0d55-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0d55-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0d55-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b0d55-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="b0d55-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b0d55-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0d55-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0d55-129">Request body</span></span>
<span data-ttu-id="b0d55-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0d55-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0d55-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0d55-131">Response</span></span>

<span data-ttu-id="b0d55-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0d55-132">If successful, this method returns a `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0d55-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b0d55-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0d55-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0d55-134">Request</span></span>
<span data-ttu-id="b0d55-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0d55-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0d55-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0d55-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="b0d55-137">C#</span><span class="sxs-lookup"><span data-stu-id="b0d55-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0d55-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0d55-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0d55-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0d55-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0d55-140">Java</span><span class="sxs-lookup"><span data-stu-id="b0d55-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0d55-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0d55-141">Response</span></span>
<span data-ttu-id="b0d55-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0d55-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
