---
title: 'Worksheet: Range'
description: Возвращает объект диапазона, указанный по адресу или имени.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 86bc1295382146fbfd9350f838b5884d1c792556
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451191"
---
# <a name="worksheet-range"></a><span data-ttu-id="327f9-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="327f9-103">Worksheet: Range</span></span>

<span data-ttu-id="327f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="327f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="327f9-105">Возвращает объект диапазона, указанный по адресу или имени.</span><span class="sxs-lookup"><span data-stu-id="327f9-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="327f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="327f9-106">Permissions</span></span>
<span data-ttu-id="327f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="327f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="327f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="327f9-109">Permission type</span></span>      | <span data-ttu-id="327f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="327f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="327f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="327f9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="327f9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="327f9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="327f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="327f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="327f9-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="327f9-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="327f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="327f9-115">Application</span></span> | <span data-ttu-id="327f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="327f9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="327f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="327f9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="327f9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="327f9-118">Request headers</span></span>
| <span data-ttu-id="327f9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="327f9-119">Name</span></span>       | <span data-ttu-id="327f9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="327f9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="327f9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="327f9-121">Authorization</span></span>  | <span data-ttu-id="327f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="327f9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="327f9-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="327f9-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="327f9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="327f9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="327f9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="327f9-127">Request body</span></span>
<span data-ttu-id="327f9-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="327f9-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="327f9-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="327f9-129">Parameter</span></span>    | <span data-ttu-id="327f9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="327f9-130">Type</span></span>   |<span data-ttu-id="327f9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="327f9-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="327f9-132">address</span><span class="sxs-lookup"><span data-stu-id="327f9-132">address</span></span>|<span data-ttu-id="327f9-133">string</span><span class="sxs-lookup"><span data-stu-id="327f9-133">string</span></span>|<span data-ttu-id="327f9-p104">Необязательный параметр. Адрес или имя диапазона. Если аргумент не указан, возвращается весь диапазон листа.</span><span class="sxs-lookup"><span data-stu-id="327f9-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="327f9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="327f9-137">Response</span></span>

<span data-ttu-id="327f9-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="327f9-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="327f9-139">Пример</span><span class="sxs-lookup"><span data-stu-id="327f9-139">Example</span></span>
<span data-ttu-id="327f9-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="327f9-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="327f9-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="327f9-141">Request</span></span>
<span data-ttu-id="327f9-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="327f9-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="327f9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="327f9-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="327f9-144">C#</span><span class="sxs-lookup"><span data-stu-id="327f9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="327f9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="327f9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="327f9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="327f9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="327f9-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="327f9-147">Response</span></span>
<span data-ttu-id="327f9-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="327f9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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
  ]
}
-->
