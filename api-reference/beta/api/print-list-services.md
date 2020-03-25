---
title: Получение служб
description: Получение списка объектов Принтсервице, представляющих службы, доступные в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5c211e14d2ec699761a503fa2768eff59b9b0181
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948271"
---
# <a name="list-services"></a><span data-ttu-id="31829-103">Список служб</span><span class="sxs-lookup"><span data-stu-id="31829-103">List services</span></span>

<span data-ttu-id="31829-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31829-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31829-105">Получение списка объектов [принтсервице](../resources/printservice.md) , представляющих **службы** , доступные в клиенте.</span><span class="sxs-lookup"><span data-stu-id="31829-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="31829-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31829-106">Permissions</span></span>
<span data-ttu-id="31829-107">Для вызова этого API не требуется никаких разрешений, но у клиента пользователя должна быть активная универсальная подписка на печать.</span><span class="sxs-lookup"><span data-stu-id="31829-107">No permissions are needed to call this API, but the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="31829-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31829-108">Permission type</span></span> | <span data-ttu-id="31829-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31829-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="31829-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31829-110">Delegated (work or school account)</span></span>|<span data-ttu-id="31829-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="31829-111">None.</span></span>|
|<span data-ttu-id="31829-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31829-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31829-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="31829-113">None.</span></span>|
|<span data-ttu-id="31829-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="31829-114">Application</span></span>|<span data-ttu-id="31829-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="31829-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31829-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31829-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31829-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="31829-117">Optional query parameters</span></span>
<span data-ttu-id="31829-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="31829-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="31829-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="31829-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="31829-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31829-120">Request headers</span></span>
| <span data-ttu-id="31829-121">Имя</span><span class="sxs-lookup"><span data-stu-id="31829-121">Name</span></span>      |<span data-ttu-id="31829-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31829-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31829-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31829-123">Authorization</span></span> | <span data-ttu-id="31829-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31829-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31829-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31829-126">Request body</span></span>
<span data-ttu-id="31829-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31829-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="31829-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="31829-128">Response</span></span>
<span data-ttu-id="31829-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтсервице](../resources/printservice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31829-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31829-130">Пример</span><span class="sxs-lookup"><span data-stu-id="31829-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31829-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="31829-131">Request</span></span>
<span data-ttu-id="31829-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31829-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31829-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="31829-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services
```
# <a name="c"></a>[<span data-ttu-id="31829-134">C#</span><span class="sxs-lookup"><span data-stu-id="31829-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31829-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31829-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31829-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31829-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="31829-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="31829-137">Response</span></span>
<span data-ttu-id="31829-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31829-138">The following is an example of the response.</span></span>
><span data-ttu-id="31829-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31829-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
