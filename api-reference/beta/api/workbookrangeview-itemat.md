---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5d6423e8899d9bc07038cf72ef453a87c44f53ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451331"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="485ae-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="485ae-104">workbookRangeView: itemAt</span></span>

<span data-ttu-id="485ae-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="485ae-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="485ae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="485ae-106">Permissions</span></span>
<span data-ttu-id="485ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="485ae-109">Permission type</span></span>      | <span data-ttu-id="485ae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="485ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="485ae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="485ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="485ae-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485ae-112">Not supported.</span></span>    |
|<span data-ttu-id="485ae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="485ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="485ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485ae-114">Not supported.</span></span>    |
|<span data-ttu-id="485ae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="485ae-115">Application</span></span> | <span data-ttu-id="485ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485ae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="485ae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="485ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="485ae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="485ae-118">Request headers</span></span>
| <span data-ttu-id="485ae-119">Имя</span><span class="sxs-lookup"><span data-stu-id="485ae-119">Name</span></span>       | <span data-ttu-id="485ae-120">Описание</span><span class="sxs-lookup"><span data-stu-id="485ae-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="485ae-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="485ae-121">Authorization</span></span>  | <span data-ttu-id="485ae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485ae-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="485ae-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="485ae-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="485ae-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="485ae-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="485ae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="485ae-127">Request body</span></span>
<span data-ttu-id="485ae-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="485ae-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="485ae-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="485ae-129">Parameter</span></span>    | <span data-ttu-id="485ae-130">Тип</span><span class="sxs-lookup"><span data-stu-id="485ae-130">Type</span></span>   |<span data-ttu-id="485ae-131">Описание</span><span class="sxs-lookup"><span data-stu-id="485ae-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="485ae-132">index</span><span class="sxs-lookup"><span data-stu-id="485ae-132">index</span></span>|<span data-ttu-id="485ae-133">Int32</span><span class="sxs-lookup"><span data-stu-id="485ae-133">Int32</span></span>|<span data-ttu-id="485ae-134">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="485ae-134">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="485ae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="485ae-135">Response</span></span>

<span data-ttu-id="485ae-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="485ae-136">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485ae-137">Пример</span><span class="sxs-lookup"><span data-stu-id="485ae-137">Example</span></span>
<span data-ttu-id="485ae-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="485ae-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="485ae-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="485ae-139">Request</span></span>
<span data-ttu-id="485ae-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="485ae-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="485ae-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="485ae-141">Response</span></span>
<span data-ttu-id="485ae-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="485ae-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
