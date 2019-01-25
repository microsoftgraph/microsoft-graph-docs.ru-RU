---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8f6ed391f1158b6b9253827c52c50a0b197e31a5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510255"
---
# <a name="range-lastrow"></a><span data-ttu-id="ea3bd-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="ea3bd-103">Range: LastRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea3bd-p101">Возвращает последнюю строку в диапазоне. Например, последняя строка в диапазоне "B2:D5" — "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="ea3bd-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="ea3bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea3bd-106">Permissions</span></span>
<span data-ttu-id="ea3bd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea3bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea3bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea3bd-109">Permission type</span></span>      | <span data-ttu-id="ea3bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea3bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea3bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea3bd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea3bd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea3bd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea3bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea3bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea3bd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea3bd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ea3bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea3bd-115">Application</span></span> | <span data-ttu-id="ea3bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea3bd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea3bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea3bd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="ea3bd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea3bd-118">Request headers</span></span>
| <span data-ttu-id="ea3bd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ea3bd-119">Name</span></span>       | <span data-ttu-id="ea3bd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ea3bd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea3bd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea3bd-121">Authorization</span></span>  | <span data-ttu-id="ea3bd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea3bd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea3bd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ea3bd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ea3bd-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ea3bd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea3bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea3bd-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ea3bd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea3bd-128">Response</span></span>

<span data-ttu-id="ea3bd-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ea3bd-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea3bd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ea3bd-130">Example</span></span>
<span data-ttu-id="ea3bd-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ea3bd-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ea3bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea3bd-132">Request</span></span>
<span data-ttu-id="ea3bd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea3bd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="ea3bd-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea3bd-134">Response</span></span>
<span data-ttu-id="ea3bd-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ea3bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
