---
title: 'Range: Row'
description: Возвращает строку из диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 24c9aa530afd08742f62be07f3639358fd7f052f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055801"
---
# <a name="range-row"></a><span data-ttu-id="e65e1-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="e65e1-103">Range: Row</span></span>

<span data-ttu-id="e65e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e65e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e65e1-105">Возвращает строку из диапазона.</span><span class="sxs-lookup"><span data-stu-id="e65e1-105">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e65e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e65e1-106">Permissions</span></span>
<span data-ttu-id="e65e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e65e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e65e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e65e1-109">Permission type</span></span>      | <span data-ttu-id="e65e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e65e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e65e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e65e1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e65e1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e65e1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e65e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e65e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e65e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e65e1-114">Not supported.</span></span>    |
|<span data-ttu-id="e65e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e65e1-115">Application</span></span> | <span data-ttu-id="e65e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e65e1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e65e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e65e1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/row
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/row
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/row
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/row
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/row
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/row

```
## <a name="request-headers"></a><span data-ttu-id="e65e1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e65e1-118">Request headers</span></span>
| <span data-ttu-id="e65e1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e65e1-119">Name</span></span>       | <span data-ttu-id="e65e1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e65e1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e65e1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e65e1-121">Authorization</span></span>  | <span data-ttu-id="e65e1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e65e1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e65e1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e65e1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e65e1-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e65e1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e65e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e65e1-127">Request body</span></span>
<span data-ttu-id="e65e1-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e65e1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e65e1-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="e65e1-129">Parameter</span></span>    | <span data-ttu-id="e65e1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e65e1-130">Type</span></span>   |<span data-ttu-id="e65e1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e65e1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e65e1-132">row</span><span class="sxs-lookup"><span data-stu-id="e65e1-132">row</span></span>|<span data-ttu-id="e65e1-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e65e1-133">Int32</span></span>|<span data-ttu-id="e65e1-p104">Номер строки диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="e65e1-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e65e1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e65e1-136">Response</span></span>

<span data-ttu-id="e65e1-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e65e1-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e65e1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e65e1-138">Example</span></span>
<span data-ttu-id="e65e1-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e65e1-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e65e1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e65e1-140">Request</span></span>
<span data-ttu-id="e65e1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e65e1-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_row",
  "idempotent": true,
  "@type": "requestBodyResourceFor.range_row"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/row
Content-type: application/json
Content-length: 18

{
  "row": 2
}
```

##### <a name="response"></a><span data-ttu-id="e65e1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e65e1-142">Response</span></span>
<span data-ttu-id="e65e1-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e65e1-143">Here is an example of the response.</span></span> <span data-ttu-id="e65e1-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e65e1-144">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

