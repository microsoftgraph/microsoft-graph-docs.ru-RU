---
title: Создание объекта Chart
description: С помощью этого API можно создать объект Chart.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dd95cd6cbf33379664a0a67d6e8f4d9dd2b18504
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866179"
---
# <a name="create-chart"></a><span data-ttu-id="e4e46-103">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="e4e46-103">Create Chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4e46-104">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="e4e46-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4e46-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4e46-105">Permissions</span></span>
<span data-ttu-id="e4e46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4e46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4e46-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4e46-108">Permission type</span></span>      | <span data-ttu-id="e4e46-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4e46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4e46-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4e46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4e46-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4e46-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4e46-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4e46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4e46-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4e46-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4e46-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4e46-114">Application</span></span> | <span data-ttu-id="e4e46-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4e46-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4e46-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4e46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="e4e46-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4e46-117">Request headers</span></span>
| <span data-ttu-id="e4e46-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e4e46-118">Name</span></span>       | <span data-ttu-id="e4e46-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e4e46-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4e46-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4e46-120">Authorization</span></span>  | <span data-ttu-id="e4e46-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4e46-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4e46-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4e46-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4e46-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e4e46-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4e46-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4e46-126">Request body</span></span>
<span data-ttu-id="e4e46-127">В тексте запроса добавьте представление объекта [воркбукчарт](../resources/workbookchart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4e46-127">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e4e46-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4e46-128">Response</span></span>

<span data-ttu-id="e4e46-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбукчарт](../resources/workbookchart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4e46-129">If successful, this method returns `201 Created` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4e46-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e4e46-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4e46-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4e46-131">Request</span></span>
<span data-ttu-id="e4e46-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4e46-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e4e46-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4e46-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e4e46-134">C#</span><span class="sxs-lookup"><span data-stu-id="e4e46-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chart-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4e46-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4e46-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chart-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e4e46-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e4e46-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chart-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e4e46-137">Java</span><span class="sxs-lookup"><span data-stu-id="e4e46-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chart-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e4e46-138">В тексте запроса добавьте представление объекта [воркбукчарт](../resources/workbookchart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4e46-138">In the request body, supply a JSON representation of [workbookChart](../resources/workbookchart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e4e46-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4e46-139">Response</span></span>
<span data-ttu-id="e4e46-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4e46-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
