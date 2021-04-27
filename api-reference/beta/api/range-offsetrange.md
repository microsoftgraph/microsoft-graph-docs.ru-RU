---
title: 'Range: OffsetRange'
description: Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e30c732a6e4595229c693d55647e938e8b13e5c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055073"
---
# <a name="range-offsetrange"></a><span data-ttu-id="cf285-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="cf285-105">Range: OffsetRange</span></span>

<span data-ttu-id="cf285-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf285-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf285-p102">Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.</span><span class="sxs-lookup"><span data-stu-id="cf285-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf285-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf285-110">Permissions</span></span>
<span data-ttu-id="cf285-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf285-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf285-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf285-113">Permission type</span></span>      | <span data-ttu-id="cf285-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf285-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf285-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf285-115">Delegated (work or school account)</span></span> | <span data-ttu-id="cf285-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf285-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cf285-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf285-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf285-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf285-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cf285-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf285-119">Application</span></span> | <span data-ttu-id="cf285-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf285-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf285-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf285-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/OffsetRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="cf285-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf285-122">Request headers</span></span>
| <span data-ttu-id="cf285-123">Имя</span><span class="sxs-lookup"><span data-stu-id="cf285-123">Name</span></span>       | <span data-ttu-id="cf285-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cf285-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cf285-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf285-125">Authorization</span></span>  | <span data-ttu-id="cf285-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf285-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf285-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cf285-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="cf285-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cf285-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf285-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf285-131">Request body</span></span>
<span data-ttu-id="cf285-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cf285-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cf285-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="cf285-133">Parameter</span></span>    | <span data-ttu-id="cf285-134">Тип</span><span class="sxs-lookup"><span data-stu-id="cf285-134">Type</span></span>   |<span data-ttu-id="cf285-135">Описание</span><span class="sxs-lookup"><span data-stu-id="cf285-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf285-136">rowOffset</span><span class="sxs-lookup"><span data-stu-id="cf285-136">rowOffset</span></span>|<span data-ttu-id="cf285-137">number</span><span class="sxs-lookup"><span data-stu-id="cf285-137">number</span></span>|<span data-ttu-id="cf285-p106">Количество строк (положительное, отрицательное или нулевое), на которое необходимо сместить диапазон. Положительные значения соответствуют смещению вниз, а отрицательные — вверх.</span><span class="sxs-lookup"><span data-stu-id="cf285-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="cf285-140">columnOffset</span><span class="sxs-lookup"><span data-stu-id="cf285-140">columnOffset</span></span>|<span data-ttu-id="cf285-141">number</span><span class="sxs-lookup"><span data-stu-id="cf285-141">number</span></span>|<span data-ttu-id="cf285-p107">Количество столбцов (положительное, отрицательное или 0), на который нужно сместить диапазон. Положительные значения соответствуют смещению вправо, а отрицательные — влево.</span><span class="sxs-lookup"><span data-stu-id="cf285-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="cf285-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf285-144">Response</span></span>

<span data-ttu-id="cf285-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf285-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf285-146">Пример</span><span class="sxs-lookup"><span data-stu-id="cf285-146">Example</span></span>
<span data-ttu-id="cf285-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cf285-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cf285-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf285-148">Request</span></span>
<span data-ttu-id="cf285-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf285-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="cf285-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf285-150">Response</span></span>
<span data-ttu-id="cf285-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf285-151">Here is an example of the response.</span></span> <span data-ttu-id="cf285-152">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf285-152">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


