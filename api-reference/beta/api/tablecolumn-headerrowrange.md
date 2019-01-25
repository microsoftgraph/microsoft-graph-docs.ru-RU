---
title: 'TableColumn: HeaderRowRange'
description: Получает объект диапазона, связанный со строкой заголовков столбца.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 147e12d3fb8dd26a194b1210b91e5b5d4bbb22ab
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522233"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="f5c91-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="f5c91-103">TableColumn: HeaderRowRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c91-104">Получает объект диапазона, связанный со строкой заголовков столбца.</span><span class="sxs-lookup"><span data-stu-id="f5c91-104">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5c91-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5c91-105">Permissions</span></span>
<span data-ttu-id="f5c91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5c91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5c91-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5c91-108">Permission type</span></span>      | <span data-ttu-id="f5c91-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5c91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5c91-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5c91-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f5c91-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5c91-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5c91-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5c91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5c91-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5c91-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5c91-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5c91-114">Application</span></span> | <span data-ttu-id="f5c91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5c91-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5c91-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5c91-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="f5c91-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5c91-117">Request headers</span></span>
| <span data-ttu-id="f5c91-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f5c91-118">Name</span></span>       | <span data-ttu-id="f5c91-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f5c91-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5c91-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5c91-120">Authorization</span></span>  | <span data-ttu-id="f5c91-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5c91-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5c91-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f5c91-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5c91-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f5c91-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5c91-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5c91-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f5c91-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5c91-127">Response</span></span>

<span data-ttu-id="f5c91-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f5c91-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5c91-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f5c91-129">Example</span></span>
<span data-ttu-id="f5c91-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f5c91-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5c91-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5c91-131">Request</span></span>
<span data-ttu-id="f5c91-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5c91-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="f5c91-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5c91-133">Response</span></span>
<span data-ttu-id="f5c91-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f5c91-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumn-headerrowrange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
