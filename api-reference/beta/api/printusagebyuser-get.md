---
title: Get printUsageByUser
description: Извлечение сводки об использовании пользователя за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ab81ab84a1ff70a0de7fbfb6fce33f83d0260466
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869844"
---
# <a name="get-printusagebyuser"></a><span data-ttu-id="a7e83-103">Get printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="a7e83-103">Get printUsageByUser</span></span>

<span data-ttu-id="a7e83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7e83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7e83-105">Извлечение сводки об использовании пользователя за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="a7e83-105">Retrieve a user's usage summary for a particular time period.</span></span> 

<span data-ttu-id="a7e83-106">См. [документацию printUsageByUser](../resources/printUsageByUser.md) для описаний каждой из конечных точек.</span><span class="sxs-lookup"><span data-stu-id="a7e83-106">See the [printUsageByUser](../resources/printUsageByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7e83-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7e83-107">Permissions</span></span>
<span data-ttu-id="a7e83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a7e83-110">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a7e83-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="a7e83-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7e83-111">Permission type</span></span> | <span data-ttu-id="a7e83-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7e83-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a7e83-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7e83-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a7e83-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7e83-114">Reports.Read.All</span></span> |
|<span data-ttu-id="a7e83-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7e83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7e83-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7e83-116">Not Supported.</span></span>|
|<span data-ttu-id="a7e83-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7e83-117">Application</span></span>|<span data-ttu-id="a7e83-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7e83-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7e83-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7e83-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageByUser/{id}
GET /reports/monthlyPrintUsageByUser/{id}
GET /print/reports/dailyPrintUsageByUser/{id}
GET /print/reports/monthlyPrintUsageByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7e83-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7e83-120">Optional query parameters</span></span>
<span data-ttu-id="a7e83-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a7e83-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a7e83-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a7e83-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7e83-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7e83-123">Request headers</span></span>
| <span data-ttu-id="a7e83-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a7e83-124">Name</span></span>      |<span data-ttu-id="a7e83-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a7e83-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a7e83-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7e83-126">Authorization</span></span> | <span data-ttu-id="a7e83-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7e83-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7e83-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7e83-129">Request body</span></span>
<span data-ttu-id="a7e83-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7e83-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a7e83-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7e83-131">Response</span></span>
<span data-ttu-id="a7e83-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printUsageByUser](../resources/printUsageByUser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7e83-132">If successful, this method returns a `200 OK` response code and a [printUsageByUser](../resources/printUsageByUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7e83-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a7e83-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7e83-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7e83-134">Request</span></span>
<span data-ttu-id="a7e83-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7e83-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7e83-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7e83-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageByUser",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageByUser/016b5565-3bbf-4067-b9ff-4d68167eb1a6
```
# <a name="c"></a>[<span data-ttu-id="a7e83-137">C#</span><span class="sxs-lookup"><span data-stu-id="a7e83-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7e83-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7e83-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7e83-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7e83-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7e83-140">Java</span><span class="sxs-lookup"><span data-stu-id="a7e83-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a7e83-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7e83-141">Response</span></span>
<span data-ttu-id="a7e83-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a7e83-142">The following is an example of the response.</span></span>
><span data-ttu-id="a7e83-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a7e83-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "userPrincipalName": "username@contoso.com",
  "usageDate": "2020-02-04T00:00:00.0000000Z",
  "completedBlackAndWhiteJobCount": 42,
  "completedColorJobCount": 0,
  "incompleteJobCount": 6
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printUsageByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

