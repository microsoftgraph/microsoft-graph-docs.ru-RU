---
title: 'Range: BoundingRect'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 19155801297caf56a9ba944b4220c4ba8db0bb36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546430"
---
# <a name="range-boundingrect"></a><span data-ttu-id="aac08-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="aac08-103">Range: BoundingRect</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aac08-p101">Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="aac08-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="aac08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aac08-106">Permissions</span></span>
<span data-ttu-id="aac08-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aac08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aac08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aac08-109">Permission type</span></span>      | <span data-ttu-id="aac08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aac08-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aac08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aac08-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aac08-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aac08-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aac08-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aac08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac08-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aac08-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aac08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aac08-115">Application</span></span> | <span data-ttu-id="aac08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aac08-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aac08-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aac08-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="aac08-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aac08-118">Request headers</span></span>
| <span data-ttu-id="aac08-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aac08-119">Name</span></span>       | <span data-ttu-id="aac08-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aac08-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aac08-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aac08-121">Authorization</span></span>  | <span data-ttu-id="aac08-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aac08-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aac08-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aac08-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="aac08-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="aac08-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aac08-127">Request body</span></span>
<span data-ttu-id="aac08-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="aac08-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aac08-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="aac08-129">Parameter</span></span>    | <span data-ttu-id="aac08-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aac08-130">Type</span></span>   |<span data-ttu-id="aac08-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aac08-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aac08-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="aac08-132">anotherRange</span></span>|<span data-ttu-id="aac08-133">string</span><span class="sxs-lookup"><span data-stu-id="aac08-133">string</span></span>|<span data-ttu-id="aac08-134">Объект, адрес или имя диапазона.</span><span class="sxs-lookup"><span data-stu-id="aac08-134">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="aac08-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="aac08-135">Response</span></span>

<span data-ttu-id="aac08-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aac08-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac08-137">Пример</span><span class="sxs-lookup"><span data-stu-id="aac08-137">Example</span></span>
<span data-ttu-id="aac08-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="aac08-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aac08-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="aac08-139">Request</span></span>
<span data-ttu-id="aac08-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aac08-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="aac08-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="aac08-141">Response</span></span>
<span data-ttu-id="aac08-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aac08-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-boundingrect.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
