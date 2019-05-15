---
title: Получение workbookPivotTable
description: Получение свойств и связей объекта workbookPivotTable.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 059f4898aa7d5503b141a675b255907d0a2f689f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961161"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="9414e-103">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="9414e-103">Get workbookPivotTable</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9414e-104">Получение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="9414e-104">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9414e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9414e-105">Permissions</span></span>
<span data-ttu-id="9414e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9414e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9414e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9414e-108">Permission type</span></span>      | <span data-ttu-id="9414e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9414e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9414e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9414e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9414e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9414e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9414e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9414e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9414e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9414e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9414e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9414e-114">Application</span></span> | <span data-ttu-id="9414e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9414e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9414e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9414e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9414e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9414e-117">Optional query parameters</span></span>
<span data-ttu-id="9414e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9414e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9414e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9414e-119">Request headers</span></span>
| <span data-ttu-id="9414e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9414e-120">Name</span></span>      |<span data-ttu-id="9414e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9414e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9414e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9414e-122">Authorization</span></span>  | <span data-ttu-id="9414e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9414e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9414e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9414e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9414e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9414e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9414e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9414e-128">Request body</span></span>
<span data-ttu-id="9414e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9414e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9414e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9414e-130">Response</span></span>

<span data-ttu-id="9414e-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9414e-131">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9414e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9414e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9414e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9414e-133">Request</span></span>
<span data-ttu-id="9414e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9414e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="9414e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9414e-135">Response</span></span>
<span data-ttu-id="9414e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9414e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9414e-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="9414e-139">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9414e-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="9414e-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_workbookpivottable-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="9414e-141">C#</span><span class="sxs-lookup"><span data-stu-id="9414e-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_workbookpivottable-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookpivottable-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookpivottable-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
