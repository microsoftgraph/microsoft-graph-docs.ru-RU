---
title: Получение printUsageSummaryByUser
description: Извлечение сводки об использовании пользователя за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 20cb026334e88dc6113db579be07a9de01dfaaa7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441411"
---
# <a name="get-printusagesummarybyuser"></a><span data-ttu-id="82bca-103">Получение printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="82bca-103">Get printUsageSummaryByUser</span></span>

<span data-ttu-id="82bca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82bca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82bca-105">Извлечение сводки об использовании пользователя за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="82bca-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="82bca-106">Описание каждой из конечных точек см. в документации [printUsageSummaryByUser.](../resources/printUsageSummaryByUser.md)</span><span class="sxs-lookup"><span data-stu-id="82bca-106">See the [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="82bca-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82bca-107">Permissions</span></span>
<span data-ttu-id="82bca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82bca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="82bca-110">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="82bca-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="82bca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82bca-111">Permission type</span></span> | <span data-ttu-id="82bca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82bca-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="82bca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82bca-113">Delegated (work or school account)</span></span>| <span data-ttu-id="82bca-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="82bca-114">Reports.Read.All</span></span> |
|<span data-ttu-id="82bca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82bca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82bca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82bca-116">Not Supported.</span></span>|
|<span data-ttu-id="82bca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="82bca-117">Application</span></span>|<span data-ttu-id="82bca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82bca-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82bca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82bca-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser/{id}
GET /reports/monthlyPrintUsageSummariesByUser/{id}
GET /print/reports/dailyPrintUsageSummariesByUser/{id}
GET /print/reports/monthlyPrintUsageSummariesByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82bca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82bca-120">Optional query parameters</span></span>
<span data-ttu-id="82bca-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="82bca-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="82bca-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="82bca-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="82bca-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82bca-123">Request headers</span></span>
| <span data-ttu-id="82bca-124">Имя</span><span class="sxs-lookup"><span data-stu-id="82bca-124">Name</span></span>      |<span data-ttu-id="82bca-125">Описание</span><span class="sxs-lookup"><span data-stu-id="82bca-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82bca-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82bca-126">Authorization</span></span> | <span data-ttu-id="82bca-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82bca-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82bca-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82bca-129">Request body</span></span>
<span data-ttu-id="82bca-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82bca-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="82bca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="82bca-131">Response</span></span>
<span data-ttu-id="82bca-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printUsageSummaryByUser](../resources/printusagesummarybyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="82bca-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82bca-133">Пример</span><span class="sxs-lookup"><span data-stu-id="82bca-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82bca-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="82bca-134">Request</span></span>
<span data-ttu-id="82bca-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82bca-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82bca-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="82bca-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByUser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser/{id}
```
# <a name="c"></a>[<span data-ttu-id="82bca-137">C#</span><span class="sxs-lookup"><span data-stu-id="82bca-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagesummarybyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82bca-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82bca-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagesummarybyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82bca-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82bca-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagesummarybyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82bca-140">Java</span><span class="sxs-lookup"><span data-stu-id="82bca-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagesummarybyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82bca-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="82bca-141">Response</span></span>
<span data-ttu-id="82bca-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82bca-142">The following is an example of the response.</span></span>
><span data-ttu-id="82bca-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82bca-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
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
  "description": "Get printUsageSummaryByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

