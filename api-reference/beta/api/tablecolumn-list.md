---
title: Список TableColumnCollection
description: Получение списка объектов tablecolumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 80953df1c52aec9d49082e8adbe9de38bb16b9f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451733"
---
# <a name="list-tablecolumncollection"></a><span data-ttu-id="bfe19-103">Список TableColumnCollection</span><span class="sxs-lookup"><span data-stu-id="bfe19-103">List TableColumnCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfe19-104">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="bfe19-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfe19-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfe19-105">Permissions</span></span>
<span data-ttu-id="bfe19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfe19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfe19-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfe19-108">Permission type</span></span>      | <span data-ttu-id="bfe19-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfe19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfe19-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfe19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfe19-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfe19-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfe19-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfe19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfe19-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfe19-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfe19-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfe19-114">Application</span></span> | <span data-ttu-id="bfe19-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfe19-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfe19-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfe19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfe19-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bfe19-117">Optional query parameters</span></span>
<span data-ttu-id="bfe19-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bfe19-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfe19-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfe19-119">Request headers</span></span>
| <span data-ttu-id="bfe19-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bfe19-120">Name</span></span>      |<span data-ttu-id="bfe19-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bfe19-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfe19-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfe19-122">Authorization</span></span>  | <span data-ttu-id="bfe19-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfe19-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfe19-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bfe19-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bfe19-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bfe19-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfe19-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bfe19-128">Request body</span></span>
<span data-ttu-id="bfe19-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfe19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfe19-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfe19-130">Response</span></span>

<span data-ttu-id="bfe19-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуктаблеколумн](../resources/workbooktablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfe19-131">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfe19-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bfe19-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfe19-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfe19-133">Request</span></span>
<span data-ttu-id="bfe19-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfe19-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bfe19-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfe19-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bfe19-136">C#</span><span class="sxs-lookup"><span data-stu-id="bfe19-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablecolumncollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfe19-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="bfe19-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablecolumncollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bfe19-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bfe19-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablecolumncollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bfe19-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfe19-139">Response</span></span>
<span data-ttu-id="bfe19-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfe19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
