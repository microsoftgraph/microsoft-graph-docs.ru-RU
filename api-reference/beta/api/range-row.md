---
title: 'Range: Row'
description: Возвращает строку из диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 25c887a1c827852c47baac5ce055e55296d564c8
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576990"
---
# <a name="range-row"></a><span data-ttu-id="e9c51-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="e9c51-103">Range: Row</span></span>

<span data-ttu-id="e9c51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9c51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9c51-105">Возвращает строку из диапазона.</span><span class="sxs-lookup"><span data-stu-id="e9c51-105">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9c51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9c51-106">Permissions</span></span>
<span data-ttu-id="e9c51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9c51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9c51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9c51-109">Permission type</span></span>      | <span data-ttu-id="e9c51-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9c51-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9c51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9c51-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9c51-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9c51-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9c51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9c51-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9c51-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9c51-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9c51-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9c51-115">Application</span></span> | <span data-ttu-id="e9c51-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9c51-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9c51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9c51-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/Row
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/Row
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Row
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="e9c51-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9c51-118">Request headers</span></span>
| <span data-ttu-id="e9c51-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e9c51-119">Name</span></span>       | <span data-ttu-id="e9c51-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e9c51-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e9c51-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9c51-121">Authorization</span></span>  | <span data-ttu-id="e9c51-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9c51-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9c51-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e9c51-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e9c51-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e9c51-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9c51-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9c51-127">Request body</span></span>
<span data-ttu-id="e9c51-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e9c51-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9c51-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="e9c51-129">Parameter</span></span>    | <span data-ttu-id="e9c51-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e9c51-130">Type</span></span>   |<span data-ttu-id="e9c51-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e9c51-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9c51-132">row</span><span class="sxs-lookup"><span data-stu-id="e9c51-132">row</span></span>|<span data-ttu-id="e9c51-133">number</span><span class="sxs-lookup"><span data-stu-id="e9c51-133">number</span></span>|<span data-ttu-id="e9c51-p104">Номер строки диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="e9c51-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e9c51-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9c51-136">Response</span></span>

<span data-ttu-id="e9c51-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9c51-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9c51-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e9c51-138">Example</span></span>
<span data-ttu-id="e9c51-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e9c51-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9c51-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9c51-140">Request</span></span>
<span data-ttu-id="e9c51-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9c51-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="e9c51-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9c51-142">Response</span></span>
<span data-ttu-id="e9c51-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9c51-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


