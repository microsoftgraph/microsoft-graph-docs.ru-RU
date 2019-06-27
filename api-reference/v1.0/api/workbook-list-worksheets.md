---
title: Список листов
description: Получение списка объектов листов.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eb40821a8295834dd080f8a98d8f9889a4564819
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278570"
---
# <a name="list-worksheets"></a><span data-ttu-id="446e0-103">Список листов</span><span class="sxs-lookup"><span data-stu-id="446e0-103">List worksheets</span></span>

<span data-ttu-id="446e0-104">Получение списка объектов листов.</span><span class="sxs-lookup"><span data-stu-id="446e0-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="446e0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="446e0-105">Permissions</span></span>
<span data-ttu-id="446e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="446e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="446e0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="446e0-108">Permission type</span></span>      | <span data-ttu-id="446e0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="446e0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="446e0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="446e0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="446e0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="446e0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="446e0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="446e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="446e0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="446e0-113">Not supported.</span></span>    |
|<span data-ttu-id="446e0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="446e0-114">Application</span></span> | <span data-ttu-id="446e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="446e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="446e0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="446e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="446e0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="446e0-117">Optional query parameters</span></span>
<span data-ttu-id="446e0-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="446e0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="446e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="446e0-119">Request headers</span></span>
| <span data-ttu-id="446e0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="446e0-120">Name</span></span>      |<span data-ttu-id="446e0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="446e0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="446e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="446e0-122">Authorization</span></span>  | <span data-ttu-id="446e0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="446e0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="446e0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="446e0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="446e0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="446e0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="446e0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="446e0-128">Request body</span></span>
<span data-ttu-id="446e0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="446e0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="446e0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="446e0-130">Response</span></span>

<span data-ttu-id="446e0-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукворкшит](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="446e0-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookWorksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="446e0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="446e0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="446e0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="446e0-133">Request</span></span>
<span data-ttu-id="446e0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="446e0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheets"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="446e0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="446e0-135">Response</span></span>
<span data-ttu-id="446e0-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="446e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="446e0-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="446e0-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="446e0-140">C#</span><span class="sxs-lookup"><span data-stu-id="446e0-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_worksheets-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="446e0-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="446e0-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_worksheets-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="446e0-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="446e0-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_worksheets-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List worksheets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbook-list-worksheets.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbook-list-worksheets.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbook-list-worksheets.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
