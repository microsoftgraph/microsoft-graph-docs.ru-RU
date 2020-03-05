---
title: 'Table: Range'
description: Получает объект диапазона, связанный со всей таблицей.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5ae2fcf801eb163e2bbc3d1fd346ac074ff482dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452801"
---
# <a name="table-range"></a><span data-ttu-id="513cf-103">Table: Range</span><span class="sxs-lookup"><span data-stu-id="513cf-103">Table: Range</span></span>

<span data-ttu-id="513cf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="513cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="513cf-105">Получает объект диапазона, связанный со всей таблицей.</span><span class="sxs-lookup"><span data-stu-id="513cf-105">Gets the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="513cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="513cf-106">Permissions</span></span>
<span data-ttu-id="513cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="513cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="513cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="513cf-109">Permission type</span></span>      | <span data-ttu-id="513cf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="513cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="513cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="513cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="513cf-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="513cf-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="513cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="513cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="513cf-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="513cf-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="513cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="513cf-115">Application</span></span> | <span data-ttu-id="513cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="513cf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="513cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="513cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="513cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="513cf-118">Request headers</span></span>
| <span data-ttu-id="513cf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="513cf-119">Name</span></span>       | <span data-ttu-id="513cf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="513cf-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="513cf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="513cf-121">Authorization</span></span>  | <span data-ttu-id="513cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="513cf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="513cf-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="513cf-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="513cf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="513cf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="513cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="513cf-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="513cf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="513cf-128">Response</span></span>

<span data-ttu-id="513cf-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="513cf-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="513cf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="513cf-130">Example</span></span>
<span data-ttu-id="513cf-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="513cf-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="513cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="513cf-132">Request</span></span>
<span data-ttu-id="513cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="513cf-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="513cf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="513cf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/Range
```
# <a name="c"></a>[<span data-ttu-id="513cf-135">C#</span><span class="sxs-lookup"><span data-stu-id="513cf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="513cf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="513cf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="513cf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="513cf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="513cf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="513cf-138">Response</span></span>
<span data-ttu-id="513cf-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="513cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
