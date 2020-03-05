---
title: Обновление объекта rangeFill
description: Обновление свойств объекта rangefill.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b1ee666839ea250f24ff817f06ec74d7adfa32f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454628"
---
# <a name="update-rangefill"></a><span data-ttu-id="52c12-103">Обновление объекта rangeFill</span><span class="sxs-lookup"><span data-stu-id="52c12-103">Update rangefill</span></span>

<span data-ttu-id="52c12-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52c12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52c12-105">Обновление свойств объекта rangefill.</span><span class="sxs-lookup"><span data-stu-id="52c12-105">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="52c12-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52c12-106">Permissions</span></span>
<span data-ttu-id="52c12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52c12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52c12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52c12-109">Permission type</span></span>      | <span data-ttu-id="52c12-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52c12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52c12-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52c12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="52c12-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52c12-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52c12-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52c12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52c12-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52c12-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="52c12-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52c12-115">Application</span></span> | <span data-ttu-id="52c12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52c12-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52c12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52c12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="52c12-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52c12-118">Optional request headers</span></span>
| <span data-ttu-id="52c12-119">Имя</span><span class="sxs-lookup"><span data-stu-id="52c12-119">Name</span></span>       | <span data-ttu-id="52c12-120">Описание</span><span class="sxs-lookup"><span data-stu-id="52c12-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="52c12-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52c12-121">Authorization</span></span>  | <span data-ttu-id="52c12-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52c12-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52c12-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="52c12-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="52c12-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="52c12-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52c12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52c12-127">Request body</span></span>
<span data-ttu-id="52c12-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="52c12-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="52c12-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="52c12-131">Property</span></span>     | <span data-ttu-id="52c12-132">Тип</span><span class="sxs-lookup"><span data-stu-id="52c12-132">Type</span></span>   |<span data-ttu-id="52c12-133">Описание</span><span class="sxs-lookup"><span data-stu-id="52c12-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52c12-134">color</span><span class="sxs-lookup"><span data-stu-id="52c12-134">color</span></span>|<span data-ttu-id="52c12-135">string</span><span class="sxs-lookup"><span data-stu-id="52c12-135">string</span></span>|<span data-ttu-id="52c12-136">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).</span><span class="sxs-lookup"><span data-stu-id="52c12-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="52c12-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="52c12-137">Response</span></span>

<span data-ttu-id="52c12-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукранжефилл](../resources/workbookrangefill.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52c12-138">If successful, this method returns a `200 OK` response code and updated [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52c12-139">Пример</span><span class="sxs-lookup"><span data-stu-id="52c12-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52c12-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="52c12-140">Request</span></span>
<span data-ttu-id="52c12-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52c12-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52c12-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="52c12-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="52c12-143">C#</span><span class="sxs-lookup"><span data-stu-id="52c12-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangefill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52c12-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52c12-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangefill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52c12-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52c12-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangefill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52c12-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="52c12-146">Response</span></span>
<span data-ttu-id="52c12-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52c12-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
