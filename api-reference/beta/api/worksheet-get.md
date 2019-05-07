---
title: Получение листа
description: Получение свойств и связей объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0c6ea656be12e94b24e1ad1358fe362d9c06c0f2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636886"
---
# <a name="get-worksheet"></a><span data-ttu-id="124a3-103">Получение листа</span><span class="sxs-lookup"><span data-stu-id="124a3-103">Get Worksheet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="124a3-104">Получение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="124a3-104">Retrieve the properties and relationships of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="124a3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="124a3-105">Permissions</span></span>
<span data-ttu-id="124a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="124a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="124a3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="124a3-108">Permission type</span></span>      | <span data-ttu-id="124a3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="124a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="124a3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="124a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="124a3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="124a3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="124a3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="124a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="124a3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="124a3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="124a3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="124a3-114">Application</span></span> | <span data-ttu-id="124a3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="124a3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="124a3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="124a3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="124a3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="124a3-117">Optional query parameters</span></span>
<span data-ttu-id="124a3-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="124a3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="124a3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="124a3-119">Request headers</span></span>
| <span data-ttu-id="124a3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="124a3-120">Name</span></span>      |<span data-ttu-id="124a3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="124a3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="124a3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="124a3-122">Authorization</span></span>  | <span data-ttu-id="124a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="124a3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="124a3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="124a3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="124a3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="124a3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="124a3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="124a3-128">Request body</span></span>
<span data-ttu-id="124a3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="124a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="124a3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="124a3-130">Response</span></span>

<span data-ttu-id="124a3-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукворкшит](../resources/workbookworksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="124a3-131">If successful, this method returns a `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="124a3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="124a3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="124a3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="124a3-133">Request</span></span>
<span data-ttu-id="124a3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="124a3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheet"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
```
##### <a name="response"></a><span data-ttu-id="124a3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="124a3-135">Response</span></span>
<span data-ttu-id="124a3-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="124a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="124a3-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="124a3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="124a3-140">Языках</span><span class="sxs-lookup"><span data-stu-id="124a3-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_worksheet-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="124a3-141">Язык</span><span class="sxs-lookup"><span data-stu-id="124a3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_worksheet-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/worksheet-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
