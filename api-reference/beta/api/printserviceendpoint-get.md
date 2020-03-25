---
title: Получение Принтсервицеендпоинт
description: Получение свойств и связей конечной точки службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bd1a479cb72d6863108770b2e896bb6e8ca7cf21
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947519"
---
# <a name="get-printserviceendpoint"></a><span data-ttu-id="eb6a1-103">Получение Принтсервицеендпоинт</span><span class="sxs-lookup"><span data-stu-id="eb6a1-103">Get printServiceEndpoint</span></span>

<span data-ttu-id="eb6a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb6a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb6a1-105">Получение свойств и связей конечной точки службы печати.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-105">Retrieve the properties and relationships of a print service endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb6a1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb6a1-106">Permissions</span></span>
<span data-ttu-id="eb6a1-107">Для вызова этого API не требуется никаких разрешений, но у клиента пользователя должна быть активная универсальная подписка на печать.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-107">No permissions are needed to call this API, but the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="eb6a1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb6a1-108">Permission type</span></span> | <span data-ttu-id="eb6a1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb6a1-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eb6a1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb6a1-110">Delegated (work or school account)</span></span>|<span data-ttu-id="eb6a1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-111">None.</span></span>|
|<span data-ttu-id="eb6a1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb6a1-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb6a1-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-113">None.</span></span>|
|<span data-ttu-id="eb6a1-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="eb6a1-114">Application</span></span>|<span data-ttu-id="eb6a1-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb6a1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb6a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints/{name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb6a1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb6a1-117">Optional query parameters</span></span>
<span data-ttu-id="eb6a1-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="eb6a1-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eb6a1-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb6a1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb6a1-120">Request headers</span></span>
| <span data-ttu-id="eb6a1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eb6a1-121">Name</span></span>      |<span data-ttu-id="eb6a1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6a1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb6a1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb6a1-123">Authorization</span></span> | <span data-ttu-id="eb6a1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb6a1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb6a1-126">Request body</span></span>
<span data-ttu-id="eb6a1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eb6a1-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb6a1-128">Response</span></span>
<span data-ttu-id="eb6a1-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтсервицеендпоинт](../resources/printserviceendpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-129">If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb6a1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eb6a1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb6a1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb6a1-131">Request</span></span>
<span data-ttu-id="eb6a1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb6a1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6a1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints/{name}
```
# <a name="c"></a>[<span data-ttu-id="eb6a1-134">C#</span><span class="sxs-lookup"><span data-stu-id="eb6a1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printserviceendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb6a1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb6a1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printserviceendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb6a1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb6a1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printserviceendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eb6a1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb6a1-137">Response</span></span>
<span data-ttu-id="eb6a1-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-138">The following is an example of the response.</span></span>
><span data-ttu-id="eb6a1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb6a1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "id": "mpsdiscovery",
  "displayName": "Microsoft Universal Print Discovery Service",
  "uri": "https://discovery.print.microsoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printServiceEndpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
