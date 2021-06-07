---
title: Get printUsageByUser
description: Извлечение сводки об использовании пользователя за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 53ecf8c004b6d610b4c9bd8cb6552b2f96407cbf
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781289"
---
# <a name="get-printusagebyuser"></a><span data-ttu-id="4ea09-103">Get printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="4ea09-103">Get printUsageByUser</span></span>

<span data-ttu-id="4ea09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea09-105">Извлечение сводки об использовании пользователя за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="4ea09-105">Retrieve a user's usage summary for a particular time period.</span></span> 

<span data-ttu-id="4ea09-106">См. [документацию printUsageByUser](../resources/printUsageByUser.md) для описаний каждой из конечных точек.</span><span class="sxs-lookup"><span data-stu-id="4ea09-106">See the [printUsageByUser](../resources/printUsageByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ea09-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea09-107">Permissions</span></span>
<span data-ttu-id="4ea09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ea09-110">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4ea09-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="4ea09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ea09-111">Permission type</span></span> | <span data-ttu-id="4ea09-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ea09-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4ea09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ea09-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4ea09-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ea09-114">Reports.Read.All</span></span> |
|<span data-ttu-id="4ea09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ea09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ea09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea09-116">Not Supported.</span></span>|
|<span data-ttu-id="4ea09-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ea09-117">Application</span></span>|<span data-ttu-id="4ea09-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea09-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ea09-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageByUser/{id}
GET /reports/monthlyPrintUsageByUser/{id}
GET /print/reports/dailyPrintUsageByUser/{id}
GET /print/reports/monthlyPrintUsageByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ea09-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ea09-120">Optional query parameters</span></span>
<span data-ttu-id="4ea09-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4ea09-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4ea09-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4ea09-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ea09-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ea09-123">Request headers</span></span>
| <span data-ttu-id="4ea09-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4ea09-124">Name</span></span>      |<span data-ttu-id="4ea09-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea09-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ea09-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ea09-126">Authorization</span></span> | <span data-ttu-id="4ea09-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ea09-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ea09-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ea09-129">Request body</span></span>
<span data-ttu-id="4ea09-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ea09-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4ea09-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ea09-131">Response</span></span>
<span data-ttu-id="4ea09-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printUsageByUser](../resources/printUsageByUser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4ea09-132">If successful, this method returns a `200 OK` response code and a [printUsageByUser](../resources/printUsageByUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ea09-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4ea09-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ea09-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ea09-134">Request</span></span>
<span data-ttu-id="4ea09-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ea09-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ea09-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea09-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageByUser",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageByUser/016b5565-3bbf-4067-b9ff-4d68167eb1a6
```
# <a name="c"></a>[<span data-ttu-id="4ea09-137">C#</span><span class="sxs-lookup"><span data-stu-id="4ea09-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagesummarybyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ea09-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ea09-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagesummarybyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ea09-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ea09-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagesummarybyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ea09-140">Java</span><span class="sxs-lookup"><span data-stu-id="4ea09-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagesummarybyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4ea09-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ea09-141">Response</span></span>
<span data-ttu-id="4ea09-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4ea09-142">The following is an example of the response.</span></span>
><span data-ttu-id="4ea09-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4ea09-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

