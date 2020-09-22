---
title: Создание объекта Chart
description: С помощью этого API можно создать объект Chart.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e1c11cfc8c5c0876a01719c230ff03e1666396e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024691"
---
# <a name="create-chart"></a><span data-ttu-id="71e08-103">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="71e08-103">Create Chart</span></span>

<span data-ttu-id="71e08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71e08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71e08-105">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="71e08-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="71e08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71e08-106">Permissions</span></span>
<span data-ttu-id="71e08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71e08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71e08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71e08-109">Permission type</span></span>      | <span data-ttu-id="71e08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71e08-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71e08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71e08-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71e08-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71e08-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71e08-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71e08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71e08-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71e08-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71e08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71e08-115">Application</span></span> | <span data-ttu-id="71e08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71e08-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71e08-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71e08-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="71e08-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71e08-118">Request headers</span></span>
| <span data-ttu-id="71e08-119">Имя</span><span class="sxs-lookup"><span data-stu-id="71e08-119">Name</span></span>       | <span data-ttu-id="71e08-120">Описание</span><span class="sxs-lookup"><span data-stu-id="71e08-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71e08-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71e08-121">Authorization</span></span>  | <span data-ttu-id="71e08-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71e08-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71e08-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71e08-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="71e08-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="71e08-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71e08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71e08-127">Request body</span></span>
<span data-ttu-id="71e08-128">В тексте запроса добавьте представление объекта [воркбукчарт](../resources/workbookchart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71e08-128">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71e08-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e08-129">Response</span></span>

<span data-ttu-id="71e08-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [воркбукчарт](../resources/workbookchart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71e08-130">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71e08-131">Пример</span><span class="sxs-lookup"><span data-stu-id="71e08-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71e08-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71e08-132">Request</span></span>
<span data-ttu-id="71e08-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71e08-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71e08-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="71e08-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
# <a name="c"></a>[<span data-ttu-id="71e08-135">C#</span><span class="sxs-lookup"><span data-stu-id="71e08-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71e08-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71e08-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71e08-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71e08-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="71e08-138">В тексте запроса добавьте представление объекта [воркбукчарт](../resources/workbookchart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71e08-138">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71e08-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e08-139">Response</span></span>
<span data-ttu-id="71e08-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71e08-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


