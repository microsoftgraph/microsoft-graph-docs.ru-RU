---
title: 'Table: DataBodyRange'
description: Получает объект диапазона, связанный с основными данными таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d66911b1906df828ee4e1b345e8090070ddebab9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517563"
---
# <a name="table-databodyrange"></a><span data-ttu-id="7a5a9-103">Table: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="7a5a9-103">Table: DataBodyRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a5a9-104">Получает объект диапазона, связанный с данными таблицы.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-104">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a5a9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a5a9-105">Permissions</span></span>
<span data-ttu-id="7a5a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a5a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a5a9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a5a9-108">Permission type</span></span>      | <span data-ttu-id="7a5a9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a5a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a5a9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a5a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7a5a9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a5a9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7a5a9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a5a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a5a9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a5a9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7a5a9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a5a9-114">Application</span></span> | <span data-ttu-id="7a5a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a5a9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a5a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/DataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="7a5a9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a5a9-117">Request headers</span></span>
| <span data-ttu-id="7a5a9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7a5a9-118">Name</span></span>       | <span data-ttu-id="7a5a9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7a5a9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a5a9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a5a9-120">Authorization</span></span>  | <span data-ttu-id="7a5a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a5a9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7a5a9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7a5a9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a5a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a5a9-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7a5a9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a5a9-127">Response</span></span>

<span data-ttu-id="7a5a9-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a5a9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7a5a9-129">Example</span></span>
<span data-ttu-id="7a5a9-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7a5a9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a5a9-131">Request</span></span>
<span data-ttu-id="7a5a9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a5a9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_databodyrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange
```

##### <a name="response"></a><span data-ttu-id="7a5a9-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a5a9-133">Response</span></span>
<span data-ttu-id="7a5a9-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7a5a9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-databodyrange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
