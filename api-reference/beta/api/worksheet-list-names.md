---
title: Перечисление имен
description: 'Получение списка именованных элементов, связанных с листом. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 1fb9641f783e3297ac4481d211fd0eb4905fcb37
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406186"
---
# <a name="list-names"></a><span data-ttu-id="70a70-103">Перечисление имен</span><span class="sxs-lookup"><span data-stu-id="70a70-103">List names</span></span>

<span data-ttu-id="70a70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70a70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70a70-105">Получение списка именованных элементов, связанных с листом.</span><span class="sxs-lookup"><span data-stu-id="70a70-105">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="70a70-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70a70-106">Permissions</span></span>
<span data-ttu-id="70a70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70a70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70a70-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70a70-109">Permission type</span></span>      | <span data-ttu-id="70a70-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70a70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70a70-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70a70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70a70-112">Files. Read, Files. ReadWrite, sites. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="70a70-112">Files.Read, Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="70a70-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70a70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70a70-114">Files. Read, Files. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70a70-114">Files.Read, Files.ReadWrite</span></span>    |
|<span data-ttu-id="70a70-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70a70-115">Application</span></span> | <span data-ttu-id="70a70-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="70a70-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70a70-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70a70-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70a70-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70a70-118">Optional query parameters</span></span>
<span data-ttu-id="70a70-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70a70-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70a70-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70a70-120">Request headers</span></span>
| <span data-ttu-id="70a70-121">Имя</span><span class="sxs-lookup"><span data-stu-id="70a70-121">Name</span></span>      |<span data-ttu-id="70a70-122">Описание</span><span class="sxs-lookup"><span data-stu-id="70a70-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70a70-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70a70-123">Authorization</span></span>  | <span data-ttu-id="70a70-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70a70-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70a70-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="70a70-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="70a70-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="70a70-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70a70-129">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="70a70-129">Request body</span></span>
<span data-ttu-id="70a70-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70a70-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70a70-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a70-131">Response</span></span>

<span data-ttu-id="70a70-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукнамедитем](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70a70-132">If successful, this method returns a `200 OK` response code and collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70a70-133">Пример</span><span class="sxs-lookup"><span data-stu-id="70a70-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70a70-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="70a70-134">Request</span></span>
<span data-ttu-id="70a70-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70a70-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70a70-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="70a70-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
# <a name="c"></a>[<span data-ttu-id="70a70-137">C#</span><span class="sxs-lookup"><span data-stu-id="70a70-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tables-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70a70-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70a70-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tables-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70a70-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70a70-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tables-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70a70-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a70-140">Response</span></span>
<span data-ttu-id="70a70-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70a70-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->