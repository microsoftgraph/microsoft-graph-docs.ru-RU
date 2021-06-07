---
title: 'отчеты: getPrinterArchivedPrintJobs'
description: Получите список архивных заданий печати, которые стояли в очереди для определенного принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8c779775284a98ae5e68a6b57bb773c7a1753264
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780976"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="bd5f2-103">отчеты: getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="bd5f2-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="bd5f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd5f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd5f2-105">Получите список архивных заданий печати, которые стояли в очереди для определенного [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="bd5f2-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd5f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5f2-106">Permissions</span></span>
<span data-ttu-id="bd5f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd5f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bd5f2-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="bd5f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5f2-110">Permission type</span></span> | <span data-ttu-id="bd5f2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd5f2-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bd5f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd5f2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="bd5f2-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd5f2-113">Reports.Read.All</span></span> |
|<span data-ttu-id="bd5f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd5f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd5f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-115">Not Supported.</span></span>|
|<span data-ttu-id="bd5f2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bd5f2-116">Application</span></span>|<span data-ttu-id="bd5f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd5f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd5f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="bd5f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd5f2-119">Request headers</span></span>
| <span data-ttu-id="bd5f2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bd5f2-120">Name</span></span>          | <span data-ttu-id="bd5f2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5f2-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd5f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd5f2-122">Authorization</span></span> | <span data-ttu-id="bd5f2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="bd5f2-125">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="bd5f2-125">Function parameters</span></span>

| <span data-ttu-id="bd5f2-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="bd5f2-126">Parameter</span></span>     | <span data-ttu-id="bd5f2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bd5f2-127">Type</span></span>                 | <span data-ttu-id="bd5f2-128">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="bd5f2-128">Required?</span></span> | <span data-ttu-id="bd5f2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5f2-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="bd5f2-130">Да</span><span class="sxs-lookup"><span data-stu-id="bd5f2-130">Yes</span></span>       | <span data-ttu-id="bd5f2-131">ID принтера для возврата данных.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-131">The ID of the printer to return data for.</span></span>                            |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="bd5f2-132">Нет</span><span class="sxs-lookup"><span data-stu-id="bd5f2-132">No</span></span>        | <span data-ttu-id="bd5f2-133">Дата начала (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="bd5f2-134">Нет</span><span class="sxs-lookup"><span data-stu-id="bd5f2-134">No</span></span>        | <span data-ttu-id="bd5f2-135">Дата окончания (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="bd5f2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd5f2-136">Response</span></span>
<span data-ttu-id="bd5f2-137">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd5f2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="bd5f2-138">Example</span></span>
<span data-ttu-id="bd5f2-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bd5f2-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd5f2-140">Request</span></span>
<span data-ttu-id="bd5f2-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)
```

##### <a name="response"></a><span data-ttu-id="bd5f2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd5f2-142">Response</span></span>
<span data-ttu-id="bd5f2-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-143">The following is an example of the response.</span></span>
><span data-ttu-id="bd5f2-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd5f2-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.archivedPrintJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 236

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printer": {
        "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6"
      },
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: getPrinterArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

