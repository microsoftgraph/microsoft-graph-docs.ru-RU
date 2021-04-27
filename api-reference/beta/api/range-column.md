---
title: 'Range: Column'
description: Возвращает столбец в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f3e7de29404775b3eb888fe617018503d81fea49
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055136"
---
# <a name="range-column"></a><span data-ttu-id="fc92f-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="fc92f-103">Range: Column</span></span>

<span data-ttu-id="fc92f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc92f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc92f-105">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="fc92f-105">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc92f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc92f-106">Permissions</span></span>
<span data-ttu-id="fc92f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc92f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc92f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc92f-109">Permission type</span></span>      | <span data-ttu-id="fc92f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc92f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc92f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc92f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc92f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc92f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc92f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc92f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc92f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc92f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc92f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc92f-115">Application</span></span> | <span data-ttu-id="fc92f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc92f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc92f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc92f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/Column
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/Column
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Column
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="fc92f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc92f-118">Request headers</span></span>
| <span data-ttu-id="fc92f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fc92f-119">Name</span></span>       | <span data-ttu-id="fc92f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc92f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc92f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc92f-121">Authorization</span></span>  | <span data-ttu-id="fc92f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc92f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc92f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc92f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc92f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fc92f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc92f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc92f-127">Request body</span></span>
<span data-ttu-id="fc92f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fc92f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc92f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc92f-129">Parameter</span></span>    | <span data-ttu-id="fc92f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fc92f-130">Type</span></span>   |<span data-ttu-id="fc92f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fc92f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc92f-132">column</span><span class="sxs-lookup"><span data-stu-id="fc92f-132">column</span></span>|<span data-ttu-id="fc92f-133">number</span><span class="sxs-lookup"><span data-stu-id="fc92f-133">number</span></span>|<span data-ttu-id="fc92f-p104">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="fc92f-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="fc92f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc92f-136">Response</span></span>

<span data-ttu-id="fc92f-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc92f-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc92f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="fc92f-138">Example</span></span>
<span data-ttu-id="fc92f-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc92f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc92f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc92f-140">Request</span></span>
<span data-ttu-id="fc92f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc92f-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="fc92f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc92f-142">Response</span></span>
<span data-ttu-id="fc92f-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc92f-143">Here is an example of the response.</span></span> <span data-ttu-id="fc92f-144">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc92f-144">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


