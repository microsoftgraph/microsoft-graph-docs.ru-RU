---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: db17537de2cd002a16b2c0306d4e4c9304010e44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503676"
---
# <a name="range-usedrange"></a><span data-ttu-id="e5a3b-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="e5a3b-103">Range: UsedRange</span></span>

<span data-ttu-id="e5a3b-104">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5a3b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5a3b-105">Permissions</span></span>
<span data-ttu-id="e5a3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5a3b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5a3b-108">Permission type</span></span>      | <span data-ttu-id="e5a3b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5a3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5a3b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5a3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5a3b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5a3b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5a3b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5a3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5a3b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-113">Not supported.</span></span>    |
|<span data-ttu-id="e5a3b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5a3b-114">Application</span></span> | <span data-ttu-id="e5a3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5a3b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5a3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="e5a3b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5a3b-117">Request headers</span></span>
| <span data-ttu-id="e5a3b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e5a3b-118">Name</span></span>       | <span data-ttu-id="e5a3b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a3b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5a3b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5a3b-120">Authorization</span></span>  | <span data-ttu-id="e5a3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5a3b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5a3b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5a3b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="e5a3b-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e5a3b-126">Path parameters</span></span>
| <span data-ttu-id="e5a3b-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="e5a3b-127">Parameter</span></span>    | <span data-ttu-id="e5a3b-128">Тип</span><span class="sxs-lookup"><span data-stu-id="e5a3b-128">Type</span></span>   |<span data-ttu-id="e5a3b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a3b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5a3b-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="e5a3b-130">valuesOnly</span></span>|<span data-ttu-id="e5a3b-131">boolean</span><span class="sxs-lookup"><span data-stu-id="e5a3b-131">boolean</span></span>|<span data-ttu-id="e5a3b-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="e5a3b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5a3b-134">Response</span></span>

<span data-ttu-id="e5a3b-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5a3b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e5a3b-136">Example</span></span>
<span data-ttu-id="e5a3b-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5a3b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5a3b-138">Request</span></span>
<span data-ttu-id="e5a3b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="e5a3b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5a3b-140">Response</span></span>
<span data-ttu-id="e5a3b-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="e5a3b-144">Ниже приведен пример, в котором указывается `valuesOnly` необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-144">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="e5a3b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5a3b-145">Request</span></span>
<span data-ttu-id="e5a3b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5a3b-146">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="e5a3b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5a3b-147">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
