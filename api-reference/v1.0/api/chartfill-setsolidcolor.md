---
title: 'ChartFill: setSolidColor'
description: Задает заливку одним цветом для элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5864ab47c3b7806685674ace46c27d537e09de18
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316634"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="892eb-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="892eb-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="892eb-104">Задает заливку одним цветом для элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="892eb-104">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="892eb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="892eb-105">Permissions</span></span>
<span data-ttu-id="892eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="892eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="892eb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="892eb-108">Permission type</span></span>      | <span data-ttu-id="892eb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="892eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="892eb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="892eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="892eb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="892eb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="892eb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="892eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="892eb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="892eb-113">Not supported.</span></span>    |
|<span data-ttu-id="892eb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="892eb-114">Application</span></span> | <span data-ttu-id="892eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="892eb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="892eb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="892eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="892eb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="892eb-117">Request headers</span></span>
| <span data-ttu-id="892eb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="892eb-118">Name</span></span>       | <span data-ttu-id="892eb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="892eb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="892eb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="892eb-120">Authorization</span></span>  | <span data-ttu-id="892eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="892eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="892eb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="892eb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="892eb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="892eb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="892eb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="892eb-126">Request body</span></span>
<span data-ttu-id="892eb-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="892eb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="892eb-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="892eb-128">Parameter</span></span>    | <span data-ttu-id="892eb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="892eb-129">Type</span></span>   |<span data-ttu-id="892eb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="892eb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="892eb-131">color</span><span class="sxs-lookup"><span data-stu-id="892eb-131">color</span></span>|<span data-ttu-id="892eb-132">string</span><span class="sxs-lookup"><span data-stu-id="892eb-132">string</span></span>|<span data-ttu-id="892eb-133">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="892eb-133">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="892eb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="892eb-134">Response</span></span>

<span data-ttu-id="892eb-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="892eb-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="892eb-137">Пример</span><span class="sxs-lookup"><span data-stu-id="892eb-137">Example</span></span>
<span data-ttu-id="892eb-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="892eb-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="892eb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="892eb-139">Request</span></span>
<span data-ttu-id="892eb-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="892eb-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="892eb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="892eb-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="892eb-142">C#</span><span class="sxs-lookup"><span data-stu-id="892eb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="892eb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="892eb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="892eb-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="892eb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="892eb-145">Java</span><span class="sxs-lookup"><span data-stu-id="892eb-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="892eb-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="892eb-146">Response</span></span>
<span data-ttu-id="892eb-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="892eb-147">Here is an example of the response.</span></span> 
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
