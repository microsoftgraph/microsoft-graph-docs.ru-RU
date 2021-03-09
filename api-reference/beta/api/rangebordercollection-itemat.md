---
title: 'RangeBorderCollection: ItemAt'
description: Возвращает объект границы, указанный по индексу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 819b5f74981143ed2f784f89f957d66702e81d26
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576955"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="710f4-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="710f4-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="710f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="710f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="710f4-105">Возвращает объект границы, указанный по индексу.</span><span class="sxs-lookup"><span data-stu-id="710f4-105">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="710f4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="710f4-106">Permissions</span></span>
<span data-ttu-id="710f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="710f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="710f4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="710f4-109">Permission type</span></span>      | <span data-ttu-id="710f4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="710f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="710f4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="710f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="710f4-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="710f4-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="710f4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="710f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="710f4-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="710f4-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="710f4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="710f4-115">Application</span></span> | <span data-ttu-id="710f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="710f4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="710f4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="710f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/names/{name}/range/format/borders/ItemAt
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="710f4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="710f4-118">Request headers</span></span>
| <span data-ttu-id="710f4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="710f4-119">Name</span></span>       | <span data-ttu-id="710f4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="710f4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="710f4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="710f4-121">Authorization</span></span>  | <span data-ttu-id="710f4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="710f4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="710f4-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="710f4-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="710f4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="710f4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="710f4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="710f4-127">Request body</span></span>
<span data-ttu-id="710f4-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="710f4-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="710f4-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="710f4-129">Parameter</span></span>    | <span data-ttu-id="710f4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="710f4-130">Type</span></span>   |<span data-ttu-id="710f4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="710f4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="710f4-132">index</span><span class="sxs-lookup"><span data-stu-id="710f4-132">index</span></span>|<span data-ttu-id="710f4-133">number</span><span class="sxs-lookup"><span data-stu-id="710f4-133">number</span></span>|<span data-ttu-id="710f4-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="710f4-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="710f4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="710f4-136">Response</span></span>

<span data-ttu-id="710f4-137">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [workbookRangeBorder](../resources/workbookrangeborder.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="710f4-137">If successful, this method returns `200 OK` response code and [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="710f4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="710f4-138">Example</span></span>
<span data-ttu-id="710f4-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="710f4-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="710f4-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="710f4-140">Request</span></span>
<span data-ttu-id="710f4-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="710f4-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="710f4-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="710f4-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="710f4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="710f4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rangebordercollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="710f4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="710f4-144">Response</span></span>
<span data-ttu-id="710f4-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="710f4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


