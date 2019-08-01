---
title: 'ChartCollection: ItemAt'
description: Возвращает диаграмму на основании сведений о ее позиции в коллекции.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 029f22ee7af7a1762b1bb9b10790901580860e5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003618"
---
# <a name="chartcollection-itemat"></a><span data-ttu-id="7d645-103">ChartCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="7d645-103">ChartCollection: ItemAt</span></span>

<span data-ttu-id="7d645-104">Возвращает диаграмму на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="7d645-104">Gets a chart based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d645-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d645-105">Permissions</span></span>
<span data-ttu-id="7d645-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d645-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d645-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d645-108">Permission type</span></span>      | <span data-ttu-id="7d645-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d645-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d645-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d645-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d645-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d645-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d645-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d645-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d645-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d645-113">Not supported.</span></span>    |
|<span data-ttu-id="7d645-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d645-114">Application</span></span> | <span data-ttu-id="7d645-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d645-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d645-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d645-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7d645-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d645-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="7d645-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d645-118">Request headers</span></span>
| <span data-ttu-id="7d645-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d645-119">Name</span></span>       | <span data-ttu-id="7d645-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7d645-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d645-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d645-121">Authorization</span></span>  | <span data-ttu-id="7d645-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d645-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d645-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d645-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d645-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7d645-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d645-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d645-127">Request body</span></span>
<span data-ttu-id="7d645-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7d645-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d645-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="7d645-129">Parameter</span></span>    | <span data-ttu-id="7d645-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7d645-130">Type</span></span>   |<span data-ttu-id="7d645-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7d645-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d645-132">index</span><span class="sxs-lookup"><span data-stu-id="7d645-132">index</span></span>|<span data-ttu-id="7d645-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7d645-133">Int32</span></span>|<span data-ttu-id="7d645-p104">Значение индекса получаемого объекта. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="7d645-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7d645-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d645-136">Response</span></span>

<span data-ttu-id="7d645-137">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [воркбукчарт](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d645-137">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d645-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7d645-138">Example</span></span>
<span data-ttu-id="7d645-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7d645-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d645-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d645-140">Request</span></span>
<span data-ttu-id="7d645-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d645-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d645-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d645-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d645-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7d645-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7d645-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d645-144">Response</span></span>
<span data-ttu-id="7d645-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d645-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
