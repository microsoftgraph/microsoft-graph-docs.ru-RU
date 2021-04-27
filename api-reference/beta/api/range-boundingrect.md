---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bf548c798a6539a0be25b78481ee2da6e90614cd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055150"
---
# <a name="range-boundingrect"></a><span data-ttu-id="cbfe7-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="cbfe7-103">Range: BoundingRect</span></span>

<span data-ttu-id="cbfe7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbfe7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbfe7-p101">Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="cbfe7-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="cbfe7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbfe7-107">Permissions</span></span>
<span data-ttu-id="cbfe7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbfe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbfe7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbfe7-110">Permission type</span></span>      | <span data-ttu-id="cbfe7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbfe7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbfe7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbfe7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cbfe7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbfe7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbfe7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbfe7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbfe7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbfe7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cbfe7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbfe7-116">Application</span></span> | <span data-ttu-id="cbfe7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbfe7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbfe7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/BoundingRect
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/BoundingRect
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="cbfe7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbfe7-119">Request headers</span></span>
| <span data-ttu-id="cbfe7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cbfe7-120">Name</span></span>       | <span data-ttu-id="cbfe7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cbfe7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cbfe7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbfe7-122">Authorization</span></span>  | <span data-ttu-id="cbfe7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbfe7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cbfe7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cbfe7-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbfe7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbfe7-128">Request body</span></span>
<span data-ttu-id="cbfe7-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cbfe7-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="cbfe7-130">Parameter</span></span>    | <span data-ttu-id="cbfe7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cbfe7-131">Type</span></span>   |<span data-ttu-id="cbfe7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cbfe7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbfe7-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="cbfe7-133">anotherRange</span></span>|<span data-ttu-id="cbfe7-134">string</span><span class="sxs-lookup"><span data-stu-id="cbfe7-134">string</span></span>|<span data-ttu-id="cbfe7-135">Объект, адрес или имя диапазона.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-135">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="cbfe7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbfe7-136">Response</span></span>

<span data-ttu-id="cbfe7-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbfe7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cbfe7-138">Example</span></span>
<span data-ttu-id="cbfe7-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cbfe7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbfe7-140">Request</span></span>
<span data-ttu-id="cbfe7-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="cbfe7-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbfe7-142">Response</span></span>
<span data-ttu-id="cbfe7-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-143">Here is an example of the response.</span></span> <span data-ttu-id="cbfe7-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cbfe7-144">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


