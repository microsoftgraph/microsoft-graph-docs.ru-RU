---
title: 'Table: DataBodyRange'
description: Получает объект диапазона, связанный с данными таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 36a7b3f625ebf5571b55465b179e2549cdea6f5d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575954"
---
# <a name="table-databodyrange"></a><span data-ttu-id="8c93f-103">Table: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="8c93f-103">Table: DataBodyRange</span></span>

<span data-ttu-id="8c93f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c93f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c93f-105">Получает объект диапазона, связанный с данными таблицы.</span><span class="sxs-lookup"><span data-stu-id="8c93f-105">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c93f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c93f-106">Permissions</span></span>
<span data-ttu-id="8c93f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c93f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c93f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c93f-109">Permission type</span></span>      | <span data-ttu-id="8c93f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c93f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c93f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c93f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c93f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c93f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8c93f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c93f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c93f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c93f-114">Not supported.</span></span>    |
|<span data-ttu-id="8c93f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c93f-115">Application</span></span> | <span data-ttu-id="8c93f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c93f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c93f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c93f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/dataBodyRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/dataBodyRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="8c93f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c93f-118">Request headers</span></span>
| <span data-ttu-id="8c93f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8c93f-119">Name</span></span>       | <span data-ttu-id="8c93f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8c93f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8c93f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c93f-121">Authorization</span></span>  | <span data-ttu-id="8c93f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c93f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c93f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8c93f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="8c93f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8c93f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c93f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c93f-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="8c93f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c93f-128">Response</span></span>

<span data-ttu-id="8c93f-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c93f-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c93f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8c93f-130">Example</span></span>
<span data-ttu-id="8c93f-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8c93f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8c93f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c93f-132">Request</span></span>
<span data-ttu-id="8c93f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c93f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c93f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c93f-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_databodyrange",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange
```
# <a name="c"></a>[<span data-ttu-id="8c93f-135">C#</span><span class="sxs-lookup"><span data-stu-id="8c93f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c93f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c93f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c93f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c93f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c93f-138">Java</span><span class="sxs-lookup"><span data-stu-id="8c93f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8c93f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c93f-139">Response</span></span>
<span data-ttu-id="8c93f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c93f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

