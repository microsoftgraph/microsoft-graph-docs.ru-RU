---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
ms.openlocfilehash: 108c19b5af6fcaf5b4c0792d9a71b8f32f1d6148
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301717"
---
# <a name="range-usedrange"></a><span data-ttu-id="9c462-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="9c462-103">Range: UsedRange</span></span>

<span data-ttu-id="9c462-104">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="9c462-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c462-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c462-105">Permissions</span></span>
<span data-ttu-id="9c462-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c462-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c462-108">Permission type</span></span>      | <span data-ttu-id="9c462-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c462-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c462-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c462-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c462-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c462-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c462-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c462-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c462-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c462-113">Not supported.</span></span>    |
|<span data-ttu-id="9c462-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c462-114">Application</span></span> | <span data-ttu-id="9c462-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c462-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c462-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c462-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="9c462-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c462-117">Request headers</span></span>
| <span data-ttu-id="9c462-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9c462-118">Name</span></span>       | <span data-ttu-id="9c462-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9c462-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9c462-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c462-120">Authorization</span></span>  | <span data-ttu-id="9c462-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c462-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c462-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9c462-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9c462-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9c462-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="9c462-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="9c462-126">Path parameters</span></span>
| <span data-ttu-id="9c462-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="9c462-127">Parameter</span></span>    | <span data-ttu-id="9c462-128">Тип</span><span class="sxs-lookup"><span data-stu-id="9c462-128">Type</span></span>   |<span data-ttu-id="9c462-129">Описание</span><span class="sxs-lookup"><span data-stu-id="9c462-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c462-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="9c462-130">valuesOnly</span></span>|<span data-ttu-id="9c462-131">boolean</span><span class="sxs-lookup"><span data-stu-id="9c462-131">boolean</span></span>|<span data-ttu-id="9c462-p104">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="9c462-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="9c462-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c462-134">Response</span></span>

<span data-ttu-id="9c462-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9c462-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c462-136">Пример</span><span class="sxs-lookup"><span data-stu-id="9c462-136">Example</span></span>
<span data-ttu-id="9c462-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9c462-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c462-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c462-138">Request</span></span>
<span data-ttu-id="9c462-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c462-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="9c462-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c462-140">Response</span></span>
<span data-ttu-id="9c462-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9c462-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="9c462-144">Ниже приведен пример указания Дополнительно `valuesOnly` параметр.</span><span class="sxs-lookup"><span data-stu-id="9c462-144">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="9c462-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c462-145">Request</span></span>
<span data-ttu-id="9c462-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c462-146">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="9c462-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c462-147">Response</span></span>

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