---
title: PrintServices списка
description: Извлечение списка объектов printService, которые представляют службы, доступные вашему клиенту.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3461665b6d027fdba0ecd88e97af422b4f3865ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051097"
---
# <a name="list-printservices"></a><span data-ttu-id="747a0-103">PrintServices списка</span><span class="sxs-lookup"><span data-stu-id="747a0-103">List printServices</span></span>

<span data-ttu-id="747a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="747a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="747a0-105">Извлечение списка [объектов printService,](../resources/printservice.md) которые представляют **службы,** доступные вашему клиенту.</span><span class="sxs-lookup"><span data-stu-id="747a0-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="747a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="747a0-106">Permissions</span></span>
<span data-ttu-id="747a0-107">Для вызова этого API не требуется никаких разрешений, но для использования службы универсальной печати клиент пользователя или клиента приложения должен иметь активную подписку универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="747a0-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="747a0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="747a0-108">Permission type</span></span> | <span data-ttu-id="747a0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="747a0-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="747a0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="747a0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="747a0-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="747a0-111">None.</span></span>|
|<span data-ttu-id="747a0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="747a0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="747a0-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="747a0-113">None.</span></span>|
|<span data-ttu-id="747a0-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="747a0-114">Application</span></span>|<span data-ttu-id="747a0-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="747a0-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="747a0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="747a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="747a0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="747a0-117">Optional query parameters</span></span>
<span data-ttu-id="747a0-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="747a0-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="747a0-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="747a0-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="747a0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="747a0-120">Request headers</span></span>
| <span data-ttu-id="747a0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="747a0-121">Name</span></span>      |<span data-ttu-id="747a0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="747a0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="747a0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="747a0-123">Authorization</span></span> | <span data-ttu-id="747a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="747a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="747a0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="747a0-126">Request body</span></span>
<span data-ttu-id="747a0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="747a0-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="747a0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="747a0-128">Response</span></span>
<span data-ttu-id="747a0-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printService](../resources/printservice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="747a0-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="747a0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="747a0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="747a0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="747a0-131">Request</span></span>
<span data-ttu-id="747a0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="747a0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="747a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="747a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services
```
# <a name="c"></a>[<span data-ttu-id="747a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="747a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="747a0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="747a0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="747a0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="747a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="747a0-137">Java</span><span class="sxs-lookup"><span data-stu-id="747a0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="747a0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="747a0-138">Response</span></span>
<span data-ttu-id="747a0-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="747a0-139">The following is an example of the response.</span></span>
><span data-ttu-id="747a0-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="747a0-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


