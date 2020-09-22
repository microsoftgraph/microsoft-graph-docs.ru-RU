---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6a4fb6cc26cc4652aa3b16b815829b9c6b7c13be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045490"
---
# <a name="table-converttorange"></a><span data-ttu-id="db8bb-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="db8bb-104">Table: convertToRange</span></span>

<span data-ttu-id="db8bb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db8bb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db8bb-p102">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="db8bb-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="db8bb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db8bb-108">Permissions</span></span>
<span data-ttu-id="db8bb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db8bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db8bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db8bb-111">Permission type</span></span>      | <span data-ttu-id="db8bb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db8bb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db8bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db8bb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db8bb-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db8bb-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db8bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db8bb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db8bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db8bb-116">Not supported.</span></span>    |
|<span data-ttu-id="db8bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db8bb-117">Application</span></span> | <span data-ttu-id="db8bb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db8bb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db8bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db8bb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="db8bb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db8bb-120">Request headers</span></span>
| <span data-ttu-id="db8bb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="db8bb-121">Name</span></span>       | <span data-ttu-id="db8bb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="db8bb-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db8bb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db8bb-123">Authorization</span></span>  | <span data-ttu-id="db8bb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db8bb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db8bb-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db8bb-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="db8bb-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="db8bb-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db8bb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db8bb-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="db8bb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="db8bb-130">Response</span></span>

<span data-ttu-id="db8bb-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db8bb-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db8bb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="db8bb-132">Example</span></span>
<span data-ttu-id="db8bb-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="db8bb-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db8bb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="db8bb-134">Request</span></span>
<span data-ttu-id="db8bb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db8bb-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db8bb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="db8bb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```
# <a name="c"></a>[<span data-ttu-id="db8bb-137">C#</span><span class="sxs-lookup"><span data-stu-id="db8bb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-converttorange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db8bb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db8bb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-converttorange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db8bb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db8bb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-converttorange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db8bb-140">Java</span><span class="sxs-lookup"><span data-stu-id="db8bb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-converttorange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db8bb-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="db8bb-141">Response</span></span>
<span data-ttu-id="db8bb-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db8bb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

