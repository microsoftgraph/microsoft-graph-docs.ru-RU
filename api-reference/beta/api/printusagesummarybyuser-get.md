---
title: Получение Принтусажесуммарибюсер
description: Получение сводки об использовании пользователя за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: efeb9a9007fbe09636db266f145a294f12ab4d6e
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896161"
---
# <a name="get-printusagesummarybyuser"></a><span data-ttu-id="a2274-103">Получение Принтусажесуммарибюсер</span><span class="sxs-lookup"><span data-stu-id="a2274-103">Get printUsageSummaryByUser</span></span>

<span data-ttu-id="a2274-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2274-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2274-105">Получение сводки об использовании пользователя за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="a2274-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="a2274-106">Описание каждой из этих конечных точек представлено в документации по [принтусажесуммарибюсер](../resources/printUsageSummaryByUser.md) .</span><span class="sxs-lookup"><span data-stu-id="a2274-106">See the [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2274-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2274-107">Permissions</span></span>
<span data-ttu-id="a2274-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2274-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a2274-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="a2274-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="a2274-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2274-111">Permission type</span></span> | <span data-ttu-id="a2274-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2274-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a2274-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2274-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a2274-114">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a2274-114">Users.Read.All</span></span> |
|<span data-ttu-id="a2274-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2274-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2274-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2274-116">Not Supported.</span></span>|
|<span data-ttu-id="a2274-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a2274-117">Application</span></span>|<span data-ttu-id="a2274-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2274-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2274-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2274-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser/{id}
GET /reports/monthlyPrintUsageSummariesByUser/{id}
GET /print/reports/dailyPrintUsageSummariesByUser/{id}
GET /print/reports/monthlyPrintUsageSummariesByUser/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a2274-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2274-120">Request headers</span></span>
| <span data-ttu-id="a2274-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a2274-121">Name</span></span>      |<span data-ttu-id="a2274-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a2274-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2274-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2274-123">Authorization</span></span> | <span data-ttu-id="a2274-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2274-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2274-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2274-126">Request body</span></span>
<span data-ttu-id="a2274-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2274-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a2274-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2274-128">Response</span></span>
<span data-ttu-id="a2274-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтусажесуммарибюсер](../resources/printusagesummarybyuser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2274-129">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2274-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a2274-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2274-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2274-131">Request</span></span>
<span data-ttu-id="a2274-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2274-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByUser"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser/{id}
```
##### <a name="response"></a><span data-ttu-id="a2274-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2274-133">Response</span></span>
<span data-ttu-id="a2274-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a2274-134">The following is an example of the response.</span></span>
><span data-ttu-id="a2274-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2274-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "userPrincipalName": "username@microsoft.com",
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