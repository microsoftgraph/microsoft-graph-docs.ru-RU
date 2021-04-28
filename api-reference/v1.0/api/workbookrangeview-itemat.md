---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2a4636103a4e038c118051bb927c64d76c6aa906
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031405"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="5249c-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="5249c-104">workbookRangeView: itemAt</span></span>

<span data-ttu-id="5249c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5249c-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="5249c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5249c-106">Permissions</span></span>
<span data-ttu-id="5249c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5249c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5249c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5249c-109">Permission type</span></span>      | <span data-ttu-id="5249c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5249c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5249c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5249c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5249c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5249c-112">Files.ReadWrite</span></span> |
|<span data-ttu-id="5249c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5249c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5249c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5249c-114">Not supported.</span></span>    |
|<span data-ttu-id="5249c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5249c-115">Application</span></span> | <span data-ttu-id="5249c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5249c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5249c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5249c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="5249c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5249c-118">Request headers</span></span>
| <span data-ttu-id="5249c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5249c-119">Name</span></span>       | <span data-ttu-id="5249c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5249c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5249c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5249c-121">Authorization</span></span>  | <span data-ttu-id="5249c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5249c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5249c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5249c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5249c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5249c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="5249c-127">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5249c-127">Function parameters</span></span>
<span data-ttu-id="5249c-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="5249c-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="5249c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="5249c-129">Parameter</span></span>    | <span data-ttu-id="5249c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5249c-130">Type</span></span>   |<span data-ttu-id="5249c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5249c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5249c-132">index</span><span class="sxs-lookup"><span data-stu-id="5249c-132">index</span></span>|<span data-ttu-id="5249c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5249c-133">Int32</span></span>|<span data-ttu-id="5249c-134">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="5249c-134">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="5249c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5249c-135">Response</span></span>

<span data-ttu-id="5249c-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5249c-136">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5249c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5249c-137">Example</span></span>
<span data-ttu-id="5249c-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5249c-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5249c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5249c-139">Request</span></span>
<span data-ttu-id="5249c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5249c-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="5249c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5249c-141">Response</span></span>
<span data-ttu-id="5249c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5249c-142">Here is an example of the response.</span></span> <span data-ttu-id="5249c-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5249c-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```

