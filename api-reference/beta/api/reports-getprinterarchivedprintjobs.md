---
title: 'отчеты: Жетпринтерарчиведпринтжобс'
description: Получение списка архивированных заданий печати, которые были поставлены в очередь для определенного принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a6ff5b6d9031c142821728b31cb66f8b0c5d100f
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845472"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="2d9e5-103">отчеты: Жетпринтерарчиведпринтжобс</span><span class="sxs-lookup"><span data-stu-id="2d9e5-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="2d9e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d9e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d9e5-105">Получение списка архивированных заданий печати, которые были поставлены в очередь для определенного [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="2d9e5-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d9e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9e5-106">Permissions</span></span>
<span data-ttu-id="2d9e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d9e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2d9e5-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="2d9e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9e5-110">Permission type</span></span> | <span data-ttu-id="2d9e5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d9e5-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2d9e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d9e5-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2d9e5-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="2d9e5-113">Users.Read.All</span></span> |
|<span data-ttu-id="2d9e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d9e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d9e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-115">Not Supported.</span></span>|
|<span data-ttu-id="2d9e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d9e5-116">Application</span></span>|<span data-ttu-id="2d9e5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d9e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d9e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs
GET /reports/getPrinterArchivedPrintJobs
```
## <a name="request-headers"></a><span data-ttu-id="2d9e5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d9e5-119">Request headers</span></span>
| <span data-ttu-id="2d9e5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2d9e5-120">Name</span></span>          | <span data-ttu-id="2d9e5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2d9e5-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2d9e5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d9e5-122">Authorization</span></span> | <span data-ttu-id="2d9e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="2d9e5-125">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2d9e5-125">Function parameters</span></span>

| <span data-ttu-id="2d9e5-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="2d9e5-126">Parameter</span></span>     | <span data-ttu-id="2d9e5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2d9e5-127">Type</span></span>                 | <span data-ttu-id="2d9e5-128">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="2d9e5-128">Required?</span></span> | <span data-ttu-id="2d9e5-129">Description</span><span class="sxs-lookup"><span data-stu-id="2d9e5-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="2d9e5-130">Да</span><span class="sxs-lookup"><span data-stu-id="2d9e5-130">Yes</span></span>       | <span data-ttu-id="2d9e5-131">ИДЕНТИФИКАТОР принтера, для которого возвращаются данные.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-131">The ID of the printer to return data for.</span></span>                            |
| `periodStart` | `Edm.DateTimeOffset` | <span data-ttu-id="2d9e5-132">Нет</span><span class="sxs-lookup"><span data-stu-id="2d9e5-132">No</span></span>        | <span data-ttu-id="2d9e5-133">Дата начала (включительно) периода времени, из которого требуется включить данные.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `periodEnd`   | `Edm.DateTimeOffset` | <span data-ttu-id="2d9e5-134">Нет</span><span class="sxs-lookup"><span data-stu-id="2d9e5-134">No</span></span>        | <span data-ttu-id="2d9e5-135">Дата окончания (включительно) периода времени, из которого требуется включить данные.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="2d9e5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9e5-136">Response</span></span>
<span data-ttu-id="2d9e5-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [арчиведпринтжоб](../resources/archivedprintjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d9e5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2d9e5-138">Example</span></span>
<span data-ttu-id="2d9e5-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d9e5-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d9e5-140">Request</span></span>
<span data-ttu-id="2d9e5-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='{id}',periodStart=<timestamp>,periodEnd=<timestamp>)
```

##### <a name="response"></a><span data-ttu-id="2d9e5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9e5-142">Response</span></span>
<span data-ttu-id="2d9e5-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-143">The following is an example of the response.</span></span>
><span data-ttu-id="2d9e5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d9e5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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