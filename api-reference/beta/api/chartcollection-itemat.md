---
title: 'Воркбукчартколлектион: Итемат'
description: Получает объект воркбукчарт, основанный на его позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 39b96da2dcaff690c445ba68a2a93d5aa12c62d1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317230"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="be58f-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="be58f-103">ChartCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be58f-104">Возвращает диаграмму на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="be58f-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="be58f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be58f-105">Permissions</span></span>
<span data-ttu-id="be58f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be58f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be58f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be58f-108">Permission type</span></span>      | <span data-ttu-id="be58f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be58f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be58f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be58f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be58f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be58f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be58f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be58f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be58f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be58f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be58f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be58f-114">Application</span></span> | <span data-ttu-id="be58f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be58f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be58f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be58f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="be58f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be58f-117">Request headers</span></span>
| <span data-ttu-id="be58f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="be58f-118">Name</span></span>       | <span data-ttu-id="be58f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="be58f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="be58f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be58f-120">Authorization</span></span>  | <span data-ttu-id="be58f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be58f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be58f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="be58f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="be58f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="be58f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be58f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be58f-126">Request body</span></span>
<span data-ttu-id="be58f-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="be58f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="be58f-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="be58f-128">Parameter</span></span>    | <span data-ttu-id="be58f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="be58f-129">Type</span></span>   |<span data-ttu-id="be58f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="be58f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be58f-131">index</span><span class="sxs-lookup"><span data-stu-id="be58f-131">index</span></span>|<span data-ttu-id="be58f-132">number</span><span class="sxs-lookup"><span data-stu-id="be58f-132">number</span></span>|<span data-ttu-id="be58f-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="be58f-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="be58f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="be58f-135">Response</span></span>

<span data-ttu-id="be58f-136">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукчарт](../resources/workbookchart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be58f-136">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be58f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="be58f-137">Example</span></span>
<span data-ttu-id="be58f-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="be58f-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="be58f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="be58f-139">Request</span></span>
<span data-ttu-id="be58f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be58f-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be58f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="be58f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be58f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be58f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be58f-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="be58f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="be58f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="be58f-144">Response</span></span>
<span data-ttu-id="be58f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be58f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
