---
title: 'Range: Column'
description: Возвращает столбец в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ed2b41cc9c72607da4a9777d9685cabfd1f51980
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991942"
---
# <a name="range-column"></a><span data-ttu-id="32367-103">Range: Column</span><span class="sxs-lookup"><span data-stu-id="32367-103">Range: Column</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32367-104">Возвращает столбец в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="32367-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="32367-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32367-105">Permissions</span></span>
<span data-ttu-id="32367-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32367-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32367-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32367-108">Permission type</span></span>      | <span data-ttu-id="32367-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32367-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32367-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32367-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32367-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32367-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32367-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32367-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32367-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32367-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32367-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32367-114">Application</span></span> | <span data-ttu-id="32367-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32367-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32367-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32367-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/Column
GET /workbook/worksheets/{id|name}/range(address='<address>')/Column
GET /workbook/tables/{id|name}/columns/{id|name}/range/Column

```
## <a name="request-headers"></a><span data-ttu-id="32367-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32367-117">Request headers</span></span>
| <span data-ttu-id="32367-118">Имя</span><span class="sxs-lookup"><span data-stu-id="32367-118">Name</span></span>       | <span data-ttu-id="32367-119">Описание</span><span class="sxs-lookup"><span data-stu-id="32367-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="32367-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32367-120">Authorization</span></span>  | <span data-ttu-id="32367-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32367-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32367-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="32367-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="32367-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="32367-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32367-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32367-126">Request body</span></span>
<span data-ttu-id="32367-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="32367-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32367-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="32367-128">Parameter</span></span>    | <span data-ttu-id="32367-129">Тип</span><span class="sxs-lookup"><span data-stu-id="32367-129">Type</span></span>   |<span data-ttu-id="32367-130">Описание</span><span class="sxs-lookup"><span data-stu-id="32367-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32367-131">column</span><span class="sxs-lookup"><span data-stu-id="32367-131">column</span></span>|<span data-ttu-id="32367-132">number</span><span class="sxs-lookup"><span data-stu-id="32367-132">number</span></span>|<span data-ttu-id="32367-p104">Номер столбца диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="32367-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="32367-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="32367-135">Response</span></span>

<span data-ttu-id="32367-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="32367-136">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32367-137">Пример</span><span class="sxs-lookup"><span data-stu-id="32367-137">Example</span></span>
<span data-ttu-id="32367-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="32367-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="32367-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="32367-139">Request</span></span>
<span data-ttu-id="32367-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32367-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Column
Content-type: application/json
Content-length: 21

{
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="32367-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="32367-141">Response</span></span>
<span data-ttu-id="32367-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32367-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
