---
title: Обновление объекта ChartTitle
description: Обновление свойств объекта charttitle.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 010df5d61d3275e7dd6b89494991a1bd432f51e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438703"
---
# <a name="update-charttitle"></a><span data-ttu-id="3374e-103">Обновление объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="3374e-103">Update charttitle</span></span>

<span data-ttu-id="3374e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3374e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3374e-105">Обновление свойств объекта charttitle.</span><span class="sxs-lookup"><span data-stu-id="3374e-105">Update the properties of charttitle object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3374e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3374e-106">Permissions</span></span>
<span data-ttu-id="3374e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3374e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3374e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3374e-109">Permission type</span></span>      | <span data-ttu-id="3374e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3374e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3374e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3374e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3374e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3374e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3374e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3374e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3374e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3374e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3374e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3374e-115">Application</span></span> | <span data-ttu-id="3374e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3374e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3374e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3374e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/title
```
## <a name="optional-request-headers"></a><span data-ttu-id="3374e-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3374e-118">Optional request headers</span></span>
| <span data-ttu-id="3374e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3374e-119">Name</span></span>       | <span data-ttu-id="3374e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3374e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3374e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3374e-121">Authorization</span></span>  | <span data-ttu-id="3374e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3374e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3374e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3374e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3374e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3374e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3374e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3374e-127">Request body</span></span>
<span data-ttu-id="3374e-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3374e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3374e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="3374e-131">Property</span></span>     | <span data-ttu-id="3374e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3374e-132">Type</span></span>   |<span data-ttu-id="3374e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3374e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3374e-134">overlay</span><span class="sxs-lookup"><span data-stu-id="3374e-134">overlay</span></span>|<span data-ttu-id="3374e-135">boolean</span><span class="sxs-lookup"><span data-stu-id="3374e-135">boolean</span></span>|<span data-ttu-id="3374e-136">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="3374e-136">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="3374e-137">text</span><span class="sxs-lookup"><span data-stu-id="3374e-137">text</span></span>|<span data-ttu-id="3374e-138">string</span><span class="sxs-lookup"><span data-stu-id="3374e-138">string</span></span>|<span data-ttu-id="3374e-139">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3374e-139">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="3374e-140">visible</span><span class="sxs-lookup"><span data-stu-id="3374e-140">visible</span></span>|<span data-ttu-id="3374e-141">boolean</span><span class="sxs-lookup"><span data-stu-id="3374e-141">boolean</span></span>|<span data-ttu-id="3374e-142">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3374e-142">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="response"></a><span data-ttu-id="3374e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3374e-143">Response</span></span>

<span data-ttu-id="3374e-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркбукчарттитле](../resources/workbookcharttitle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3374e-144">If successful, this method returns a `200 OK` response code and updated [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3374e-145">Пример</span><span class="sxs-lookup"><span data-stu-id="3374e-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3374e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="3374e-146">Request</span></span>
<span data-ttu-id="3374e-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3374e-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3374e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="3374e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_charttitle"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```
# <a name="c"></a>[<span data-ttu-id="3374e-149">C#</span><span class="sxs-lookup"><span data-stu-id="3374e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-charttitle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3374e-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3374e-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-charttitle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3374e-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3374e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-charttitle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3374e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3374e-152">Response</span></span>
<span data-ttu-id="3374e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3374e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartTitle"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "overlay": true,
  "text": "text-value",
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update charttitle",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
