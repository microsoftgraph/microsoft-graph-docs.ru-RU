---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e5b37cc6eb9702526e73cb5a515aab8b39f9dc63
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575485"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="d4092-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="d4092-104">workbookRangeView: itemAt</span></span>

<span data-ttu-id="d4092-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4092-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="d4092-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4092-106">Permissions</span></span>
<span data-ttu-id="d4092-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4092-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4092-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4092-109">Permission type</span></span>      | <span data-ttu-id="d4092-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4092-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4092-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4092-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4092-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4092-112">Files.ReadWrite</span></span> |
|<span data-ttu-id="d4092-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4092-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4092-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4092-114">Not supported.</span></span>    |
|<span data-ttu-id="d4092-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4092-115">Application</span></span> | <span data-ttu-id="d4092-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4092-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4092-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4092-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="d4092-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4092-118">Request headers</span></span>
| <span data-ttu-id="d4092-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d4092-119">Name</span></span>       | <span data-ttu-id="d4092-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4092-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d4092-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4092-121">Authorization</span></span>  | <span data-ttu-id="d4092-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4092-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4092-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d4092-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="d4092-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d4092-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="d4092-127">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d4092-127">Function parameters</span></span>
<span data-ttu-id="d4092-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="d4092-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="d4092-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="d4092-129">Parameter</span></span>    | <span data-ttu-id="d4092-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d4092-130">Type</span></span>   |<span data-ttu-id="d4092-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d4092-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4092-132">index</span><span class="sxs-lookup"><span data-stu-id="d4092-132">index</span></span>|<span data-ttu-id="d4092-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d4092-133">Int32</span></span>|<span data-ttu-id="d4092-134">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="d4092-134">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="d4092-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4092-135">Response</span></span>

<span data-ttu-id="d4092-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d4092-136">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4092-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d4092-137">Example</span></span>
<span data-ttu-id="d4092-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d4092-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d4092-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4092-139">Request</span></span>
<span data-ttu-id="d4092-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4092-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="d4092-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4092-141">Response</span></span>
<span data-ttu-id="d4092-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4092-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

