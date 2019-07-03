---
title: 'ChartFill: setSolidColor'
description: Задает заливку одним цветом для элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1930dd4fe8924d87c680a4b82304008514a0c8de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443426"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="abedf-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="abedf-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="abedf-104">Задает заливку одним цветом для элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="abedf-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="abedf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abedf-105">Permissions</span></span>
<span data-ttu-id="abedf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abedf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abedf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abedf-108">Permission type</span></span>      | <span data-ttu-id="abedf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abedf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abedf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abedf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abedf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abedf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="abedf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abedf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abedf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abedf-113">Not supported.</span></span>    |
|<span data-ttu-id="abedf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abedf-114">Application</span></span> | <span data-ttu-id="abedf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abedf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abedf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abedf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="abedf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abedf-117">Request headers</span></span>
| <span data-ttu-id="abedf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="abedf-118">Name</span></span>       | <span data-ttu-id="abedf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="abedf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="abedf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abedf-120">Authorization</span></span>  | <span data-ttu-id="abedf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abedf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="abedf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="abedf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="abedf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="abedf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abedf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="abedf-126">Request body</span></span>
<span data-ttu-id="abedf-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="abedf-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="abedf-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="abedf-128">Parameter</span></span>    | <span data-ttu-id="abedf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="abedf-129">Type</span></span>   |<span data-ttu-id="abedf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="abedf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abedf-131">color</span><span class="sxs-lookup"><span data-stu-id="abedf-131">color</span></span>|<span data-ttu-id="abedf-132">string</span><span class="sxs-lookup"><span data-stu-id="abedf-132">string</span></span>|<span data-ttu-id="abedf-133">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="abedf-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="abedf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="abedf-134">Response</span></span>

<span data-ttu-id="abedf-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="abedf-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abedf-137">Пример</span><span class="sxs-lookup"><span data-stu-id="abedf-137">Example</span></span>
<span data-ttu-id="abedf-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="abedf-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="abedf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="abedf-139">Request</span></span>
<span data-ttu-id="abedf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abedf-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="abedf-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="abedf-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abedf-142">C#</span><span class="sxs-lookup"><span data-stu-id="abedf-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abedf-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="abedf-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abedf-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="abedf-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="abedf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="abedf-145">Response</span></span>
<span data-ttu-id="abedf-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="abedf-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
