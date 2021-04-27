---
title: Get printServiceEndpoint
description: Извлечение свойств и связей конечной точки службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8e5e26d620d0285686859862c014cf1f2390659d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053603"
---
# <a name="get-printserviceendpoint"></a><span data-ttu-id="8498f-103">Get printServiceEndpoint</span><span class="sxs-lookup"><span data-stu-id="8498f-103">Get printServiceEndpoint</span></span>

<span data-ttu-id="8498f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8498f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8498f-105">Извлечение свойств и связей конечной точки службы печати.</span><span class="sxs-lookup"><span data-stu-id="8498f-105">Retrieve the properties and relationships of a print service endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="8498f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8498f-106">Permissions</span></span>
<span data-ttu-id="8498f-107">Для вызова этого API не требуется никаких разрешений, но для использования службы универсальной печати клиент пользователя или клиента приложения должен иметь активную подписку универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="8498f-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8498f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8498f-108">Permission type</span></span> | <span data-ttu-id="8498f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8498f-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8498f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8498f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8498f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8498f-111">None.</span></span>|
|<span data-ttu-id="8498f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8498f-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8498f-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="8498f-113">None.</span></span>|
|<span data-ttu-id="8498f-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="8498f-114">Application</span></span>|<span data-ttu-id="8498f-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8498f-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8498f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8498f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}/endpoints/{name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8498f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8498f-117">Optional query parameters</span></span>
<span data-ttu-id="8498f-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8498f-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8498f-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8498f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8498f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8498f-120">Request headers</span></span>
| <span data-ttu-id="8498f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8498f-121">Name</span></span>      |<span data-ttu-id="8498f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8498f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8498f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8498f-123">Authorization</span></span> | <span data-ttu-id="8498f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8498f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8498f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8498f-126">Request body</span></span>
<span data-ttu-id="8498f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8498f-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8498f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8498f-128">Response</span></span>
<span data-ttu-id="8498f-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printServiceEndpoint](../resources/printserviceendpoint.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8498f-129">If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8498f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8498f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8498f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8498f-131">Request</span></span>
<span data-ttu-id="8498f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8498f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8498f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8498f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}/endpoints/{name}
```
# <a name="c"></a>[<span data-ttu-id="8498f-134">C#</span><span class="sxs-lookup"><span data-stu-id="8498f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printserviceendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8498f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8498f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printserviceendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8498f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8498f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printserviceendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8498f-137">Java</span><span class="sxs-lookup"><span data-stu-id="8498f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printserviceendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8498f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8498f-138">Response</span></span>
<span data-ttu-id="8498f-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8498f-139">The following is an example of the response.</span></span>
><span data-ttu-id="8498f-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8498f-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


