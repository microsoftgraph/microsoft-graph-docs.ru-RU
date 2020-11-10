---
title: Получение Принтсервице
description: Получение свойств и связей службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2735e019d4e861bb0a2fc066f3c4796011745d9b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968217"
---
# <a name="get-printservice"></a><span data-ttu-id="993e3-103">Получение Принтсервице</span><span class="sxs-lookup"><span data-stu-id="993e3-103">Get printService</span></span>

<span data-ttu-id="993e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="993e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="993e3-105">Получение свойств и связей службы печати.</span><span class="sxs-lookup"><span data-stu-id="993e3-105">Retrieve the properties and relationships of a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="993e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="993e3-106">Permissions</span></span>
<span data-ttu-id="993e3-107">Для вызова этого API не требуется никаких разрешений, но чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="993e3-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="993e3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="993e3-108">Permission type</span></span> | <span data-ttu-id="993e3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="993e3-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="993e3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="993e3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="993e3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="993e3-111">None.</span></span>|
|<span data-ttu-id="993e3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="993e3-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="993e3-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="993e3-113">None.</span></span>|
|<span data-ttu-id="993e3-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="993e3-114">Application</span></span>|<span data-ttu-id="993e3-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="993e3-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="993e3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="993e3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="993e3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="993e3-117">Optional query parameters</span></span>
<span data-ttu-id="993e3-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="993e3-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="993e3-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="993e3-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="993e3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="993e3-120">Request headers</span></span>
| <span data-ttu-id="993e3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="993e3-121">Name</span></span>      |<span data-ttu-id="993e3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="993e3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="993e3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="993e3-123">Authorization</span></span> | <span data-ttu-id="993e3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="993e3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="993e3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="993e3-126">Request body</span></span>
<span data-ttu-id="993e3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="993e3-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="993e3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="993e3-128">Response</span></span>
<span data-ttu-id="993e3-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтсервице](../resources/printservice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="993e3-129">If successful, this method returns a `200 OK` response code and a [printService](../resources/printservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="993e3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="993e3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="993e3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="993e3-131">Request</span></span>
<span data-ttu-id="993e3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="993e3-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="993e3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="993e3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}
```
# <a name="c"></a>[<span data-ttu-id="993e3-134">C#</span><span class="sxs-lookup"><span data-stu-id="993e3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="993e3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="993e3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="993e3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="993e3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="993e3-137">Java</span><span class="sxs-lookup"><span data-stu-id="993e3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="993e3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="993e3-138">Response</span></span>
<span data-ttu-id="993e3-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="993e3-139">The following is an example of the response.</span></span>
><span data-ttu-id="993e3-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="993e3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 332

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services/$entity",
  "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
  "endpoints": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


