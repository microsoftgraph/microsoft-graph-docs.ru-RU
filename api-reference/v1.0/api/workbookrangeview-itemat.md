---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a8d0426c86b6e2a2bdadb50dfd3fb93c5495b1ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569909"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="b8b70-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="b8b70-104">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="b8b70-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8b70-105">Permissions</span></span>
<span data-ttu-id="b8b70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8b70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b70-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8b70-108">Permission type</span></span>      | <span data-ttu-id="b8b70-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8b70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8b70-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8b70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8b70-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8b70-111">Files.ReadWrite</span></span> |
|<span data-ttu-id="b8b70-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8b70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8b70-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8b70-113">Not supported.</span></span>    |
|<span data-ttu-id="b8b70-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8b70-114">Application</span></span> | <span data-ttu-id="b8b70-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8b70-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8b70-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8b70-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="b8b70-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8b70-117">Request headers</span></span>
| <span data-ttu-id="b8b70-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b8b70-118">Name</span></span>       | <span data-ttu-id="b8b70-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b8b70-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b8b70-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8b70-120">Authorization</span></span>  | <span data-ttu-id="b8b70-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8b70-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8b70-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b8b70-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b8b70-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b8b70-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="b8b70-126">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b8b70-126">Function parameters</span></span>
<span data-ttu-id="b8b70-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="b8b70-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="b8b70-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="b8b70-128">Parameter</span></span>    | <span data-ttu-id="b8b70-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b8b70-129">Type</span></span>   |<span data-ttu-id="b8b70-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b8b70-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8b70-131">index</span><span class="sxs-lookup"><span data-stu-id="b8b70-131">index</span></span>|<span data-ttu-id="b8b70-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b8b70-132">Int32</span></span>|<span data-ttu-id="b8b70-133">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="b8b70-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="b8b70-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8b70-134">Response</span></span>

<span data-ttu-id="b8b70-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b8b70-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8b70-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b8b70-136">Example</span></span>
<span data-ttu-id="b8b70-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b8b70-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b8b70-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8b70-138">Request</span></span>
<span data-ttu-id="b8b70-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8b70-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="b8b70-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8b70-140">Response</span></span>
<span data-ttu-id="b8b70-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8b70-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
