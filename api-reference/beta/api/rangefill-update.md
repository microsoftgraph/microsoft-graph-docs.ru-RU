---
title: Обновление объекта rangeFill
description: Обновление свойств объекта rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4405bb1d339ef33ce9b749455d8b15d3e32a7fa0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412077"
---
# <a name="update-rangefill"></a><span data-ttu-id="88a1f-103">Обновление объекта rangeFill</span><span class="sxs-lookup"><span data-stu-id="88a1f-103">Update rangefill</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a1f-104">Обновление свойств объекта rangefill.</span><span class="sxs-lookup"><span data-stu-id="88a1f-104">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="88a1f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88a1f-105">Permissions</span></span>
<span data-ttu-id="88a1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88a1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88a1f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88a1f-108">Permission type</span></span>      | <span data-ttu-id="88a1f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88a1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88a1f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88a1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88a1f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88a1f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="88a1f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88a1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88a1f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88a1f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="88a1f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88a1f-114">Application</span></span> | <span data-ttu-id="88a1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a1f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88a1f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88a1f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="88a1f-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88a1f-117">Optional request headers</span></span>
| <span data-ttu-id="88a1f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="88a1f-118">Name</span></span>       | <span data-ttu-id="88a1f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="88a1f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="88a1f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88a1f-120">Authorization</span></span>  | <span data-ttu-id="88a1f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88a1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88a1f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="88a1f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="88a1f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="88a1f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88a1f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88a1f-126">Request body</span></span>
<span data-ttu-id="88a1f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="88a1f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="88a1f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a1f-130">Property</span></span>     | <span data-ttu-id="88a1f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="88a1f-131">Type</span></span>   |<span data-ttu-id="88a1f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="88a1f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88a1f-133">color</span><span class="sxs-lookup"><span data-stu-id="88a1f-133">color</span></span>|<span data-ttu-id="88a1f-134">string</span><span class="sxs-lookup"><span data-stu-id="88a1f-134">string</span></span>|<span data-ttu-id="88a1f-135">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="88a1f-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="88a1f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a1f-136">Response</span></span>

<span data-ttu-id="88a1f-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжефилл](../resources/workbookrangefill.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88a1f-137">If successful, this method returns a `200 OK` response code and updated [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88a1f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="88a1f-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88a1f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="88a1f-139">Request</span></span>
<span data-ttu-id="88a1f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88a1f-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="88a1f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="88a1f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="88a1f-142">C#</span><span class="sxs-lookup"><span data-stu-id="88a1f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88a1f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88a1f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88a1f-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="88a1f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="88a1f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="88a1f-145">Response</span></span>
<span data-ttu-id="88a1f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88a1f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
