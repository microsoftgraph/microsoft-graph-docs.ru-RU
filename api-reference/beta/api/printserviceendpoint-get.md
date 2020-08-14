---
title: Получение Принтсервицеендпоинт
description: Получение свойств и связей конечной точки службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9a0b57f00f487ec6f939c063ccbefa452212976d
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674157"
---
# <a name="get-printserviceendpoint"></a><span data-ttu-id="0dccc-103">Получение Принтсервицеендпоинт</span><span class="sxs-lookup"><span data-stu-id="0dccc-103">Get printServiceEndpoint</span></span>

<span data-ttu-id="0dccc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dccc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dccc-105">Получение свойств и связей конечной точки службы печати.</span><span class="sxs-lookup"><span data-stu-id="0dccc-105">Retrieve the properties and relationships of a print service endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dccc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0dccc-106">Permissions</span></span>
<span data-ttu-id="0dccc-107">Для вызова этого API не требуется никаких разрешений, но чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="0dccc-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0dccc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0dccc-108">Permission type</span></span> | <span data-ttu-id="0dccc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0dccc-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0dccc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0dccc-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0dccc-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0dccc-111">None.</span></span>|
|<span data-ttu-id="0dccc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0dccc-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dccc-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="0dccc-113">None.</span></span>|
|<span data-ttu-id="0dccc-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="0dccc-114">Application</span></span>|<span data-ttu-id="0dccc-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="0dccc-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dccc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0dccc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints/{name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0dccc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0dccc-117">Optional query parameters</span></span>
<span data-ttu-id="0dccc-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0dccc-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0dccc-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0dccc-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0dccc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0dccc-120">Request headers</span></span>
| <span data-ttu-id="0dccc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0dccc-121">Name</span></span>      |<span data-ttu-id="0dccc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0dccc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0dccc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0dccc-123">Authorization</span></span> | <span data-ttu-id="0dccc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0dccc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dccc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0dccc-126">Request body</span></span>
<span data-ttu-id="0dccc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0dccc-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0dccc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dccc-128">Response</span></span>
<span data-ttu-id="0dccc-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтсервицеендпоинт](../resources/printserviceendpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0dccc-129">If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0dccc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0dccc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0dccc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dccc-131">Request</span></span>
<span data-ttu-id="0dccc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0dccc-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0dccc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dccc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints/{name}
```
# <a name="c"></a>[<span data-ttu-id="0dccc-134">C#</span><span class="sxs-lookup"><span data-stu-id="0dccc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printserviceendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dccc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dccc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printserviceendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dccc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dccc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printserviceendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0dccc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dccc-137">Response</span></span>
<span data-ttu-id="0dccc-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0dccc-138">The following is an example of the response.</span></span>
><span data-ttu-id="0dccc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0dccc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
