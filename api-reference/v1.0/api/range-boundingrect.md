---
title: 'Range: BoundingRect'
description: .
author: lumine2008
ms.openlocfilehash: fbe8354a8905fde587ec1d30a5dff9a4ceb2238c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337368"
---
# <a name="range-boundingrect"></a><span data-ttu-id="0ae6a-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="0ae6a-103">Range: BoundingRect</span></span>

<span data-ttu-id="0ae6a-p101">Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="0ae6a-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="0ae6a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ae6a-106">Permissions</span></span>
<span data-ttu-id="0ae6a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ae6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ae6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ae6a-109">Permission type</span></span>      | <span data-ttu-id="0ae6a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ae6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ae6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ae6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ae6a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ae6a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ae6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ae6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ae6a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-114">Not supported.</span></span>    |
|<span data-ttu-id="0ae6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ae6a-115">Application</span></span> | <span data-ttu-id="0ae6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ae6a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ae6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/boundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/boundingRect

```
## <a name="request-headers"></a><span data-ttu-id="0ae6a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ae6a-118">Request headers</span></span>
| <span data-ttu-id="0ae6a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ae6a-119">Name</span></span>       | <span data-ttu-id="0ae6a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ae6a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ae6a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ae6a-121">Authorization</span></span>  | <span data-ttu-id="0ae6a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ae6a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ae6a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ae6a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ae6a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ae6a-127">Request body</span></span>
<span data-ttu-id="0ae6a-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ae6a-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="0ae6a-129">Parameter</span></span>    | <span data-ttu-id="0ae6a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0ae6a-130">Type</span></span>   |<span data-ttu-id="0ae6a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0ae6a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ae6a-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="0ae6a-132">anotherRange</span></span>|<span data-ttu-id="0ae6a-133">string</span><span class="sxs-lookup"><span data-stu-id="0ae6a-133">string</span></span>|<span data-ttu-id="0ae6a-134">Объект, адрес или имя диапазона.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-134">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="0ae6a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ae6a-135">Response</span></span>

<span data-ttu-id="0ae6a-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ae6a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0ae6a-137">Example</span></span>
<span data-ttu-id="0ae6a-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0ae6a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ae6a-139">Request</span></span>
<span data-ttu-id="0ae6a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0ae6a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ae6a-141">Response</span></span>
<span data-ttu-id="0ae6a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ae6a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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