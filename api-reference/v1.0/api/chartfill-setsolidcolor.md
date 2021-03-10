---
title: 'ChartFill: setSolidColor'
description: Задает заливку одним цветом для элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e2b0b99cd3ac431b15257b3698fc050822989e93
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573721"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="e84af-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="e84af-103">ChartFill: setSolidColor</span></span>

<span data-ttu-id="e84af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e84af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e84af-105">Задает заливку одним цветом для элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e84af-105">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="e84af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e84af-106">Permissions</span></span>
<span data-ttu-id="e84af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e84af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e84af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e84af-109">Permission type</span></span>      | <span data-ttu-id="e84af-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e84af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e84af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e84af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e84af-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e84af-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e84af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e84af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e84af-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e84af-114">Not supported.</span></span>    |
|<span data-ttu-id="e84af-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e84af-115">Application</span></span> | <span data-ttu-id="e84af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e84af-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e84af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e84af-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/format/fill/setSolidColor
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/title/format/fill/setSolidColor
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="e84af-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e84af-118">Request headers</span></span>
| <span data-ttu-id="e84af-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e84af-119">Name</span></span>       | <span data-ttu-id="e84af-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e84af-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e84af-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e84af-121">Authorization</span></span>  | <span data-ttu-id="e84af-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e84af-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e84af-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e84af-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e84af-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e84af-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e84af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e84af-127">Request body</span></span>
<span data-ttu-id="e84af-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e84af-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e84af-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="e84af-129">Parameter</span></span>    | <span data-ttu-id="e84af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e84af-130">Type</span></span>   |<span data-ttu-id="e84af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e84af-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e84af-132">color</span><span class="sxs-lookup"><span data-stu-id="e84af-132">color</span></span>|<span data-ttu-id="e84af-133">string</span><span class="sxs-lookup"><span data-stu-id="e84af-133">string</span></span>|<span data-ttu-id="e84af-134">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="e84af-134">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="e84af-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e84af-135">Response</span></span>

<span data-ttu-id="e84af-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e84af-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e84af-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e84af-138">Example</span></span>
<span data-ttu-id="e84af-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e84af-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e84af-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e84af-140">Request</span></span>
<span data-ttu-id="e84af-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e84af-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e84af-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="e84af-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e84af-143">C#</span><span class="sxs-lookup"><span data-stu-id="e84af-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartfill-setsolidcolor-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e84af-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e84af-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartfill-setsolidcolor-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e84af-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e84af-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartfill-setsolidcolor-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e84af-146">Java</span><span class="sxs-lookup"><span data-stu-id="e84af-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartfill-setsolidcolor-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e84af-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e84af-147">Response</span></span>
<span data-ttu-id="e84af-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e84af-148">Here is an example of the response.</span></span> 
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

