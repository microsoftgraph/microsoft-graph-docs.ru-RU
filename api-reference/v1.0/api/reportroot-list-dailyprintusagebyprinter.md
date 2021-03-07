---
title: Список dailyPrintUsageByPrinter
description: Извлечение списка сводок ежедневного использования печати, сгруппив по принтеру.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 093d1180cacfbbc933fca0f3bc7031085ab5f46a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518089"
---
# <a name="list-dailyprintusagebyprinter"></a><span data-ttu-id="c8941-103">Список dailyPrintUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="c8941-103">List dailyPrintUsageByPrinter</span></span>
<span data-ttu-id="c8941-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8941-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c8941-105">Извлечение списка сводок ежедневного использования печати, сгруппив по [принтеру.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="c8941-105">Retrieve a list of daily print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8941-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8941-106">Permissions</span></span>
<span data-ttu-id="c8941-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c8941-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="c8941-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c8941-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8941-110">Permission type</span></span> | <span data-ttu-id="c8941-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8941-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c8941-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8941-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c8941-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8941-113">Reports.Read.All</span></span> |
|<span data-ttu-id="c8941-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8941-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8941-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8941-115">Not Supported.</span></span>|
|<span data-ttu-id="c8941-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8941-116">Application</span></span>|<span data-ttu-id="c8941-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8941-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8941-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8941-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByPrinter
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8941-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8941-119">Optional query parameters</span></span>
<span data-ttu-id="c8941-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c8941-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c8941-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c8941-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8941-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8941-122">Request headers</span></span>
|<span data-ttu-id="c8941-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c8941-123">Name</span></span>|<span data-ttu-id="c8941-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c8941-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c8941-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8941-125">Authorization</span></span>|<span data-ttu-id="c8941-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8941-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8941-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8941-128">Request body</span></span>
<span data-ttu-id="c8941-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8941-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8941-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8941-130">Response</span></span>

<span data-ttu-id="c8941-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printUsageByPrinter](../resources/printusagebyprinter.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8941-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageByPrinter](../resources/printusagebyprinter.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8941-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8941-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8941-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8941-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByPrinter
```


### <a name="response"></a><span data-ttu-id="c8941-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8941-134">Response</span></span>
<span data-ttu-id="c8941-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8941-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printUsageByPrinter)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

