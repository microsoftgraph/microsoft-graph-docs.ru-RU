---
title: 'отчеты: getPrinterArchivedPrintJobs'
description: Получите список архивных заданий печати, которые стояли в очереди для определенного принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7e5788016efded3975fe77f4028ecd48b6bbde54
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517993"
---
# <a name="reportroot-getprinterarchivedprintjobs"></a><span data-ttu-id="0c0e2-103">reportRoot: getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="0c0e2-103">reportRoot: getPrinterArchivedPrintJobs</span></span>
<span data-ttu-id="0c0e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c0e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0c0e2-105">Получите список архивных заданий печати, которые стояли в очереди для определенного [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="0c0e2-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c0e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c0e2-106">Permissions</span></span>
<span data-ttu-id="0c0e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c0e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0c0e2-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0c0e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c0e2-110">Permission type</span></span> | <span data-ttu-id="0c0e2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c0e2-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0c0e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c0e2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0c0e2-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c0e2-113">Reports.Read.All</span></span> |
|<span data-ttu-id="0c0e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c0e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c0e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-115">Not Supported.</span></span>|
|<span data-ttu-id="0c0e2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c0e2-116">Application</span></span>|<span data-ttu-id="0c0e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c0e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c0e2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getPrinterArchivedPrintJobs
```

## <a name="function-parameters"></a><span data-ttu-id="0c0e2-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0c0e2-119">Function parameters</span></span>

| <span data-ttu-id="0c0e2-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c0e2-120">Parameter</span></span>     | <span data-ttu-id="0c0e2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0c0e2-121">Type</span></span>                 | <span data-ttu-id="0c0e2-122">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="0c0e2-122">Required?</span></span> | <span data-ttu-id="0c0e2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0c0e2-123">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="0c0e2-124">Да</span><span class="sxs-lookup"><span data-stu-id="0c0e2-124">Yes</span></span>       | <span data-ttu-id="0c0e2-125">ID принтера для возврата данных.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-125">The ID of the printer to return data for.</span></span>                            |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="0c0e2-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0c0e2-126">No</span></span>        | <span data-ttu-id="0c0e2-127">Дата начала (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-127">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="0c0e2-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0c0e2-128">No</span></span>        | <span data-ttu-id="0c0e2-129">Дата окончания (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-129">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="request-headers"></a><span data-ttu-id="0c0e2-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c0e2-130">Request headers</span></span>
|<span data-ttu-id="0c0e2-131">Имя</span><span class="sxs-lookup"><span data-stu-id="0c0e2-131">Name</span></span>|<span data-ttu-id="0c0e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c0e2-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0c0e2-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c0e2-133">Authorization</span></span>|<span data-ttu-id="0c0e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c0e2-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c0e2-136">Request body</span></span>
<span data-ttu-id="0c0e2-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c0e2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c0e2-138">Response</span></span>

<span data-ttu-id="0c0e2-139">В случае успешной работы эта функция возвращает код ответа и коллекцию `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-139">If successful, this function returns a `200 OK` response code and a [archivedPrintJob](../resources/archivedprintjob.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c0e2-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="0c0e2-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c0e2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c0e2-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getprinterarchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getPrinterArchivedPrintJobs(printerId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
```


### <a name="response"></a><span data-ttu-id="0c0e2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c0e2-142">Response</span></span>
<span data-ttu-id="0c0e2-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0c0e2-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.archivedPrintJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "fe6ff85a-f0d3-4c4f-aec6-b9d5154356a1",
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

