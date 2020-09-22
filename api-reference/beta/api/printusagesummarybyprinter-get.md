---
title: Получение Принтусажесуммарибипринтер
description: Получение сводки об использовании принтера за определенный период времени.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
ms.date: 2/4/2020
doc_type: apiPageType
ms.openlocfilehash: 54b62ecab5016970f5c9e3034207e38e13fcef92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035235"
---
# <a name="get-printusagesummarybyprinter"></a><span data-ttu-id="ca087-103">Получение Принтусажесуммарибипринтер</span><span class="sxs-lookup"><span data-stu-id="ca087-103">Get printUsageSummaryByPrinter</span></span>

<span data-ttu-id="ca087-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca087-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca087-105">Получение сводки об использовании [принтера](../resources/printer.md)за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="ca087-105">Retrieve a [printer](../resources/printer.md)'s usage summary for a particular time period.</span></span> <span data-ttu-id="ca087-106">Описания каждой из конечных точек приведены в разделе [принтусажесуммарибипринтер](../resources/printUsageSummaryByPrinter.md).</span><span class="sxs-lookup"><span data-stu-id="ca087-106">For descriptions of each of the endpoints, see [printUsageSummaryByPrinter](../resources/printUsageSummaryByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca087-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca087-107">Permissions</span></span>
<span data-ttu-id="ca087-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca087-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ca087-110">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ca087-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="ca087-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca087-111">Permission type</span></span> | <span data-ttu-id="ca087-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca087-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ca087-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca087-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ca087-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="ca087-114">User.Read</span></span> |
|<span data-ttu-id="ca087-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca087-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca087-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca087-116">Not Supported.</span></span>|
|<span data-ttu-id="ca087-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca087-117">Application</span></span>|<span data-ttu-id="ca087-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca087-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca087-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca087-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByPrinter/{id}
GET /reports/monhtlyPrintUsageSummariesByPrinter/{id}
GET /print/reports/dailyPrintUsageSummariesByPrinter/{id}
GET /print/reports/monthlyPrintUsageSummariesByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca087-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca087-120">Optional query parameters</span></span>
<span data-ttu-id="ca087-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ca087-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ca087-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ca087-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca087-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca087-123">Request headers</span></span>
| <span data-ttu-id="ca087-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ca087-124">Name</span></span>      |<span data-ttu-id="ca087-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ca087-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca087-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca087-126">Authorization</span></span> | <span data-ttu-id="ca087-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca087-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca087-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca087-129">Request body</span></span>
<span data-ttu-id="ca087-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca087-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ca087-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca087-131">Response</span></span>
<span data-ttu-id="ca087-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтусажесуммарибипринтер](../resources/printusagesummarybyprinter.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca087-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByPrinter](../resources/printusagesummarybyprinter.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca087-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ca087-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca087-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca087-134">Request</span></span>
<span data-ttu-id="ca087-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca087-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByPrinter"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByPrinter/{id}
```
##### <a name="response"></a><span data-ttu-id="ca087-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca087-136">Response</span></span>
<span data-ttu-id="ca087-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca087-137">The following is an example of the response.</span></span>
><span data-ttu-id="ca087-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca087-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

