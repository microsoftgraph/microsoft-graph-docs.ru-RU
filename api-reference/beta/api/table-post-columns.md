---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d6735c9f57c1b32465f56da075fcaf826a2d0c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514952"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="3a5a0-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="3a5a0-103">Create TableColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a5a0-104">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a5a0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a5a0-105">Permissions</span></span>
<span data-ttu-id="3a5a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a5a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a5a0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a5a0-108">Permission type</span></span>      | <span data-ttu-id="3a5a0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a5a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a5a0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a5a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a5a0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a5a0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a5a0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a5a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a5a0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a5a0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a5a0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a5a0-114">Application</span></span> | <span data-ttu-id="3a5a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a5a0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a5a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="3a5a0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a5a0-117">Request headers</span></span>
| <span data-ttu-id="3a5a0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3a5a0-118">Name</span></span>       | <span data-ttu-id="3a5a0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3a5a0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a5a0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a5a0-120">Authorization</span></span>  | <span data-ttu-id="3a5a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a5a0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3a5a0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a5a0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a5a0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a5a0-126">Request body</span></span>
<span data-ttu-id="3a5a0-127">Предоставьте в тексте запроса описание объекта [TableColumn](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-127">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3a5a0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a5a0-128">Response</span></span>

<span data-ttu-id="3a5a0-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-129">If successful, this method returns `201 Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a5a0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3a5a0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a5a0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a5a0-131">Request</span></span>
<span data-ttu-id="3a5a0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="3a5a0-133">Предоставьте в тексте запроса описание объекта [TableColumn](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a5a0-133">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3a5a0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a5a0-134">Response</span></span>
<span data-ttu-id="3a5a0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3a5a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-post-columns.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
