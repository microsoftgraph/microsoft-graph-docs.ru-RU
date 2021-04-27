---
title: Get printService
description: Извлечение свойств и связей службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1eb5f1475889e7f1d8b399baa40c739cad018f66
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049886"
---
# <a name="get-printservice"></a><span data-ttu-id="6b4b8-103">Get printService</span><span class="sxs-lookup"><span data-stu-id="6b4b8-103">Get printService</span></span>

<span data-ttu-id="6b4b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b4b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b4b8-105">Извлечение свойств и связей службы печати.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-105">Retrieve the properties and relationships of a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b4b8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b4b8-106">Permissions</span></span>
<span data-ttu-id="6b4b8-107">Для вызова этого API не требуется никаких разрешений, но для использования службы универсальной печати клиент пользователя или клиента приложения должен иметь активную подписку универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="6b4b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b4b8-108">Permission type</span></span> | <span data-ttu-id="6b4b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b4b8-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6b4b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b4b8-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6b4b8-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-111">None.</span></span>|
|<span data-ttu-id="6b4b8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b4b8-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b4b8-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-113">None.</span></span>|
|<span data-ttu-id="6b4b8-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="6b4b8-114">Application</span></span>|<span data-ttu-id="6b4b8-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b4b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b4b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b4b8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6b4b8-117">Optional query parameters</span></span>
<span data-ttu-id="6b4b8-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6b4b8-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6b4b8-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b4b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b4b8-120">Request headers</span></span>
| <span data-ttu-id="6b4b8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6b4b8-121">Name</span></span>      |<span data-ttu-id="6b4b8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6b4b8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b4b8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b4b8-123">Authorization</span></span> | <span data-ttu-id="6b4b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b4b8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b4b8-126">Request body</span></span>
<span data-ttu-id="6b4b8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6b4b8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b4b8-128">Response</span></span>
<span data-ttu-id="6b4b8-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [printService](../resources/printservice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-129">If successful, this method returns a `200 OK` response code and a [printService](../resources/printservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b4b8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6b4b8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b4b8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b4b8-131">Request</span></span>
<span data-ttu-id="6b4b8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b4b8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b4b8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}
```
# <a name="c"></a>[<span data-ttu-id="6b4b8-134">C#</span><span class="sxs-lookup"><span data-stu-id="6b4b8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b4b8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b4b8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b4b8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b4b8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b4b8-137">Java</span><span class="sxs-lookup"><span data-stu-id="6b4b8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b4b8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b4b8-138">Response</span></span>
<span data-ttu-id="6b4b8-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-139">The following is an example of the response.</span></span>
><span data-ttu-id="6b4b8-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


