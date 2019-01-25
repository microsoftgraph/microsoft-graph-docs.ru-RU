---
title: 'TableColumn: DataBodyRange'
description: Получает объект диапазона, связанный с основными данными столбца.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b0d960010cb08e2978434597cc376be7129d2e68
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509758"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="f1d3e-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="f1d3e-103">TableColumn: DataBodyRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1d3e-104">Получает объект диапазона, связанный с данными столбца.</span><span class="sxs-lookup"><span data-stu-id="f1d3e-104">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1d3e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1d3e-105">Permissions</span></span>
<span data-ttu-id="f1d3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1d3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d3e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1d3e-108">Permission type</span></span>      | <span data-ttu-id="f1d3e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1d3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1d3e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1d3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1d3e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1d3e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1d3e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1d3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1d3e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1d3e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1d3e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1d3e-114">Application</span></span> | <span data-ttu-id="f1d3e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1d3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1d3e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1d3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="f1d3e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1d3e-117">Request headers</span></span>
| <span data-ttu-id="f1d3e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f1d3e-118">Name</span></span>       | <span data-ttu-id="f1d3e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f1d3e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1d3e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1d3e-120">Authorization</span></span>  | <span data-ttu-id="f1d3e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1d3e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1d3e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f1d3e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f1d3e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f1d3e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d3e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1d3e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f1d3e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1d3e-127">Response</span></span>

<span data-ttu-id="f1d3e-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f1d3e-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1d3e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f1d3e-129">Example</span></span>
<span data-ttu-id="f1d3e-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f1d3e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1d3e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1d3e-131">Request</span></span>
<span data-ttu-id="f1d3e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1d3e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_databodyrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/DataBodyRange
```

##### <a name="response"></a><span data-ttu-id="f1d3e-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1d3e-133">Response</span></span>
<span data-ttu-id="f1d3e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f1d3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumn-databodyrange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
