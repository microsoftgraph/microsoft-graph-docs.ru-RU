---
title: 'TableColumn: Range'
description: Получает объект диапазона, связанный со всем столбцом.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 754fe9b22a20d8a0e082d7f4de7c183c47ed78ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330273"
---
# <a name="tablecolumn-range"></a><span data-ttu-id="c342a-103">TableColumn: Range</span><span class="sxs-lookup"><span data-stu-id="c342a-103">TableColumn: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c342a-104">Получает объект диапазона, связанный со всем столбцом.</span><span class="sxs-lookup"><span data-stu-id="c342a-104">Gets the range object associated with the entire column.</span></span>
## <a name="permissions"></a><span data-ttu-id="c342a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c342a-105">Permissions</span></span>
<span data-ttu-id="c342a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c342a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c342a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c342a-108">Permission type</span></span>      | <span data-ttu-id="c342a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c342a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c342a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c342a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c342a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c342a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c342a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c342a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c342a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c342a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c342a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c342a-114">Application</span></span> | <span data-ttu-id="c342a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c342a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c342a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c342a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="c342a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c342a-117">Request headers</span></span>
| <span data-ttu-id="c342a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c342a-118">Name</span></span>       | <span data-ttu-id="c342a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c342a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c342a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c342a-120">Authorization</span></span>  | <span data-ttu-id="c342a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c342a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c342a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c342a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c342a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c342a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c342a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c342a-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c342a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c342a-127">Response</span></span>

<span data-ttu-id="c342a-128">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [workbookRange](../resources/workbookrange.md)) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c342a-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md)) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c342a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c342a-129">Example</span></span>
<span data-ttu-id="c342a-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c342a-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c342a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c342a-131">Request</span></span>
<span data-ttu-id="c342a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c342a-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range
```

##### <a name="response"></a><span data-ttu-id="c342a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c342a-133">Response</span></span>
<span data-ttu-id="c342a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c342a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
