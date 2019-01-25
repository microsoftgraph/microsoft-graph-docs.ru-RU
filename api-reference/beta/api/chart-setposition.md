---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4e439356f2156a14bdbc906972c44f3c3299b05b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523108"
---
# <a name="chart-setposition"></a><span data-ttu-id="abe0e-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="abe0e-103">Chart: setPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe0e-104">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="abe0e-104">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="abe0e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abe0e-105">Permissions</span></span>
<span data-ttu-id="abe0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abe0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe0e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abe0e-108">Permission type</span></span>      | <span data-ttu-id="abe0e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abe0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abe0e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abe0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abe0e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abe0e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="abe0e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abe0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abe0e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abe0e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="abe0e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abe0e-114">Application</span></span> | <span data-ttu-id="abe0e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abe0e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abe0e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abe0e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="abe0e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abe0e-117">Request headers</span></span>
| <span data-ttu-id="abe0e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="abe0e-118">Name</span></span>       | <span data-ttu-id="abe0e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="abe0e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="abe0e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abe0e-120">Authorization</span></span>  | <span data-ttu-id="abe0e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abe0e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="abe0e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="abe0e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="abe0e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="abe0e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abe0e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abe0e-126">Request body</span></span>
<span data-ttu-id="abe0e-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="abe0e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="abe0e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="abe0e-128">Parameter</span></span>    | <span data-ttu-id="abe0e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="abe0e-129">Type</span></span>   |<span data-ttu-id="abe0e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="abe0e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abe0e-131">startCell</span><span class="sxs-lookup"><span data-stu-id="abe0e-131">startCell</span></span>|<span data-ttu-id="abe0e-132">string</span><span class="sxs-lookup"><span data-stu-id="abe0e-132">string</span></span>|<span data-ttu-id="abe0e-p104">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="abe0e-p104">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="abe0e-136">endCell</span><span class="sxs-lookup"><span data-stu-id="abe0e-136">endCell</span></span>|<span data-ttu-id="abe0e-137">string</span><span class="sxs-lookup"><span data-stu-id="abe0e-137">string</span></span>|<span data-ttu-id="abe0e-p105">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="abe0e-p105">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="abe0e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe0e-141">Response</span></span>

<span data-ttu-id="abe0e-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="abe0e-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abe0e-144">Пример</span><span class="sxs-lookup"><span data-stu-id="abe0e-144">Example</span></span>
<span data-ttu-id="abe0e-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="abe0e-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="abe0e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="abe0e-146">Request</span></span>
<span data-ttu-id="abe0e-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abe0e-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="abe0e-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="abe0e-148">Response</span></span>
<span data-ttu-id="abe0e-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="abe0e-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-setposition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
