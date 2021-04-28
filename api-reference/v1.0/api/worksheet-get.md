---
title: Получение листа
description: Получение свойств и связей объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 90d4c306fe4db5c21f43a77b29181aa8a9611175
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049347"
---
# <a name="get-worksheet"></a><span data-ttu-id="be4c3-103">Получение листа</span><span class="sxs-lookup"><span data-stu-id="be4c3-103">Get Worksheet</span></span>

<span data-ttu-id="be4c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be4c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be4c3-105">Получение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="be4c3-105">Retrieve the properties and relationships of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be4c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be4c3-106">Permissions</span></span>
<span data-ttu-id="be4c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be4c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be4c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be4c3-109">Permission type</span></span>      | <span data-ttu-id="be4c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be4c3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be4c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be4c3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="be4c3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be4c3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be4c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be4c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be4c3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be4c3-114">Not supported.</span></span>    |
|<span data-ttu-id="be4c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be4c3-115">Application</span></span> | <span data-ttu-id="be4c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be4c3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be4c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be4c3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be4c3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be4c3-118">Optional query parameters</span></span>
<span data-ttu-id="be4c3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be4c3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be4c3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be4c3-120">Request headers</span></span>
| <span data-ttu-id="be4c3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="be4c3-121">Name</span></span>      |<span data-ttu-id="be4c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="be4c3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be4c3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be4c3-123">Authorization</span></span>  | <span data-ttu-id="be4c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be4c3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be4c3-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be4c3-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="be4c3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="be4c3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be4c3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be4c3-129">Request body</span></span>
<span data-ttu-id="be4c3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be4c3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be4c3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="be4c3-131">Response</span></span>

<span data-ttu-id="be4c3-132">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [WorkbookWorksheet](../resources/worksheet.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="be4c3-132">If successful, this method returns a `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be4c3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="be4c3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be4c3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="be4c3-134">Request</span></span>
<span data-ttu-id="be4c3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be4c3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be4c3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="be4c3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheet"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="be4c3-137">C#</span><span class="sxs-lookup"><span data-stu-id="be4c3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be4c3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be4c3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be4c3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be4c3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be4c3-140">Java</span><span class="sxs-lookup"><span data-stu-id="be4c3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="be4c3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="be4c3-141">Response</span></span>
<span data-ttu-id="be4c3-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be4c3-142">Here is an example of the response.</span></span> <span data-ttu-id="be4c3-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="be4c3-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
