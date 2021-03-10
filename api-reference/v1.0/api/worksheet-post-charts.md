---
title: Создание объекта Chart
description: С помощью этого API можно создать объект Chart.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4f5715ca356b50be73f85d7100c3a3c9357a8242
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578313"
---
# <a name="create-chart"></a><span data-ttu-id="f640f-103">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="f640f-103">Create Chart</span></span>

<span data-ttu-id="f640f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f640f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f640f-105">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="f640f-105">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="f640f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f640f-106">Permissions</span></span>
<span data-ttu-id="f640f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f640f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f640f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f640f-109">Permission type</span></span>      | <span data-ttu-id="f640f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f640f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f640f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f640f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f640f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f640f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f640f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f640f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f640f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f640f-114">Not supported.</span></span>    |
|<span data-ttu-id="f640f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f640f-115">Application</span></span> | <span data-ttu-id="f640f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f640f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f640f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f640f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="f640f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f640f-118">Request headers</span></span>
| <span data-ttu-id="f640f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f640f-119">Name</span></span>       | <span data-ttu-id="f640f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f640f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f640f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f640f-121">Authorization</span></span>  | <span data-ttu-id="f640f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f640f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f640f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f640f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f640f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f640f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f640f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f640f-127">Request body</span></span>
<span data-ttu-id="f640f-128">В теле запроса поставляем JSON-представление объекта [WorkbookChart.](../resources/chart.md)</span><span class="sxs-lookup"><span data-stu-id="f640f-128">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f640f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f640f-129">Response</span></span>

<span data-ttu-id="f640f-130">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WorkbookChart](../resources/chart.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f640f-130">If successful, this method returns `201 Created` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f640f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f640f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f640f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f640f-132">Request</span></span>
<span data-ttu-id="f640f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f640f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f640f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f640f-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f640f-135">C#</span><span class="sxs-lookup"><span data-stu-id="f640f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f640f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f640f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f640f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f640f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f640f-138">Java</span><span class="sxs-lookup"><span data-stu-id="f640f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chart-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f640f-139">В теле запроса поставляем JSON-представление объекта [WorkbookChart.](../resources/chart.md)</span><span class="sxs-lookup"><span data-stu-id="f640f-139">In the request body, supply a JSON representation of [WorkbookChart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f640f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f640f-140">Response</span></span>
<span data-ttu-id="f640f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f640f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

