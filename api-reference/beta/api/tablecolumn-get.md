---
title: Получение объекта TableColumn
description: Получение свойств и связей объекта tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8273f47ec600b15a89860e5610896819df4569b9
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034102"
---
# <a name="get-tablecolumn"></a><span data-ttu-id="16178-103">Получение объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="16178-103">Get TableColumn</span></span>

<span data-ttu-id="16178-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16178-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16178-105">Получение свойств и связей объекта tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="16178-105">Retrieve the properties and relationships of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="16178-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16178-106">Permissions</span></span>
<span data-ttu-id="16178-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16178-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16178-109">Permission type</span></span>      | <span data-ttu-id="16178-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16178-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16178-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16178-111">Delegated (work or school account)</span></span> | <span data-ttu-id="16178-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16178-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16178-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16178-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16178-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16178-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="16178-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16178-115">Application</span></span> | <span data-ttu-id="16178-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16178-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16178-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16178-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16178-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16178-118">Optional query parameters</span></span>
<span data-ttu-id="16178-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16178-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16178-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16178-120">Request headers</span></span>
| <span data-ttu-id="16178-121">Имя</span><span class="sxs-lookup"><span data-stu-id="16178-121">Name</span></span>      |<span data-ttu-id="16178-122">Описание</span><span class="sxs-lookup"><span data-stu-id="16178-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16178-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16178-123">Authorization</span></span>  | <span data-ttu-id="16178-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16178-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="16178-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="16178-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="16178-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="16178-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16178-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16178-129">Request body</span></span>
<span data-ttu-id="16178-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16178-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16178-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="16178-131">Response</span></span>

<span data-ttu-id="16178-132">В случае успеха этот метод возвращает код отклика и объект `200 OK` [workbookTableColumn](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16178-132">If successful, this method returns a `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16178-133">Пример</span><span class="sxs-lookup"><span data-stu-id="16178-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16178-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="16178-134">Request</span></span>
<span data-ttu-id="16178-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16178-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16178-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="16178-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="16178-137">C#</span><span class="sxs-lookup"><span data-stu-id="16178-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16178-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16178-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16178-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16178-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16178-140">Java</span><span class="sxs-lookup"><span data-stu-id="16178-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16178-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="16178-141">Response</span></span>
<span data-ttu-id="16178-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16178-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "99",
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
