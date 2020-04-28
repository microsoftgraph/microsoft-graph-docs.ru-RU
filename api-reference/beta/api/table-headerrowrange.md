---
title: 'Table: HeaderRowRange'
description: Получает объект диапазона, связанный со строкой заголовков таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fd9f4ad37aa7048c2449751834b506a7d8de8954
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452842"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="c5afb-103">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="c5afb-103">Table: HeaderRowRange</span></span>

<span data-ttu-id="c5afb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5afb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5afb-105">Получает объект диапазона, связанный со строкой заголовков таблицы.</span><span class="sxs-lookup"><span data-stu-id="c5afb-105">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5afb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5afb-106">Permissions</span></span>
<span data-ttu-id="c5afb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5afb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5afb-109">Permission type</span></span>      | <span data-ttu-id="c5afb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5afb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5afb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5afb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5afb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5afb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5afb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5afb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5afb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5afb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5afb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5afb-115">Application</span></span> | <span data-ttu-id="c5afb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5afb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5afb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5afb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="c5afb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5afb-118">Request headers</span></span>
| <span data-ttu-id="c5afb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c5afb-119">Name</span></span>       | <span data-ttu-id="c5afb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c5afb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5afb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5afb-121">Authorization</span></span>  | <span data-ttu-id="c5afb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5afb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5afb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5afb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5afb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c5afb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5afb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5afb-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c5afb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5afb-128">Response</span></span>

<span data-ttu-id="c5afb-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c5afb-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5afb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c5afb-130">Example</span></span>
<span data-ttu-id="c5afb-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c5afb-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5afb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5afb-132">Request</span></span>
<span data-ttu-id="c5afb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5afb-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5afb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5afb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```
# <a name="c"></a>[<span data-ttu-id="c5afb-135">C#</span><span class="sxs-lookup"><span data-stu-id="c5afb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5afb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5afb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5afb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5afb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c5afb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5afb-138">Response</span></span>
<span data-ttu-id="c5afb-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5afb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
