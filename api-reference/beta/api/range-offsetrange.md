---
title: 'Range: OffsetRange'
description: Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5cd6b8251c855e1dd3a059722f8719dae33dd2c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331897"
---
# <a name="range-offsetrange"></a><span data-ttu-id="da47c-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="da47c-105">Range: OffsetRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da47c-p102">Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.</span><span class="sxs-lookup"><span data-stu-id="da47c-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="da47c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da47c-109">Permissions</span></span>
<span data-ttu-id="da47c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da47c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da47c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da47c-112">Permission type</span></span>      | <span data-ttu-id="da47c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da47c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da47c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da47c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="da47c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da47c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da47c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da47c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da47c-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da47c-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da47c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da47c-118">Application</span></span> | <span data-ttu-id="da47c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da47c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da47c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da47c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="da47c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da47c-121">Request headers</span></span>
| <span data-ttu-id="da47c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="da47c-122">Name</span></span>       | <span data-ttu-id="da47c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="da47c-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da47c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da47c-124">Authorization</span></span>  | <span data-ttu-id="da47c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da47c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da47c-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da47c-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="da47c-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="da47c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da47c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da47c-130">Request body</span></span>
<span data-ttu-id="da47c-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="da47c-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="da47c-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="da47c-132">Parameter</span></span>    | <span data-ttu-id="da47c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="da47c-133">Type</span></span>   |<span data-ttu-id="da47c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="da47c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da47c-135">rowOffset</span><span class="sxs-lookup"><span data-stu-id="da47c-135">rowOffset</span></span>|<span data-ttu-id="da47c-136">число</span><span class="sxs-lookup"><span data-stu-id="da47c-136">number</span></span>|<span data-ttu-id="da47c-p106">Количество строк (положительное, отрицательное или нулевое), на которое необходимо сместить диапазон. Положительные значения соответствуют смещению вниз, а отрицательные — вверх.</span><span class="sxs-lookup"><span data-stu-id="da47c-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="da47c-139">columnOffset</span><span class="sxs-lookup"><span data-stu-id="da47c-139">columnOffset</span></span>|<span data-ttu-id="da47c-140">number</span><span class="sxs-lookup"><span data-stu-id="da47c-140">number</span></span>|<span data-ttu-id="da47c-p107">Количество столбцов (положительное, отрицательное или 0), на который нужно сместить диапазон. Положительные значения соответствуют смещению вправо, а отрицательные — влево.</span><span class="sxs-lookup"><span data-stu-id="da47c-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="da47c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="da47c-143">Response</span></span>

<span data-ttu-id="da47c-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da47c-144">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da47c-145">Пример</span><span class="sxs-lookup"><span data-stu-id="da47c-145">Example</span></span>
<span data-ttu-id="da47c-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="da47c-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="da47c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="da47c-147">Request</span></span>
<span data-ttu-id="da47c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da47c-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="da47c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="da47c-149">Response</span></span>
<span data-ttu-id="da47c-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da47c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
