---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
ms.openlocfilehash: b6af086e9867ca4c4d61a4102de1d2800163c453
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024458"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="7c4a2-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="7c4a2-104">workbookRangeView: itemAt</span></span>


## <a name="permissions"></a><span data-ttu-id="7c4a2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c4a2-105">Permissions</span></span>
<span data-ttu-id="7c4a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c4a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c4a2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c4a2-108">Permission type</span></span>      | <span data-ttu-id="7c4a2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c4a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c4a2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c4a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c4a2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c4a2-111">Files.ReadWrite</span></span> |
|<span data-ttu-id="7c4a2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c4a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c4a2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-113">Not supported.</span></span>    |
|<span data-ttu-id="7c4a2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c4a2-114">Application</span></span> | <span data-ttu-id="7c4a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c4a2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c4a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="7c4a2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c4a2-117">Request headers</span></span>
| <span data-ttu-id="7c4a2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7c4a2-118">Name</span></span>       | <span data-ttu-id="7c4a2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7c4a2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c4a2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c4a2-120">Authorization</span></span>  | <span data-ttu-id="7c4a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c4a2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c4a2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c4a2-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="7c4a2-126">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="7c4a2-126">Function parameters</span></span>
<span data-ttu-id="7c4a2-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="7c4a2-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="7c4a2-128">Parameter</span></span>    | <span data-ttu-id="7c4a2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7c4a2-129">Type</span></span>   |<span data-ttu-id="7c4a2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7c4a2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c4a2-131">index</span><span class="sxs-lookup"><span data-stu-id="7c4a2-131">index</span></span>|<span data-ttu-id="7c4a2-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7c4a2-132">Int32</span></span>|<span data-ttu-id="7c4a2-133">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="7c4a2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c4a2-134">Response</span></span>

<span data-ttu-id="7c4a2-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c4a2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="7c4a2-136">Example</span></span>
<span data-ttu-id="7c4a2-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c4a2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c4a2-138">Request</span></span>
<span data-ttu-id="7c4a2-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c4a2-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="7c4a2-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c4a2-140">Response</span></span>
<span data-ttu-id="7c4a2-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7c4a2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
