---
title: Список диаграмм
description: Получение списка объектов диаграмм.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: eb4454b036f6f69662592c6ca4ca29b490f25108
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577641"
---
# <a name="list-charts"></a><span data-ttu-id="30137-103">Список диаграмм</span><span class="sxs-lookup"><span data-stu-id="30137-103">List charts</span></span>

<span data-ttu-id="30137-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30137-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30137-105">Получение списка объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="30137-105">Retrieve a list of chart objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="30137-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30137-106">Permissions</span></span>
<span data-ttu-id="30137-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30137-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30137-109">Permission type</span></span>      | <span data-ttu-id="30137-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30137-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30137-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30137-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30137-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30137-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30137-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30137-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30137-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30137-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30137-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30137-115">Application</span></span> | <span data-ttu-id="30137-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30137-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30137-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30137-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/charts
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30137-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30137-118">Optional query parameters</span></span>
<span data-ttu-id="30137-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30137-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30137-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30137-120">Request headers</span></span>
| <span data-ttu-id="30137-121">Имя</span><span class="sxs-lookup"><span data-stu-id="30137-121">Name</span></span>      |<span data-ttu-id="30137-122">Описание</span><span class="sxs-lookup"><span data-stu-id="30137-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30137-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30137-123">Authorization</span></span>  | <span data-ttu-id="30137-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30137-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30137-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="30137-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="30137-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="30137-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30137-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30137-129">Request body</span></span>
<span data-ttu-id="30137-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30137-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30137-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="30137-131">Response</span></span>

<span data-ttu-id="30137-132">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` объектов [книгиChart](../resources/workbookchart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30137-132">If successful, this method returns a `200 OK` response code and collection of [workbookChart](../resources/workbookchart.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30137-133">Пример</span><span class="sxs-lookup"><span data-stu-id="30137-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30137-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="30137-134">Request</span></span>
<span data-ttu-id="30137-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30137-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="30137-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="30137-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_charts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
```
# <a name="c"></a>[<span data-ttu-id="30137-137">C#</span><span class="sxs-lookup"><span data-stu-id="30137-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-charts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30137-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30137-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-charts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30137-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30137-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-charts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30137-140">Java</span><span class="sxs-lookup"><span data-stu-id="30137-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-charts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30137-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="30137-141">Response</span></span>
<span data-ttu-id="30137-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30137-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 93

{
  "value": [
    {
      "id": "id-value",
      "height": 99,
      "left": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List charts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
