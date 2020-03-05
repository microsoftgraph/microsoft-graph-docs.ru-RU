---
title: Получение объекта TableSort
description: Получение свойств и связей объекта tablesort.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2031b5f75adb7563ac546f2fac69d167f92f945f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452633"
---
# <a name="get-tablesort"></a><span data-ttu-id="ea347-103">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="ea347-103">Get TableSort</span></span>

<span data-ttu-id="ea347-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ea347-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea347-105">Получение свойств и связей объекта tablesort.</span><span class="sxs-lookup"><span data-stu-id="ea347-105">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea347-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea347-106">Permissions</span></span>
<span data-ttu-id="ea347-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea347-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea347-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea347-109">Permission type</span></span>      | <span data-ttu-id="ea347-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea347-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea347-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea347-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea347-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea347-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea347-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea347-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea347-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea347-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea347-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea347-115">Application</span></span> | <span data-ttu-id="ea347-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea347-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea347-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea347-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea347-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea347-118">Optional query parameters</span></span>
<span data-ttu-id="ea347-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea347-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea347-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea347-120">Request headers</span></span>
| <span data-ttu-id="ea347-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ea347-121">Name</span></span>      |<span data-ttu-id="ea347-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ea347-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea347-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea347-123">Authorization</span></span>  | <span data-ttu-id="ea347-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea347-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea347-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ea347-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="ea347-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ea347-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea347-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea347-129">Request body</span></span>
<span data-ttu-id="ea347-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea347-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea347-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea347-131">Response</span></span>

<span data-ttu-id="ea347-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбуктаблесорт](../resources/workbooktablesort.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea347-132">If successful, this method returns a `200 OK` response code and [workbookTableSort](../resources/workbooktablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea347-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ea347-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea347-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea347-134">Request</span></span>
<span data-ttu-id="ea347-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea347-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea347-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea347-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
# <a name="c"></a>[<span data-ttu-id="ea347-137">C#</span><span class="sxs-lookup"><span data-stu-id="ea347-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablesort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea347-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea347-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablesort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea347-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea347-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablesort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ea347-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea347-140">Response</span></span>
<span data-ttu-id="ea347-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea347-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableSort"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "matchCase": true,
  "method": "method-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableSort",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
