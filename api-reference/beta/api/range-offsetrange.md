---
title: 'Range: OffsetRange'
description: Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 22c5455a0e7e935e126e4a05aace34def5f0acff
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577016"
---
# <a name="range-offsetrange"></a><span data-ttu-id="dbae8-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="dbae8-105">Range: OffsetRange</span></span>

<span data-ttu-id="dbae8-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbae8-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbae8-p102">Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.</span><span class="sxs-lookup"><span data-stu-id="dbae8-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="dbae8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbae8-110">Permissions</span></span>
<span data-ttu-id="dbae8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbae8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbae8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbae8-113">Permission type</span></span>      | <span data-ttu-id="dbae8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbae8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbae8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbae8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="dbae8-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbae8-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dbae8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbae8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbae8-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbae8-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dbae8-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbae8-119">Application</span></span> | <span data-ttu-id="dbae8-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbae8-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbae8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbae8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/OffsetRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="dbae8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbae8-122">Request headers</span></span>
| <span data-ttu-id="dbae8-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dbae8-123">Name</span></span>       | <span data-ttu-id="dbae8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dbae8-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dbae8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbae8-125">Authorization</span></span>  | <span data-ttu-id="dbae8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbae8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbae8-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dbae8-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="dbae8-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dbae8-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbae8-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbae8-131">Request body</span></span>
<span data-ttu-id="dbae8-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dbae8-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dbae8-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="dbae8-133">Parameter</span></span>    | <span data-ttu-id="dbae8-134">Тип</span><span class="sxs-lookup"><span data-stu-id="dbae8-134">Type</span></span>   |<span data-ttu-id="dbae8-135">Описание</span><span class="sxs-lookup"><span data-stu-id="dbae8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbae8-136">rowOffset</span><span class="sxs-lookup"><span data-stu-id="dbae8-136">rowOffset</span></span>|<span data-ttu-id="dbae8-137">number</span><span class="sxs-lookup"><span data-stu-id="dbae8-137">number</span></span>|<span data-ttu-id="dbae8-p106">Количество строк (положительное, отрицательное или нулевое), на которое необходимо сместить диапазон. Положительные значения соответствуют смещению вниз, а отрицательные — вверх.</span><span class="sxs-lookup"><span data-stu-id="dbae8-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="dbae8-140">columnOffset</span><span class="sxs-lookup"><span data-stu-id="dbae8-140">columnOffset</span></span>|<span data-ttu-id="dbae8-141">number</span><span class="sxs-lookup"><span data-stu-id="dbae8-141">number</span></span>|<span data-ttu-id="dbae8-p107">Количество столбцов (положительное, отрицательное или 0), на который нужно сместить диапазон. Положительные значения соответствуют смещению вправо, а отрицательные — влево.</span><span class="sxs-lookup"><span data-stu-id="dbae8-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="dbae8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbae8-144">Response</span></span>

<span data-ttu-id="dbae8-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbae8-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbae8-146">Пример</span><span class="sxs-lookup"><span data-stu-id="dbae8-146">Example</span></span>
<span data-ttu-id="dbae8-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dbae8-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dbae8-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbae8-148">Request</span></span>
<span data-ttu-id="dbae8-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbae8-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dbae8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbae8-150">Response</span></span>
<span data-ttu-id="dbae8-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbae8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


