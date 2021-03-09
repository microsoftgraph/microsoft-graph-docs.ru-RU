---
title: Создание объекта ChartPoints
description: С помощью этого API можно создать объект ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3c9a98f731b58a55b70a27b0d39fd6d0d2b2d240
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574365"
---
# <a name="create-chartpoint"></a><span data-ttu-id="f5e1a-103">Создание ChartPoint</span><span class="sxs-lookup"><span data-stu-id="f5e1a-103">Create ChartPoint</span></span>

<span data-ttu-id="f5e1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5e1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5e1a-105">Используйте этот API для создания нового ChartPoint.</span><span class="sxs-lookup"><span data-stu-id="f5e1a-105">Use this API to create a new ChartPoint.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5e1a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5e1a-106">Permissions</span></span>
<span data-ttu-id="f5e1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5e1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5e1a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5e1a-109">Permission type</span></span>      | <span data-ttu-id="f5e1a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5e1a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5e1a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5e1a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f5e1a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5e1a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5e1a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5e1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5e1a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5e1a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f5e1a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5e1a-115">Application</span></span> | <span data-ttu-id="f5e1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5e1a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5e1a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5e1a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points

```
## <a name="request-headers"></a><span data-ttu-id="f5e1a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5e1a-118">Request headers</span></span>
| <span data-ttu-id="f5e1a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f5e1a-119">Name</span></span>       | <span data-ttu-id="f5e1a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f5e1a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5e1a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5e1a-121">Authorization</span></span>  | <span data-ttu-id="f5e1a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5e1a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5e1a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f5e1a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f5e1a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f5e1a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5e1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5e1a-127">Request body</span></span>
<span data-ttu-id="f5e1a-128">В теле запроса укажи JSON представление [объекта книгиChartPoint.](../resources/workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="f5e1a-128">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f5e1a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5e1a-129">Response</span></span>

<span data-ttu-id="f5e1a-130">В случае успеха этот метод возвращает код отклика и объект `201 Created` [книгиChartPoint](../resources/workbookchartpoint.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f5e1a-130">If successful, this method returns `201 Created` response code and [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5e1a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f5e1a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5e1a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5e1a-132">Request</span></span>
<span data-ttu-id="f5e1a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5e1a-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5e1a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e1a-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f5e1a-135">C#</span><span class="sxs-lookup"><span data-stu-id="f5e1a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartpoints-from-chartseries-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5e1a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5e1a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartpoints-from-chartseries-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5e1a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5e1a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartpoints-from-chartseries-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5e1a-138">Java</span><span class="sxs-lookup"><span data-stu-id="f5e1a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chartpoints-from-chartseries-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f5e1a-139">В теле запроса укажи JSON представление [объекта книгиChartPoint.](../resources/workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="f5e1a-139">In the request body, supply a JSON representation of [workbookChartPoint](../resources/workbookchartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f5e1a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5e1a-140">Response</span></span>
<span data-ttu-id="f5e1a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5e1a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


