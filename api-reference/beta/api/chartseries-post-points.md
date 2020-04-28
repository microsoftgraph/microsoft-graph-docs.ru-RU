---
title: Создание объекта ChartPoints
description: С помощью этого API можно создать объект ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5a3ad794a34b1f6f3d60033a9e062bcb9982470b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438920"
---
# <a name="create-chartpoint"></a><span data-ttu-id="ae438-103">Создание ChartPoint</span><span class="sxs-lookup"><span data-stu-id="ae438-103">Create ChartPoint</span></span>

<span data-ttu-id="ae438-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae438-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae438-105">Используйте этот API для создания нового ChartPoint.</span><span class="sxs-lookup"><span data-stu-id="ae438-105">Use this API to create a new ChartPoint.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae438-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae438-106">Permissions</span></span>
<span data-ttu-id="ae438-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae438-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae438-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae438-109">Permission type</span></span>      | <span data-ttu-id="ae438-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae438-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae438-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae438-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae438-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae438-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae438-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae438-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae438-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae438-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae438-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae438-115">Application</span></span> | <span data-ttu-id="ae438-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae438-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae438-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae438-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points

```
## <a name="request-headers"></a><span data-ttu-id="ae438-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae438-118">Request headers</span></span>
| <span data-ttu-id="ae438-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ae438-119">Name</span></span>       | <span data-ttu-id="ae438-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae438-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae438-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae438-121">Authorization</span></span>  | <span data-ttu-id="ae438-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae438-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae438-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ae438-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ae438-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ae438-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae438-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae438-127">Request body</span></span>
<span data-ttu-id="ae438-128">В тексте запроса добавьте представление объекта [воркбукчартпоинт](../resources/workbookchartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae438-128">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae438-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae438-129">Response</span></span>

<span data-ttu-id="ae438-130">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбукчартпоинт](../resources/workbookchartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae438-130">If successful, this method returns `201 Created` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae438-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ae438-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae438-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae438-132">Request</span></span>
<span data-ttu-id="ae438-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae438-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae438-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae438-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
Content-type: application/json
Content-length: 3

{
}
```
# <a name="c"></a>[<span data-ttu-id="ae438-135">C#</span><span class="sxs-lookup"><span data-stu-id="ae438-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae438-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae438-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae438-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae438-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ae438-138">В тексте запроса добавьте представление объекта [воркбукчартпоинт](../resources/workbookchartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae438-138">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ae438-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae438-139">Response</span></span>
<span data-ttu-id="ae438-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae438-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
