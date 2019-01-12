---
title: 'Range: OffsetRange'
description: Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4f1a513a33185dba976398e31caf4996005feb67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925800"
---
# <a name="range-offsetrange"></a><span data-ttu-id="9330c-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="9330c-105">Range: OffsetRange</span></span>

> <span data-ttu-id="9330c-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9330c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9330c-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9330c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9330c-p103">Возвращает объект, представляющий диапазон, который смещен от указанного диапазона. Измерение возвращаемого диапазона будет соответствовать этому диапазону. Если результирующий диапазон выходит за пределы таблицы листа, вызывается исключение.</span><span class="sxs-lookup"><span data-stu-id="9330c-p103">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="9330c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9330c-111">Permissions</span></span>
<span data-ttu-id="9330c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9330c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9330c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9330c-114">Permission type</span></span>      | <span data-ttu-id="9330c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9330c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9330c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9330c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9330c-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9330c-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9330c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9330c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9330c-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9330c-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9330c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9330c-120">Application</span></span> | <span data-ttu-id="9330c-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9330c-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9330c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9330c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="9330c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9330c-123">Request headers</span></span>
| <span data-ttu-id="9330c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9330c-124">Name</span></span>       | <span data-ttu-id="9330c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9330c-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9330c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9330c-126">Authorization</span></span>  | <span data-ttu-id="9330c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9330c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9330c-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9330c-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="9330c-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9330c-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9330c-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9330c-132">Request body</span></span>
<span data-ttu-id="9330c-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9330c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9330c-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="9330c-134">Parameter</span></span>    | <span data-ttu-id="9330c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="9330c-135">Type</span></span>   |<span data-ttu-id="9330c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9330c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9330c-137">rowOffset</span><span class="sxs-lookup"><span data-stu-id="9330c-137">rowOffset</span></span>|<span data-ttu-id="9330c-138">number</span><span class="sxs-lookup"><span data-stu-id="9330c-138">number</span></span>|<span data-ttu-id="9330c-p107">Количество строк (положительное, отрицательное или нулевое), на которое необходимо сместить диапазон. Положительные значения соответствуют смещению вниз, а отрицательные — вверх.</span><span class="sxs-lookup"><span data-stu-id="9330c-p107">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="9330c-141">columnOffset</span><span class="sxs-lookup"><span data-stu-id="9330c-141">columnOffset</span></span>|<span data-ttu-id="9330c-142">number</span><span class="sxs-lookup"><span data-stu-id="9330c-142">number</span></span>|<span data-ttu-id="9330c-p108">Количество столбцов (положительное, отрицательное или 0), на который нужно сместить диапазон. Положительные значения соответствуют смещению вправо, а отрицательные — влево.</span><span class="sxs-lookup"><span data-stu-id="9330c-p108">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="9330c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9330c-145">Response</span></span>

<span data-ttu-id="9330c-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9330c-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9330c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9330c-147">Example</span></span>
<span data-ttu-id="9330c-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9330c-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9330c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="9330c-149">Request</span></span>
<span data-ttu-id="9330c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9330c-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="9330c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="9330c-151">Response</span></span>
<span data-ttu-id="9330c-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9330c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
