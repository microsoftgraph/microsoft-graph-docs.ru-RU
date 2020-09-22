---
title: 'workbookRange: resizedRange'
description: Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 765de8c2452ecc065abdb28e09cf67032766b190
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062136"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="b58a3-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="b58a3-103">workbookRange: resizedRange</span></span>

<span data-ttu-id="b58a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b58a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b58a3-105">Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.</span><span class="sxs-lookup"><span data-stu-id="b58a3-105">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="b58a3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b58a3-106">Permissions</span></span>
<span data-ttu-id="b58a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b58a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b58a3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b58a3-109">Permission type</span></span>      | <span data-ttu-id="b58a3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b58a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b58a3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b58a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b58a3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b58a3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b58a3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b58a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b58a3-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b58a3-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b58a3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b58a3-115">Application</span></span> | <span data-ttu-id="b58a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b58a3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b58a3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b58a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="b58a3-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b58a3-118">Function parameters</span></span>

| <span data-ttu-id="b58a3-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="b58a3-119">Parameter</span></span>    | <span data-ttu-id="b58a3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b58a3-120">Type</span></span>   |<span data-ttu-id="b58a3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b58a3-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b58a3-122">deltarows</span><span class="sxs-lookup"><span data-stu-id="b58a3-122">deltarows</span></span>|<span data-ttu-id="b58a3-123">Int32</span><span class="sxs-lookup"><span data-stu-id="b58a3-123">Int32</span></span>|<span data-ttu-id="b58a3-p102">Количество строк, добавляемых в правый нижний угол текущего диапазона. Используйте положительное число, чтобы расширить диапазон, или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="b58a3-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="b58a3-126">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="b58a3-126">deltaColumns</span></span>|<span data-ttu-id="b58a3-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b58a3-127">Int32</span></span>|<span data-ttu-id="b58a3-p103">Количество столбцов, добавляемых в правый нижний угол, относительно текущего диапазона. Используйте положительное число, чтобы расширить диапазон или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="b58a3-p103">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b58a3-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b58a3-130">Request headers</span></span>
| <span data-ttu-id="b58a3-131">Имя</span><span class="sxs-lookup"><span data-stu-id="b58a3-131">Name</span></span>       | <span data-ttu-id="b58a3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b58a3-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b58a3-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b58a3-133">Authorization</span></span>  | <span data-ttu-id="b58a3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b58a3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b58a3-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b58a3-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="b58a3-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b58a3-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b58a3-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b58a3-139">Request body</span></span>
<span data-ttu-id="b58a3-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b58a3-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b58a3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b58a3-141">Response</span></span>

<span data-ttu-id="b58a3-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b58a3-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b58a3-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b58a3-143">Example</span></span>
<span data-ttu-id="b58a3-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b58a3-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b58a3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b58a3-145">Request</span></span>
<span data-ttu-id="b58a3-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b58a3-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="b58a3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b58a3-147">Response</span></span>
<span data-ttu-id="b58a3-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b58a3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


