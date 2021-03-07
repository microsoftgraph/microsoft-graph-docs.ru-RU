---
title: Get printUsageByPrinter
description: Извлечение сводки использования принтера за определенный период времени.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9ba1d8a3e91298b87813a9f335bb72482a743b82
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517553"
---
# <a name="get-printusagebyprinter"></a><span data-ttu-id="b52da-103">Get printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="b52da-103">Get printUsageByPrinter</span></span>
<span data-ttu-id="b52da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b52da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b52da-105">Извлечение сводки об использовании [для принтера](../resources/printer.md) за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="b52da-105">Retrieve a usage summary for a [printer](../resources/printer.md) for a particular time period.</span></span> <span data-ttu-id="b52da-106">Описание каждой из конечных точек см. в [printUsageByPrinter.](../resources/printUsageByPrinter.md)</span><span class="sxs-lookup"><span data-stu-id="b52da-106">For descriptions of each of the endpoints, see [printUsageByPrinter](../resources/printUsageByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b52da-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b52da-107">Permissions</span></span>
<span data-ttu-id="b52da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b52da-110">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b52da-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="b52da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b52da-111">Permission type</span></span> | <span data-ttu-id="b52da-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b52da-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b52da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b52da-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b52da-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b52da-114">Reports.Read.All</span></span> |
|<span data-ttu-id="b52da-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b52da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b52da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52da-116">Not Supported.</span></span>|
|<span data-ttu-id="b52da-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b52da-117">Application</span></span>|<span data-ttu-id="b52da-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52da-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b52da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b52da-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByPrinter/{id}
GET /reports/monthlyPrintUsageByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b52da-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b52da-120">Optional query parameters</span></span>
<span data-ttu-id="b52da-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b52da-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b52da-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b52da-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b52da-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b52da-123">Request headers</span></span>
|<span data-ttu-id="b52da-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b52da-124">Name</span></span>|<span data-ttu-id="b52da-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b52da-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b52da-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b52da-126">Authorization</span></span>|<span data-ttu-id="b52da-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b52da-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b52da-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b52da-129">Request body</span></span>
<span data-ttu-id="b52da-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b52da-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b52da-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52da-131">Response</span></span>

<span data-ttu-id="b52da-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printUsageByPrinter](../resources/printusagebyprinter.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b52da-132">If successful, this method returns a `200 OK` response code and a [printUsageByPrinter](../resources/printusagebyprinter.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b52da-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="b52da-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b52da-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b52da-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByPrinter/{id}
```


### <a name="response"></a><span data-ttu-id="b52da-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52da-135">Response</span></span>
<span data-ttu-id="b52da-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b52da-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByPrinter"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "usageDate": "Date",
    "completedBlackAndWhiteJobCount": 42,
    "completedColorJobCount": 0,
    "incompleteJobCount": 6
}
```

