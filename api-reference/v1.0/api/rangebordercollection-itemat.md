---
title: 'RangeBorderCollection: ItemAt'
description: Возвращает объект границы, указанный по индексу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 074314027e4c62c172245056be18a04078c6dfcb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582348"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="0ee7e-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="0ee7e-103">RangeBorderCollection: ItemAt</span></span>

<span data-ttu-id="0ee7e-104">Возвращает объект границы, указанный по индексу.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="0ee7e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee7e-105">Permissions</span></span>
<span data-ttu-id="0ee7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee7e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee7e-108">Permission type</span></span>      | <span data-ttu-id="0ee7e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ee7e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ee7e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ee7e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ee7e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ee7e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ee7e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ee7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ee7e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-113">Not supported.</span></span>    |
|<span data-ttu-id="0ee7e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ee7e-114">Application</span></span> | <span data-ttu-id="0ee7e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ee7e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ee7e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders/itemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/itemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="0ee7e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ee7e-117">Request headers</span></span>
| <span data-ttu-id="0ee7e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0ee7e-118">Name</span></span>       | <span data-ttu-id="0ee7e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0ee7e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ee7e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ee7e-120">Authorization</span></span>  | <span data-ttu-id="0ee7e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ee7e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ee7e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ee7e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee7e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ee7e-126">Request body</span></span>
<span data-ttu-id="0ee7e-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ee7e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="0ee7e-128">Parameter</span></span>    | <span data-ttu-id="0ee7e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0ee7e-129">Type</span></span>   |<span data-ttu-id="0ee7e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0ee7e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ee7e-131">index</span><span class="sxs-lookup"><span data-stu-id="0ee7e-131">index</span></span>|<span data-ttu-id="0ee7e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0ee7e-132">Int32</span></span>|<span data-ttu-id="0ee7e-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="0ee7e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee7e-135">Response</span></span>

<span data-ttu-id="0ee7e-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукранжебордер](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-136">If successful, this method returns `200 OK` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee7e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0ee7e-137">Example</span></span>
<span data-ttu-id="0ee7e-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0ee7e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ee7e-139">Request</span></span>
<span data-ttu-id="0ee7e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "rangebordercollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 1
}
```

##### <a name="response"></a><span data-ttu-id="0ee7e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee7e-141">Response</span></span>
<span data-ttu-id="0ee7e-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ee7e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
