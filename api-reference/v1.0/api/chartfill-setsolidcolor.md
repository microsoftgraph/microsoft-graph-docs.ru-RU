---
title: 'ChartFill: setSolidColor'
description: Задает заливку одним цветом для элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c44580e0a91977c5251b43d5c8d812a127690b44
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059833"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="af86e-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="af86e-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="af86e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af86e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af86e-105">Задает заливку одним цветом для элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="af86e-105">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="af86e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af86e-106">Permissions</span></span>
<span data-ttu-id="af86e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af86e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af86e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af86e-109">Permission type</span></span>      | <span data-ttu-id="af86e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af86e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af86e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af86e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af86e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af86e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="af86e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af86e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af86e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af86e-114">Not supported.</span></span>    |
|<span data-ttu-id="af86e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af86e-115">Application</span></span> | <span data-ttu-id="af86e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af86e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="af86e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af86e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="af86e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af86e-118">Request headers</span></span>
| <span data-ttu-id="af86e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="af86e-119">Name</span></span>       | <span data-ttu-id="af86e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="af86e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="af86e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af86e-121">Authorization</span></span>  | <span data-ttu-id="af86e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af86e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af86e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="af86e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="af86e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="af86e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af86e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af86e-127">Request body</span></span>
<span data-ttu-id="af86e-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="af86e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="af86e-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="af86e-129">Parameter</span></span>    | <span data-ttu-id="af86e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="af86e-130">Type</span></span>   |<span data-ttu-id="af86e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="af86e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af86e-132">color</span><span class="sxs-lookup"><span data-stu-id="af86e-132">color</span></span>|<span data-ttu-id="af86e-133">string</span><span class="sxs-lookup"><span data-stu-id="af86e-133">string</span></span>|<span data-ttu-id="af86e-134">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="af86e-134">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="af86e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="af86e-135">Response</span></span>

<span data-ttu-id="af86e-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="af86e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af86e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="af86e-138">Example</span></span>
<span data-ttu-id="af86e-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="af86e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="af86e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="af86e-140">Request</span></span>
<span data-ttu-id="af86e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af86e-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af86e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="af86e-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="af86e-143">C#</span><span class="sxs-lookup"><span data-stu-id="af86e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af86e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af86e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af86e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af86e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af86e-146">Java</span><span class="sxs-lookup"><span data-stu-id="af86e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="af86e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="af86e-147">Response</span></span>
<span data-ttu-id="af86e-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af86e-148">Here is an example of the response.</span></span> 
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

