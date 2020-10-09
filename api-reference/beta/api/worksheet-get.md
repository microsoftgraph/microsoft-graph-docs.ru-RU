---
title: Получение листа
description: Получение свойств и связей объекта листа.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d2a9b977ef587717b02bb0f7c9f68a4bd47347a8
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405703"
---
# <a name="get-worksheet"></a><span data-ttu-id="e02d9-103">Получение листа</span><span class="sxs-lookup"><span data-stu-id="e02d9-103">Get Worksheet</span></span>

<span data-ttu-id="e02d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e02d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e02d9-105">Получение свойств и связей объекта листа.</span><span class="sxs-lookup"><span data-stu-id="e02d9-105">Retrieve the properties and relationships of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e02d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e02d9-106">Permissions</span></span>
<span data-ttu-id="e02d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e02d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e02d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e02d9-109">Permission type</span></span>      | <span data-ttu-id="e02d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e02d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e02d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e02d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e02d9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e02d9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e02d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e02d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e02d9-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e02d9-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e02d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e02d9-115">Application</span></span> | <span data-ttu-id="e02d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e02d9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e02d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e02d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e02d9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e02d9-118">Optional query parameters</span></span>
<span data-ttu-id="e02d9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e02d9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e02d9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e02d9-120">Request headers</span></span>
| <span data-ttu-id="e02d9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e02d9-121">Name</span></span>      |<span data-ttu-id="e02d9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e02d9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e02d9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e02d9-123">Authorization</span></span>  | <span data-ttu-id="e02d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e02d9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e02d9-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e02d9-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="e02d9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e02d9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e02d9-129">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="e02d9-129">Request body</span></span>
<span data-ttu-id="e02d9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e02d9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e02d9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e02d9-131">Response</span></span>

<span data-ttu-id="e02d9-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукворкшит](../resources/workbookworksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e02d9-132">If successful, this method returns a `200 OK` response code and [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e02d9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e02d9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e02d9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e02d9-134">Request</span></span>
<span data-ttu-id="e02d9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e02d9-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e02d9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e02d9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_worksheet"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="e02d9-137">C#</span><span class="sxs-lookup"><span data-stu-id="e02d9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e02d9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e02d9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e02d9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e02d9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e02d9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e02d9-140">Response</span></span>
<span data-ttu-id="e02d9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e02d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get Worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->