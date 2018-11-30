---
title: 'Range: Column'
description: Возвращает столбец в диапазоне.
ms.openlocfilehash: a445a567209f1d043cecf62b6f368f079ea70ca2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026791"
---
# <a name="range-column"></a><span data-ttu-id="4d41d-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="4d41d-103">Range: Column</span></span>

<span data-ttu-id="4d41d-104">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="4d41d-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d41d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d41d-105">Permissions</span></span>
<span data-ttu-id="4d41d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d41d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d41d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d41d-108">Permission type</span></span>      | <span data-ttu-id="4d41d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d41d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d41d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d41d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d41d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d41d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d41d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d41d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d41d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d41d-113">Not supported.</span></span>    |
|<span data-ttu-id="4d41d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d41d-114">Application</span></span> | <span data-ttu-id="4d41d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d41d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d41d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d41d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="4d41d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d41d-117">Request headers</span></span>
| <span data-ttu-id="4d41d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4d41d-118">Name</span></span>       | <span data-ttu-id="4d41d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4d41d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d41d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d41d-120">Authorization</span></span>  | <span data-ttu-id="4d41d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d41d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d41d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4d41d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4d41d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4d41d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="4d41d-126">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="4d41d-126">Path parameters</span></span>
<span data-ttu-id="4d41d-127">В поле путь запроса укажите следующие параметры.</span><span class="sxs-lookup"><span data-stu-id="4d41d-127">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="4d41d-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="4d41d-128">Parameter</span></span>    | <span data-ttu-id="4d41d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4d41d-129">Type</span></span>   |<span data-ttu-id="4d41d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4d41d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d41d-131">column</span><span class="sxs-lookup"><span data-stu-id="4d41d-131">column</span></span>|<span data-ttu-id="4d41d-132">Int32</span><span class="sxs-lookup"><span data-stu-id="4d41d-132">Int32</span></span>|<span data-ttu-id="4d41d-p104">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="4d41d-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="4d41d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d41d-135">Response</span></span>

<span data-ttu-id="4d41d-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4d41d-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d41d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="4d41d-137">Example</span></span>
<span data-ttu-id="4d41d-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4d41d-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4d41d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d41d-139">Request</span></span>
<span data-ttu-id="4d41d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d41d-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```

##### <a name="response"></a><span data-ttu-id="4d41d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d41d-141">Response</span></span>
<span data-ttu-id="4d41d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4d41d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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