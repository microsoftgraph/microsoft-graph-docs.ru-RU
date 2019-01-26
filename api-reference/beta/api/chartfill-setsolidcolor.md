---
title: 'ChartFill: setSolidColor'
description: Задает заливку одним цветом для элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6c9e7a897d0dfb7a2577f69dff4fb9ac8f841cce
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573083"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="c14c9-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="c14c9-103">ChartFill: setSolidColor</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c14c9-104">Задает заливку одним цветом для элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c14c9-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="c14c9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c14c9-105">Permissions</span></span>
<span data-ttu-id="c14c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c14c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c14c9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c14c9-108">Permission type</span></span>      | <span data-ttu-id="c14c9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c14c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c14c9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c14c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c14c9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c14c9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c14c9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c14c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c14c9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c14c9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c14c9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c14c9-114">Application</span></span> | <span data-ttu-id="c14c9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c14c9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c14c9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c14c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="c14c9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c14c9-117">Request headers</span></span>
| <span data-ttu-id="c14c9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c14c9-118">Name</span></span>       | <span data-ttu-id="c14c9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c14c9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c14c9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c14c9-120">Authorization</span></span>  | <span data-ttu-id="c14c9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c14c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c14c9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c14c9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c14c9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c14c9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c14c9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c14c9-126">Request body</span></span>
<span data-ttu-id="c14c9-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c14c9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c14c9-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="c14c9-128">Parameter</span></span>    | <span data-ttu-id="c14c9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c14c9-129">Type</span></span>   |<span data-ttu-id="c14c9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c14c9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c14c9-131">color</span><span class="sxs-lookup"><span data-stu-id="c14c9-131">color</span></span>|<span data-ttu-id="c14c9-132">строка</span><span class="sxs-lookup"><span data-stu-id="c14c9-132">string</span></span>|<span data-ttu-id="c14c9-133">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="c14c9-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="c14c9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c14c9-134">Response</span></span>

<span data-ttu-id="c14c9-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c14c9-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c14c9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c14c9-137">Example</span></span>
<span data-ttu-id="c14c9-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c14c9-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c14c9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c14c9-139">Request</span></span>
<span data-ttu-id="c14c9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c14c9-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="c14c9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c14c9-141">Response</span></span>
<span data-ttu-id="c14c9-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c14c9-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartfill-setsolidcolor.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
