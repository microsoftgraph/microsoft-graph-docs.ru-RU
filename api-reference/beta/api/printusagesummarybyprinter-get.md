---
title: Получение Принтусажесуммарибипринтер
description: Получение сводки об использовании принтера за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: 71bce2c90d9ade62f5d473e2d0e530767e8092fe
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896164"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="605d4-103">Получение Принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="605d4-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="605d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="605d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="605d4-105">Получение сводки об использовании [принтера](../resources/printer.md)за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="605d4-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="605d4-106">Описания каждой из конечных точек приведены в разделе [принтусажесуммарибипринтер](../resources/printUsageSummaryByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="605d4-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="605d4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="605d4-107">Permissions</span></span>
<span data-ttu-id="605d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="605d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="605d4-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="605d4-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="605d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="605d4-111">Permission type</span></span> | <span data-ttu-id="605d4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="605d4-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="605d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="605d4-113">Delegated (work or school account)</span></span>| <span data-ttu-id="605d4-114">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="605d4-114">Users.Read.All</span></span> |
|<span data-ttu-id="605d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="605d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="605d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="605d4-116">Not Supported.</span></span>|
|<span data-ttu-id="605d4-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="605d4-117">Application</span></span>|<span data-ttu-id="605d4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="605d4-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="605d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="605d4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monhtlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="request-headers"></a><span data-ttu-id="605d4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="605d4-120">Request headers</span></span>
| <span data-ttu-id="605d4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="605d4-121">Name</span></span>      |<span data-ttu-id="605d4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="605d4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="605d4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="605d4-123">Authorization</span></span> | <span data-ttu-id="605d4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="605d4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="605d4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="605d4-126">Request body</span></span>
<span data-ttu-id="605d4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="605d4-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="605d4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="605d4-128">Response</span></span>
<span data-ttu-id="605d4-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтусажесуммарибипринтер](../resources/printusagesummarybyprinter.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="605d4-129">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="605d4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="605d4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="605d4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="605d4-131">Request</span></span>
<span data-ttu-id="605d4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="605d4-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
##### <a name="response"></a><span data-ttu-id="605d4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="605d4-133">Response</span></span>
<span data-ttu-id="605d4-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="605d4-134">The following is an example of the response.</span></span>
><span data-ttu-id="605d4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="605d4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
    "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
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
  "description": "Get printUsageSummaryByPrinter",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->