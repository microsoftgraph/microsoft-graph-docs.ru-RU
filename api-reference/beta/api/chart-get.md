---
title: Получение объекта Chart
description: Получение свойств и связей объекта диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2f01860597b5f5dc47bceb87069c1df0f694dfce
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574876"
---
# <a name="get-workbookchart"></a><span data-ttu-id="21fbf-103">Get workbookchart</span><span class="sxs-lookup"><span data-stu-id="21fbf-103">Get workbookchart</span></span>

<span data-ttu-id="21fbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21fbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21fbf-105">Получение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="21fbf-105">Retrieve the properties and relationships of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="21fbf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21fbf-106">Permissions</span></span>
<span data-ttu-id="21fbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21fbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21fbf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21fbf-109">Permission type</span></span>      | <span data-ttu-id="21fbf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21fbf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21fbf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21fbf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="21fbf-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21fbf-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21fbf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21fbf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21fbf-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21fbf-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="21fbf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21fbf-115">Application</span></span> | <span data-ttu-id="21fbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21fbf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21fbf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21fbf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="21fbf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="21fbf-118">Optional query parameters</span></span>
<span data-ttu-id="21fbf-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="21fbf-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21fbf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21fbf-120">Request headers</span></span>
| <span data-ttu-id="21fbf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="21fbf-121">Name</span></span>      |<span data-ttu-id="21fbf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="21fbf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21fbf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21fbf-123">Authorization</span></span>  | <span data-ttu-id="21fbf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21fbf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21fbf-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="21fbf-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="21fbf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="21fbf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21fbf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21fbf-129">Request body</span></span>
<span data-ttu-id="21fbf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21fbf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21fbf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="21fbf-131">Response</span></span>

<span data-ttu-id="21fbf-132">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [книгиChart](../resources/workbookchart.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="21fbf-132">If successful, this method returns a `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21fbf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="21fbf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21fbf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="21fbf-134">Request</span></span>
<span data-ttu-id="21fbf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21fbf-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21fbf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="21fbf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chart"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```
# <a name="c"></a>[<span data-ttu-id="21fbf-137">C#</span><span class="sxs-lookup"><span data-stu-id="21fbf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21fbf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21fbf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21fbf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21fbf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21fbf-140">Java</span><span class="sxs-lookup"><span data-stu-id="21fbf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="21fbf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="21fbf-141">Response</span></span>
<span data-ttu-id="21fbf-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21fbf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Get Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
