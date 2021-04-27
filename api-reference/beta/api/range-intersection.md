---
title: 'Range: Intersection'
description: Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dbfc9c1e1ed3977046ded1926af66b42ae390244
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055101"
---
# <a name="range-intersection"></a><span data-ttu-id="9b6be-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="9b6be-103">Range: Intersection</span></span>

<span data-ttu-id="9b6be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b6be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b6be-105">Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.</span><span class="sxs-lookup"><span data-stu-id="9b6be-105">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b6be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b6be-106">Permissions</span></span>
<span data-ttu-id="9b6be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b6be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b6be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b6be-109">Permission type</span></span>      | <span data-ttu-id="9b6be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b6be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b6be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b6be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b6be-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b6be-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b6be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b6be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b6be-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b6be-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b6be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b6be-115">Application</span></span> | <span data-ttu-id="9b6be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b6be-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b6be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b6be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/Intersection
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/Intersection
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Intersection
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="9b6be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b6be-118">Request headers</span></span>
| <span data-ttu-id="9b6be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9b6be-119">Name</span></span>       | <span data-ttu-id="9b6be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9b6be-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b6be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b6be-121">Authorization</span></span>  | <span data-ttu-id="9b6be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b6be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b6be-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9b6be-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9b6be-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9b6be-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b6be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b6be-127">Request body</span></span>
<span data-ttu-id="9b6be-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9b6be-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b6be-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="9b6be-129">Parameter</span></span>    | <span data-ttu-id="9b6be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9b6be-130">Type</span></span>   |<span data-ttu-id="9b6be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9b6be-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b6be-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="9b6be-132">anotherRange</span></span>|<span data-ttu-id="9b6be-133">string</span><span class="sxs-lookup"><span data-stu-id="9b6be-133">string</span></span>|<span data-ttu-id="9b6be-134">Объект или адрес диапазона, который будет использоваться для определения пересечения диапазонов.</span><span class="sxs-lookup"><span data-stu-id="9b6be-134">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="9b6be-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6be-135">Response</span></span>

<span data-ttu-id="9b6be-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9b6be-136">If successful, this method returns `200 OK` response code and [Range](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b6be-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9b6be-137">Example</span></span>
<span data-ttu-id="9b6be-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9b6be-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b6be-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b6be-139">Request</span></span>
<span data-ttu-id="9b6be-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b6be-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="9b6be-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6be-141">Response</span></span>
<span data-ttu-id="9b6be-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b6be-142">Here is an example of the response.</span></span> <span data-ttu-id="9b6be-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9b6be-143">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


