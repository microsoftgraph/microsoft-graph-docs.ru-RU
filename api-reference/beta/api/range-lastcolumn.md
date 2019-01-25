---
title: 'Range: LastColumn'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dae9fc8c3469d894c504a7e9747ee66d0adfcb72
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508365"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="5f32d-103">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="5f32d-103">Range: LastColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f32d-p101">Возвращает последний столбец в диапазоне. Например, последний столбец диапазона B2:D5 — D2:D5.</span><span class="sxs-lookup"><span data-stu-id="5f32d-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="5f32d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f32d-106">Permissions</span></span>
<span data-ttu-id="5f32d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f32d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f32d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f32d-109">Permission type</span></span>      | <span data-ttu-id="5f32d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f32d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f32d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f32d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5f32d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f32d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5f32d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f32d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f32d-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f32d-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5f32d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f32d-115">Application</span></span> | <span data-ttu-id="5f32d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f32d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f32d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f32d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="5f32d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f32d-118">Request headers</span></span>
| <span data-ttu-id="5f32d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5f32d-119">Name</span></span>       | <span data-ttu-id="5f32d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5f32d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5f32d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f32d-121">Authorization</span></span>  | <span data-ttu-id="5f32d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f32d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f32d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5f32d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5f32d-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5f32d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f32d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f32d-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5f32d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f32d-128">Response</span></span>

<span data-ttu-id="5f32d-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5f32d-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f32d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5f32d-130">Example</span></span>
<span data-ttu-id="5f32d-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5f32d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5f32d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f32d-132">Request</span></span>
<span data-ttu-id="5f32d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f32d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastColumn
```

##### <a name="response"></a><span data-ttu-id="5f32d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f32d-134">Response</span></span>
<span data-ttu-id="5f32d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5f32d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastcolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
