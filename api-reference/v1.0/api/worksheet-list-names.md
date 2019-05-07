---
title: Перечисление имен
description: 'Получение списка именованных элементов, связанных с листом. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5e089ca4898645678bcc0d6cfce5b2f394bf0f2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601864"
---
# <a name="list-names"></a><span data-ttu-id="f131d-103">Перечисление имен</span><span class="sxs-lookup"><span data-stu-id="f131d-103">List names</span></span>

<span data-ttu-id="f131d-104">Получение списка именованных элементов, связанных с листом.</span><span class="sxs-lookup"><span data-stu-id="f131d-104">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="f131d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f131d-105">Permissions</span></span>
<span data-ttu-id="f131d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f131d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f131d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f131d-108">Permission type</span></span>      | <span data-ttu-id="f131d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f131d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f131d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f131d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f131d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f131d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f131d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f131d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f131d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f131d-113">Not supported.</span></span>    |
|<span data-ttu-id="f131d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f131d-114">Application</span></span> | <span data-ttu-id="f131d-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f131d-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f131d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f131d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f131d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f131d-117">Optional query parameters</span></span>
<span data-ttu-id="f131d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f131d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f131d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f131d-119">Request headers</span></span>
| <span data-ttu-id="f131d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f131d-120">Name</span></span>      |<span data-ttu-id="f131d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f131d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f131d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f131d-122">Authorization</span></span>  | <span data-ttu-id="f131d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f131d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f131d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f131d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f131d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f131d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f131d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f131d-128">Request body</span></span>
<span data-ttu-id="f131d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f131d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f131d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f131d-130">Response</span></span>

<span data-ttu-id="f131d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукнамедитем](../resources/nameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f131d-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f131d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f131d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f131d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f131d-133">Request</span></span>
<span data-ttu-id="f131d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f131d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="f131d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f131d-135">Response</span></span>
<span data-ttu-id="f131d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f131d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f131d-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="f131d-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f131d-140">Языках</span><span class="sxs-lookup"><span data-stu-id="f131d-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tables-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f131d-141">Язык</span><span class="sxs-lookup"><span data-stu-id="f131d-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tables-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-list-names.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-list-names.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
