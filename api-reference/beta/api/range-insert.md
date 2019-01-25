---
title: 'Range: insert'
description: Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 01bb7b3a756b9d97d2d849c49cade0ff285168a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508680"
---
# <a name="range-insert"></a><span data-ttu-id="a159f-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="a159f-104">Range: insert</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a159f-p102">Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.</span><span class="sxs-lookup"><span data-stu-id="a159f-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="a159f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a159f-107">Permissions</span></span>
<span data-ttu-id="a159f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a159f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a159f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a159f-110">Permission type</span></span>      | <span data-ttu-id="a159f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a159f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a159f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a159f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a159f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a159f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a159f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a159f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a159f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a159f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a159f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a159f-116">Application</span></span> | <span data-ttu-id="a159f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a159f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a159f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a159f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="a159f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a159f-119">Request headers</span></span>
| <span data-ttu-id="a159f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a159f-120">Name</span></span>       | <span data-ttu-id="a159f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a159f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a159f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a159f-122">Authorization</span></span>  | <span data-ttu-id="a159f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a159f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a159f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a159f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a159f-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a159f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a159f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a159f-128">Request body</span></span>
<span data-ttu-id="a159f-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a159f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a159f-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="a159f-130">Parameter</span></span>    | <span data-ttu-id="a159f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a159f-131">Type</span></span>   |<span data-ttu-id="a159f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a159f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a159f-133">shift</span><span class="sxs-lookup"><span data-stu-id="a159f-133">shift</span></span>|<span data-ttu-id="a159f-134">string</span><span class="sxs-lookup"><span data-stu-id="a159f-134">string</span></span>|<span data-ttu-id="a159f-p106">Указывает направление сдвига ячеек.  Возможные значения: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="a159f-p106">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="a159f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a159f-137">Response</span></span>

<span data-ttu-id="a159f-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a159f-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a159f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a159f-139">Example</span></span>
<span data-ttu-id="a159f-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a159f-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a159f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a159f-141">Request</span></span>
<span data-ttu-id="a159f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a159f-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="a159f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a159f-143">Response</span></span>
<span data-ttu-id="a159f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a159f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-insert.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
