---
title: Получение printUsageSummaryByUser
description: Извлечение сводки об использовании пользователя за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d4051b0c9a660bfe89125b402598dae418cc5871
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982266"
---
# <a name="get-printusagesummarybyuser"></a><span data-ttu-id="db535-103">Получение printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="db535-103">Get printUsageSummaryByUser</span></span>

<span data-ttu-id="db535-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db535-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db535-105">Получить сводку об использовании пользователя за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="db535-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="db535-106">Описание каждой из конечных точек см. в документации [printUsageSummaryByUser.](../resources/printUsageSummaryByUser.md)</span><span class="sxs-lookup"><span data-stu-id="db535-106">See the [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="db535-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db535-107">Permissions</span></span>
<span data-ttu-id="db535-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db535-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="db535-110">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть активная подписка универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="db535-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="db535-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db535-111">Permission type</span></span> | <span data-ttu-id="db535-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db535-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="db535-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db535-113">Delegated (work or school account)</span></span>| <span data-ttu-id="db535-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="db535-114">Reports.Read.All</span></span> |
|<span data-ttu-id="db535-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db535-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db535-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db535-116">Not Supported.</span></span>|
|<span data-ttu-id="db535-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="db535-117">Application</span></span>|<span data-ttu-id="db535-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db535-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db535-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db535-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser/{id}
GET /reports/monthlyPrintUsageSummariesByUser/{id}
GET /print/reports/dailyPrintUsageSummariesByUser/{id}
GET /print/reports/monthlyPrintUsageSummariesByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db535-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db535-120">Optional query parameters</span></span>
<span data-ttu-id="db535-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="db535-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="db535-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="db535-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="db535-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db535-123">Request headers</span></span>
| <span data-ttu-id="db535-124">Имя</span><span class="sxs-lookup"><span data-stu-id="db535-124">Name</span></span>      |<span data-ttu-id="db535-125">Описание</span><span class="sxs-lookup"><span data-stu-id="db535-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db535-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db535-126">Authorization</span></span> | <span data-ttu-id="db535-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db535-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db535-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db535-129">Request body</span></span>
<span data-ttu-id="db535-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db535-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="db535-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="db535-131">Response</span></span>
<span data-ttu-id="db535-132">В случае успеха этот метод возвращает код отклика и объект `200 OK` [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db535-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db535-133">Пример</span><span class="sxs-lookup"><span data-stu-id="db535-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db535-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="db535-134">Request</span></span>
<span data-ttu-id="db535-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db535-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByUser"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser/{id}
```
##### <a name="response"></a><span data-ttu-id="db535-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db535-136">Response</span></span>
<span data-ttu-id="db535-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db535-137">The following is an example of the response.</span></span>
><span data-ttu-id="db535-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db535-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

