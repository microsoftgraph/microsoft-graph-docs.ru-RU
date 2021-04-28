---
title: Создание объекта Chart
description: С помощью этого API можно создать объект Chart.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: af852d0f1794906af3f95c55f4e0d7e054753f94
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055626"
---
# <a name="create-chart"></a><span data-ttu-id="c5094-103">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="c5094-103">Create Chart</span></span>

<span data-ttu-id="c5094-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5094-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5094-105">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="c5094-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5094-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5094-106">Permissions</span></span>
<span data-ttu-id="c5094-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5094-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5094-109">Permission type</span></span>      | <span data-ttu-id="c5094-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5094-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5094-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5094-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5094-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5094-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5094-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5094-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5094-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5094-114">Not supported.</span></span>    |
|<span data-ttu-id="c5094-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5094-115">Application</span></span> | <span data-ttu-id="c5094-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5094-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5094-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5094-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="c5094-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5094-118">Request headers</span></span>
| <span data-ttu-id="c5094-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c5094-119">Name</span></span>       | <span data-ttu-id="c5094-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c5094-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5094-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5094-121">Authorization</span></span>  | <span data-ttu-id="c5094-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5094-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5094-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5094-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5094-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c5094-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5094-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5094-127">Request body</span></span>
<span data-ttu-id="c5094-128">В теле запроса поставляем JSON-представление объекта [WorkbookChart.](../resources/chart.md)</span><span class="sxs-lookup"><span data-stu-id="c5094-128">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c5094-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5094-129">Response</span></span>

<span data-ttu-id="c5094-130">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WorkbookChart](../resources/chart.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c5094-130">If successful, this method returns `201 Created` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5094-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c5094-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5094-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5094-132">Request</span></span>
<span data-ttu-id="c5094-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5094-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5094-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5094-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
# <a name="c"></a>[<span data-ttu-id="c5094-135">C#</span><span class="sxs-lookup"><span data-stu-id="c5094-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5094-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5094-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5094-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5094-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5094-138">Java</span><span class="sxs-lookup"><span data-stu-id="c5094-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chart-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c5094-139">В теле запроса поставляем JSON-представление объекта [WorkbookChart.](../resources/chart.md)</span><span class="sxs-lookup"><span data-stu-id="c5094-139">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c5094-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5094-140">Response</span></span>
<span data-ttu-id="c5094-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5094-141">Here is an example of the response.</span></span> <span data-ttu-id="c5094-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c5094-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

