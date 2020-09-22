---
title: 'Range: Intersection'
description: Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 256849754c8b59349658e227da272a4610df92e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051587"
---
# <a name="range-intersection"></a><span data-ttu-id="152bf-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="152bf-103">Range: Intersection</span></span>

<span data-ttu-id="152bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="152bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="152bf-105">Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.</span><span class="sxs-lookup"><span data-stu-id="152bf-105">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="152bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="152bf-106">Permissions</span></span>
<span data-ttu-id="152bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="152bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="152bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="152bf-109">Permission type</span></span>      | <span data-ttu-id="152bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="152bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="152bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="152bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="152bf-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="152bf-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="152bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="152bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="152bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="152bf-114">Not supported.</span></span>    |
|<span data-ttu-id="152bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="152bf-115">Application</span></span> | <span data-ttu-id="152bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="152bf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="152bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="152bf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="152bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="152bf-118">Request headers</span></span>
| <span data-ttu-id="152bf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="152bf-119">Name</span></span>       | <span data-ttu-id="152bf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="152bf-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="152bf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="152bf-121">Authorization</span></span>  | <span data-ttu-id="152bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="152bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="152bf-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="152bf-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="152bf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="152bf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="152bf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="152bf-127">Request body</span></span>
<span data-ttu-id="152bf-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="152bf-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="152bf-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="152bf-129">Parameter</span></span>    | <span data-ttu-id="152bf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="152bf-130">Type</span></span>   |<span data-ttu-id="152bf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="152bf-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="152bf-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="152bf-132">anotherRange</span></span>|<span data-ttu-id="152bf-133">string</span><span class="sxs-lookup"><span data-stu-id="152bf-133">string</span></span>|<span data-ttu-id="152bf-134">Объект или адрес диапазона, который будет использоваться для определения пересечения диапазонов.</span><span class="sxs-lookup"><span data-stu-id="152bf-134">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="152bf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="152bf-135">Response</span></span>

<span data-ttu-id="152bf-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="152bf-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="152bf-137">Пример</span><span class="sxs-lookup"><span data-stu-id="152bf-137">Example</span></span>
<span data-ttu-id="152bf-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="152bf-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="152bf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="152bf-139">Request</span></span>
<span data-ttu-id="152bf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="152bf-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="152bf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="152bf-141">Response</span></span>
<span data-ttu-id="152bf-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="152bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

