---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9e8f5ef8a4c7c55ead433b0aa0557ce5fca74ecc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953053"
---
# <a name="range-boundingrect"></a><span data-ttu-id="63ca3-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="63ca3-103">Range: BoundingRect</span></span>

<span data-ttu-id="63ca3-p101">Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="63ca3-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="63ca3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63ca3-106">Permissions</span></span>
<span data-ttu-id="63ca3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63ca3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63ca3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63ca3-109">Permission type</span></span>      | <span data-ttu-id="63ca3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63ca3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63ca3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63ca3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63ca3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63ca3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="63ca3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63ca3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63ca3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ca3-114">Not supported.</span></span>    |
|<span data-ttu-id="63ca3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63ca3-115">Application</span></span> | <span data-ttu-id="63ca3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ca3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63ca3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63ca3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/boundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/boundingRect

```
## <a name="request-headers"></a><span data-ttu-id="63ca3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63ca3-118">Request headers</span></span>
| <span data-ttu-id="63ca3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="63ca3-119">Name</span></span>       | <span data-ttu-id="63ca3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="63ca3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63ca3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63ca3-121">Authorization</span></span>  | <span data-ttu-id="63ca3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63ca3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63ca3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="63ca3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="63ca3-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="63ca3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63ca3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63ca3-127">Request body</span></span>
<span data-ttu-id="63ca3-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="63ca3-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63ca3-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="63ca3-129">Parameter</span></span>    | <span data-ttu-id="63ca3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="63ca3-130">Type</span></span>   |<span data-ttu-id="63ca3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="63ca3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63ca3-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="63ca3-132">anotherRange</span></span>|<span data-ttu-id="63ca3-133">string</span><span class="sxs-lookup"><span data-stu-id="63ca3-133">string</span></span>|<span data-ttu-id="63ca3-134">Объект, адрес или имя диапазона.</span><span class="sxs-lookup"><span data-stu-id="63ca3-134">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="63ca3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="63ca3-135">Response</span></span>

<span data-ttu-id="63ca3-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63ca3-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63ca3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="63ca3-137">Example</span></span>
<span data-ttu-id="63ca3-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="63ca3-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="63ca3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="63ca3-139">Request</span></span>
<span data-ttu-id="63ca3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63ca3-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="63ca3-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="63ca3-141">Response</span></span>
<span data-ttu-id="63ca3-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="63ca3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
