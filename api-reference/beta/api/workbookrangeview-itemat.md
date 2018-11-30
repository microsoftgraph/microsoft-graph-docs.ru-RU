---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
ms.openlocfilehash: c19a2480202b1528a1d09ffd6151835a357c14ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078740"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="631d8-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="631d8-104">workbookRangeView: itemAt</span></span>

> <span data-ttu-id="631d8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="631d8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="631d8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631d8-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="631d8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="631d8-107">Permissions</span></span>
<span data-ttu-id="631d8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="631d8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="631d8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="631d8-110">Permission type</span></span>      | <span data-ttu-id="631d8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="631d8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="631d8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="631d8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="631d8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631d8-113">Not supported.</span></span>    |
|<span data-ttu-id="631d8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="631d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="631d8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631d8-115">Not supported.</span></span>    |
|<span data-ttu-id="631d8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="631d8-116">Application</span></span> | <span data-ttu-id="631d8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631d8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="631d8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="631d8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="631d8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="631d8-119">Request headers</span></span>
| <span data-ttu-id="631d8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="631d8-120">Name</span></span>       | <span data-ttu-id="631d8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="631d8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="631d8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="631d8-122">Authorization</span></span>  | <span data-ttu-id="631d8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="631d8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="631d8-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="631d8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="631d8-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="631d8-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="631d8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="631d8-128">Request body</span></span>
<span data-ttu-id="631d8-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="631d8-129">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="631d8-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="631d8-130">Parameter</span></span>    | <span data-ttu-id="631d8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="631d8-131">Type</span></span>   |<span data-ttu-id="631d8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="631d8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="631d8-133">index</span><span class="sxs-lookup"><span data-stu-id="631d8-133">index</span></span>|<span data-ttu-id="631d8-134">Int32</span><span class="sxs-lookup"><span data-stu-id="631d8-134">Int32</span></span>|<span data-ttu-id="631d8-135">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="631d8-135">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="631d8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="631d8-136">Response</span></span>

<span data-ttu-id="631d8-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="631d8-137">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="631d8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="631d8-138">Example</span></span>
<span data-ttu-id="631d8-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="631d8-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="631d8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="631d8-140">Request</span></span>
<span data-ttu-id="631d8-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="631d8-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="631d8-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="631d8-142">Response</span></span>
<span data-ttu-id="631d8-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="631d8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
