---
title: 'workbookRangeView: itemAt'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
ms.openlocfilehash: 2fc5c638bbe55f3209d629415023ece7d81e6c29
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834778"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="250fd-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="250fd-104">workbookRangeView: itemAt</span></span>

> <span data-ttu-id="250fd-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="250fd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="250fd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="250fd-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="250fd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="250fd-107">Permissions</span></span>
<span data-ttu-id="250fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="250fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="250fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="250fd-110">Permission type</span></span>      | <span data-ttu-id="250fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="250fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="250fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="250fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="250fd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="250fd-113">Not supported.</span></span>    |
|<span data-ttu-id="250fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="250fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="250fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="250fd-115">Not supported.</span></span>    |
|<span data-ttu-id="250fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="250fd-116">Application</span></span> | <span data-ttu-id="250fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="250fd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="250fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="250fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="250fd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="250fd-119">Request headers</span></span>
| <span data-ttu-id="250fd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="250fd-120">Name</span></span>       | <span data-ttu-id="250fd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="250fd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="250fd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="250fd-122">Authorization</span></span>  | <span data-ttu-id="250fd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="250fd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="250fd-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="250fd-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="250fd-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="250fd-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="250fd-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="250fd-128">Request body</span></span>
<span data-ttu-id="250fd-129">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="250fd-129">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="250fd-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="250fd-130">Parameter</span></span>    | <span data-ttu-id="250fd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="250fd-131">Type</span></span>   |<span data-ttu-id="250fd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="250fd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="250fd-133">index</span><span class="sxs-lookup"><span data-stu-id="250fd-133">index</span></span>|<span data-ttu-id="250fd-134">Int32</span><span class="sxs-lookup"><span data-stu-id="250fd-134">Int32</span></span>|<span data-ttu-id="250fd-135">Индекс элемента, который нужно вернуть.</span><span class="sxs-lookup"><span data-stu-id="250fd-135">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="250fd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="250fd-136">Response</span></span>

<span data-ttu-id="250fd-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="250fd-137">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="250fd-138">Пример</span><span class="sxs-lookup"><span data-stu-id="250fd-138">Example</span></span>
<span data-ttu-id="250fd-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="250fd-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="250fd-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="250fd-140">Request</span></span>
<span data-ttu-id="250fd-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="250fd-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="250fd-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="250fd-142">Response</span></span>
<span data-ttu-id="250fd-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="250fd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
