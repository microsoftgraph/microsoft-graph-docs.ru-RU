---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: db17537de2cd002a16b2c0306d4e4c9304010e44
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961479"
---
# <a name="range-usedrange"></a><span data-ttu-id="589fe-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="589fe-103">Range: UsedRange</span></span>

<span data-ttu-id="589fe-104">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="589fe-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="589fe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="589fe-105">Permissions</span></span>
<span data-ttu-id="589fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="589fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="589fe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="589fe-108">Permission type</span></span>      | <span data-ttu-id="589fe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="589fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="589fe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="589fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="589fe-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="589fe-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="589fe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="589fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="589fe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="589fe-113">Not supported.</span></span>    |
|<span data-ttu-id="589fe-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="589fe-114">Application</span></span> | <span data-ttu-id="589fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="589fe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="589fe-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="589fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="589fe-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="589fe-117">Request headers</span></span>
| <span data-ttu-id="589fe-118">Имя</span><span class="sxs-lookup"><span data-stu-id="589fe-118">Name</span></span>       | <span data-ttu-id="589fe-119">Описание</span><span class="sxs-lookup"><span data-stu-id="589fe-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="589fe-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="589fe-120">Authorization</span></span>  | <span data-ttu-id="589fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="589fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="589fe-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="589fe-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="589fe-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="589fe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="589fe-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="589fe-126">Path parameters</span></span>
| <span data-ttu-id="589fe-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="589fe-127">Parameter</span></span>    | <span data-ttu-id="589fe-128">Тип</span><span class="sxs-lookup"><span data-stu-id="589fe-128">Type</span></span>   |<span data-ttu-id="589fe-129">Описание</span><span class="sxs-lookup"><span data-stu-id="589fe-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="589fe-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="589fe-130">valuesOnly</span></span>|<span data-ttu-id="589fe-131">boolean</span><span class="sxs-lookup"><span data-stu-id="589fe-131">boolean</span></span>|<span data-ttu-id="589fe-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="589fe-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="589fe-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="589fe-134">Response</span></span>

<span data-ttu-id="589fe-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="589fe-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="589fe-136">Пример</span><span class="sxs-lookup"><span data-stu-id="589fe-136">Example</span></span>
<span data-ttu-id="589fe-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="589fe-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="589fe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="589fe-138">Request</span></span>
<span data-ttu-id="589fe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="589fe-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="589fe-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="589fe-140">Response</span></span>
<span data-ttu-id="589fe-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="589fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="589fe-144">Ниже приведен пример указания Дополнительно `valuesOnly` параметр.</span><span class="sxs-lookup"><span data-stu-id="589fe-144">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="589fe-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="589fe-145">Request</span></span>
<span data-ttu-id="589fe-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="589fe-146">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="589fe-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="589fe-147">Response</span></span>

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
