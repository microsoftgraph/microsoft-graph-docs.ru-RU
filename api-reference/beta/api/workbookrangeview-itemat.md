---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6a425d28f259fc0a085ebcd3e46f614c19c1a954
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339687"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="8e839-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="8e839-104">workbookRangeView: itemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="8e839-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e839-105">Permissions</span></span>
<span data-ttu-id="8e839-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e839-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e839-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e839-108">Permission type</span></span>      | <span data-ttu-id="8e839-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e839-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e839-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e839-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e839-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e839-111">Not supported.</span></span>    |
|<span data-ttu-id="8e839-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e839-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e839-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e839-113">Not supported.</span></span>    |
|<span data-ttu-id="8e839-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e839-114">Application</span></span> | <span data-ttu-id="8e839-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e839-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e839-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e839-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="8e839-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e839-117">Request headers</span></span>
| <span data-ttu-id="8e839-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8e839-118">Name</span></span>       | <span data-ttu-id="8e839-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8e839-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8e839-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e839-120">Authorization</span></span>  | <span data-ttu-id="8e839-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e839-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e839-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8e839-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8e839-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8e839-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e839-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e839-126">Request body</span></span>
<span data-ttu-id="8e839-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8e839-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="8e839-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="8e839-128">Parameter</span></span>    | <span data-ttu-id="8e839-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8e839-129">Type</span></span>   |<span data-ttu-id="8e839-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8e839-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e839-131">index</span><span class="sxs-lookup"><span data-stu-id="8e839-131">index</span></span>|<span data-ttu-id="8e839-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8e839-132">Int32</span></span>|<span data-ttu-id="8e839-133">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="8e839-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="8e839-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e839-134">Response</span></span>

<span data-ttu-id="8e839-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8e839-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e839-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8e839-136">Example</span></span>
<span data-ttu-id="8e839-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8e839-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e839-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e839-138">Request</span></span>
<span data-ttu-id="8e839-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e839-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="8e839-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e839-140">Response</span></span>
<span data-ttu-id="8e839-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e839-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
