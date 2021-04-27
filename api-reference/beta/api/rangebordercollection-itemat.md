---
title: 'RangeBorderCollection: ItemAt'
description: Возвращает объект границы, указанный по индексу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e8513851989f29a3676d3f0f0e20f226129b15da
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049816"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="3b81d-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="3b81d-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="3b81d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b81d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b81d-105">Возвращает объект границы, указанный по индексу.</span><span class="sxs-lookup"><span data-stu-id="3b81d-105">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="3b81d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b81d-106">Permissions</span></span>
<span data-ttu-id="3b81d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b81d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b81d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b81d-109">Permission type</span></span>      | <span data-ttu-id="3b81d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b81d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b81d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b81d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b81d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b81d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b81d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b81d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b81d-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b81d-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b81d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b81d-115">Application</span></span> | <span data-ttu-id="3b81d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b81d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b81d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b81d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders/ItemAt
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="3b81d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b81d-118">Request headers</span></span>
| <span data-ttu-id="3b81d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3b81d-119">Name</span></span>       | <span data-ttu-id="3b81d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3b81d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3b81d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b81d-121">Authorization</span></span>  | <span data-ttu-id="3b81d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b81d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b81d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3b81d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3b81d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3b81d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b81d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b81d-127">Request body</span></span>
<span data-ttu-id="3b81d-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3b81d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3b81d-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="3b81d-129">Parameter</span></span>    | <span data-ttu-id="3b81d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3b81d-130">Type</span></span>   |<span data-ttu-id="3b81d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3b81d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b81d-132">index</span><span class="sxs-lookup"><span data-stu-id="3b81d-132">index</span></span>|<span data-ttu-id="3b81d-133">number</span><span class="sxs-lookup"><span data-stu-id="3b81d-133">number</span></span>|<span data-ttu-id="3b81d-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="3b81d-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="3b81d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b81d-136">Response</span></span>

<span data-ttu-id="3b81d-137">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [workbookRangeBorder](../resources/workbookrangeborder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3b81d-137">If successful, this method returns `200 OK` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b81d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3b81d-138">Example</span></span>
<span data-ttu-id="3b81d-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3b81d-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3b81d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b81d-140">Request</span></span>
<span data-ttu-id="3b81d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b81d-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b81d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b81d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="3b81d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b81d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangebordercollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3b81d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b81d-144">Response</span></span>
<span data-ttu-id="3b81d-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b81d-145">Here is an example of the response.</span></span> <span data-ttu-id="3b81d-146">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3b81d-146">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


