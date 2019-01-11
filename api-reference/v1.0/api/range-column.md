---
title: 'Range: Column'
description: Возвращает столбец в диапазоне.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 5966e8429d2a0406df3b6774db673d286cc4c8b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870898"
---
# <a name="range-column"></a><span data-ttu-id="c8ea9-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="c8ea9-103">Range: Column</span></span>

<span data-ttu-id="c8ea9-104">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8ea9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8ea9-105">Permissions</span></span>
<span data-ttu-id="c8ea9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8ea9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8ea9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8ea9-108">Permission type</span></span>      | <span data-ttu-id="c8ea9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8ea9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8ea9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8ea9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8ea9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8ea9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8ea9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8ea9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8ea9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-113">Not supported.</span></span>    |
|<span data-ttu-id="c8ea9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8ea9-114">Application</span></span> | <span data-ttu-id="c8ea9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8ea9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8ea9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="c8ea9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8ea9-117">Request headers</span></span>
| <span data-ttu-id="c8ea9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c8ea9-118">Name</span></span>       | <span data-ttu-id="c8ea9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c8ea9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8ea9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8ea9-120">Authorization</span></span>  | <span data-ttu-id="c8ea9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8ea9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c8ea9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8ea9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="c8ea9-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c8ea9-126">Path parameters</span></span>
<span data-ttu-id="c8ea9-127">В поле путь запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="c8ea9-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="c8ea9-128">Parameter</span></span>    | <span data-ttu-id="c8ea9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c8ea9-129">Type</span></span>   |<span data-ttu-id="c8ea9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c8ea9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8ea9-131">column</span><span class="sxs-lookup"><span data-stu-id="c8ea9-131">column</span></span>|<span data-ttu-id="c8ea9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c8ea9-132">Int32</span></span>|<span data-ttu-id="c8ea9-p104">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="c8ea9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8ea9-135">Response</span></span>

<span data-ttu-id="c8ea9-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8ea9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c8ea9-137">Example</span></span>
<span data-ttu-id="c8ea9-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8ea9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8ea9-139">Request</span></span>
<span data-ttu-id="c8ea9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="c8ea9-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8ea9-141">Response</span></span>
<span data-ttu-id="c8ea9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8ea9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
