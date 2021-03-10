---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5edc17252101c723f7fc00656e9f90d81c231e4b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573833"
---
# <a name="range-boundingrect"></a><span data-ttu-id="858cc-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="858cc-103">Range: BoundingRect</span></span>

<span data-ttu-id="858cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="858cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="858cc-p101">Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="858cc-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="858cc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="858cc-107">Permissions</span></span>
<span data-ttu-id="858cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="858cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="858cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="858cc-110">Permission type</span></span>      | <span data-ttu-id="858cc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="858cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="858cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="858cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="858cc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="858cc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="858cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="858cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="858cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="858cc-115">Not supported.</span></span>    |
|<span data-ttu-id="858cc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="858cc-116">Application</span></span> | <span data-ttu-id="858cc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="858cc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="858cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="858cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/boundingRect
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/boundingRect
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/boundingRect
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/boundingRect

```
## <a name="request-headers"></a><span data-ttu-id="858cc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="858cc-119">Request headers</span></span>
| <span data-ttu-id="858cc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="858cc-120">Name</span></span>       | <span data-ttu-id="858cc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="858cc-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="858cc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="858cc-122">Authorization</span></span>  | <span data-ttu-id="858cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="858cc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="858cc-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="858cc-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="858cc-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="858cc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="858cc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="858cc-128">Request body</span></span>
<span data-ttu-id="858cc-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="858cc-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="858cc-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="858cc-130">Parameter</span></span>    | <span data-ttu-id="858cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="858cc-131">Type</span></span>   |<span data-ttu-id="858cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="858cc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="858cc-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="858cc-133">anotherRange</span></span>|<span data-ttu-id="858cc-134">string</span><span class="sxs-lookup"><span data-stu-id="858cc-134">string</span></span>|<span data-ttu-id="858cc-135">Объект, адрес или имя диапазона.</span><span class="sxs-lookup"><span data-stu-id="858cc-135">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="858cc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="858cc-136">Response</span></span>

<span data-ttu-id="858cc-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="858cc-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="858cc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="858cc-138">Example</span></span>
<span data-ttu-id="858cc-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="858cc-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="858cc-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="858cc-140">Request</span></span>
<span data-ttu-id="858cc-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="858cc-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/boundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="858cc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="858cc-142">Response</span></span>
<span data-ttu-id="858cc-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="858cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

