---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 81c88cd8cd454c5b31d143cd22f61412a77074c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530092"
---
# <a name="worksheet-range"></a><span data-ttu-id="497fe-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="497fe-103">Worksheet: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497fe-104">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="497fe-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="497fe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="497fe-105">Permissions</span></span>
<span data-ttu-id="497fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="497fe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="497fe-108">Permission type</span></span>      | <span data-ttu-id="497fe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="497fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="497fe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="497fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="497fe-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="497fe-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="497fe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="497fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497fe-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="497fe-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="497fe-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="497fe-114">Application</span></span> | <span data-ttu-id="497fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="497fe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="497fe-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="497fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="497fe-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="497fe-117">Request headers</span></span>
| <span data-ttu-id="497fe-118">Имя</span><span class="sxs-lookup"><span data-stu-id="497fe-118">Name</span></span>       | <span data-ttu-id="497fe-119">Описание</span><span class="sxs-lookup"><span data-stu-id="497fe-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="497fe-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="497fe-120">Authorization</span></span>  | <span data-ttu-id="497fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="497fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="497fe-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="497fe-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="497fe-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="497fe-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="497fe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="497fe-126">Request body</span></span>
<span data-ttu-id="497fe-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="497fe-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="497fe-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="497fe-128">Parameter</span></span>    | <span data-ttu-id="497fe-129">Тип</span><span class="sxs-lookup"><span data-stu-id="497fe-129">Type</span></span>   |<span data-ttu-id="497fe-130">Описание</span><span class="sxs-lookup"><span data-stu-id="497fe-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="497fe-131">address</span><span class="sxs-lookup"><span data-stu-id="497fe-131">address</span></span>|<span data-ttu-id="497fe-132">string</span><span class="sxs-lookup"><span data-stu-id="497fe-132">string</span></span>|<span data-ttu-id="497fe-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="497fe-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="497fe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="497fe-136">Response</span></span>

<span data-ttu-id="497fe-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="497fe-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="497fe-138">Пример</span><span class="sxs-lookup"><span data-stu-id="497fe-138">Example</span></span>
<span data-ttu-id="497fe-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="497fe-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="497fe-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="497fe-140">Request</span></span>
<span data-ttu-id="497fe-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="497fe-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Range
Content-type: application/json
Content-length: 32

{
  "address": "address-value"
}
```

##### <a name="response"></a><span data-ttu-id="497fe-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="497fe-142">Response</span></span>
<span data-ttu-id="497fe-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="497fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
