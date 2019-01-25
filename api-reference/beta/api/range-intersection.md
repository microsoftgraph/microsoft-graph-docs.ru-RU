---
title: 'Range: Intersection'
description: Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8d44374fa5340b8c488920ba27f2b2bf348124e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525908"
---
# <a name="range-intersection"></a><span data-ttu-id="42737-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="42737-103">Range: Intersection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42737-104">Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.</span><span class="sxs-lookup"><span data-stu-id="42737-104">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="42737-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42737-105">Permissions</span></span>
<span data-ttu-id="42737-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42737-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42737-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42737-108">Permission type</span></span>      | <span data-ttu-id="42737-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42737-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42737-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42737-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42737-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42737-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42737-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42737-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42737-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42737-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42737-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42737-114">Application</span></span> | <span data-ttu-id="42737-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42737-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42737-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42737-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="42737-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42737-117">Request headers</span></span>
| <span data-ttu-id="42737-118">Имя</span><span class="sxs-lookup"><span data-stu-id="42737-118">Name</span></span>       | <span data-ttu-id="42737-119">Описание</span><span class="sxs-lookup"><span data-stu-id="42737-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42737-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42737-120">Authorization</span></span>  | <span data-ttu-id="42737-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42737-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42737-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="42737-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="42737-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="42737-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42737-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42737-126">Request body</span></span>
<span data-ttu-id="42737-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="42737-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="42737-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="42737-128">Parameter</span></span>    | <span data-ttu-id="42737-129">Тип</span><span class="sxs-lookup"><span data-stu-id="42737-129">Type</span></span>   |<span data-ttu-id="42737-130">Описание</span><span class="sxs-lookup"><span data-stu-id="42737-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42737-131">anotherRange</span><span class="sxs-lookup"><span data-stu-id="42737-131">anotherRange</span></span>|<span data-ttu-id="42737-132">string</span><span class="sxs-lookup"><span data-stu-id="42737-132">string</span></span>|<span data-ttu-id="42737-133">Объект или адрес диапазона, который будет использоваться для определения пересечения диапазонов.</span><span class="sxs-lookup"><span data-stu-id="42737-133">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="42737-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="42737-134">Response</span></span>

<span data-ttu-id="42737-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="42737-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42737-136">Пример</span><span class="sxs-lookup"><span data-stu-id="42737-136">Example</span></span>
<span data-ttu-id="42737-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="42737-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="42737-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="42737-138">Request</span></span>
<span data-ttu-id="42737-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42737-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="42737-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="42737-140">Response</span></span>
<span data-ttu-id="42737-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="42737-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-intersection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
