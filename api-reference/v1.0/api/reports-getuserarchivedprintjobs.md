---
title: 'отчеты: getUserArchivedPrintJobs'
description: Получите список архивных заданий печати для конкретного пользователя.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f55a90939d5328075532695ff2af3416e27c5085
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517989"
---
# <a name="reportroot-getuserarchivedprintjobs"></a><span data-ttu-id="b5bf5-103">reportRoot: getUserArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="b5bf5-103">reportRoot: getUserArchivedPrintJobs</span></span>
<span data-ttu-id="b5bf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5bf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b5bf5-105">Получите список архивных заданий печати для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-105">Get a list of archived print jobs for a particular user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5bf5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5bf5-106">Permissions</span></span>
<span data-ttu-id="b5bf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b5bf5-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b5bf5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5bf5-110">Permission type</span></span> | <span data-ttu-id="b5bf5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5bf5-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b5bf5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5bf5-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b5bf5-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5bf5-113">Reports.Read.All</span></span> |
|<span data-ttu-id="b5bf5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5bf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5bf5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-115">Not Supported.</span></span>|
|<span data-ttu-id="b5bf5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b5bf5-116">Application</span></span>|<span data-ttu-id="b5bf5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5bf5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5bf5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getUserArchivedPrintJobs
```

## <a name="function-parameters"></a><span data-ttu-id="b5bf5-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b5bf5-119">Function Parameters</span></span>

| <span data-ttu-id="b5bf5-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="b5bf5-120">Parameter</span></span>     | <span data-ttu-id="b5bf5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b5bf5-121">Type</span></span>                 | <span data-ttu-id="b5bf5-122">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="b5bf5-122">Required?</span></span> | <span data-ttu-id="b5bf5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b5bf5-123">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | <span data-ttu-id="b5bf5-124">Да</span><span class="sxs-lookup"><span data-stu-id="b5bf5-124">Yes</span></span>       | <span data-ttu-id="b5bf5-125">ID пользователя для возврата данных.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-125">The ID of the user to return data for.</span></span>                               |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="b5bf5-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b5bf5-126">No</span></span>        | <span data-ttu-id="b5bf5-127">Дата начала (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-127">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="b5bf5-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b5bf5-128">No</span></span>        | <span data-ttu-id="b5bf5-129">Дата окончания (включительно) для периода времени с учетом данных.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-129">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="request-headers"></a><span data-ttu-id="b5bf5-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5bf5-130">Request headers</span></span>
|<span data-ttu-id="b5bf5-131">Имя</span><span class="sxs-lookup"><span data-stu-id="b5bf5-131">Name</span></span>|<span data-ttu-id="b5bf5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b5bf5-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b5bf5-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5bf5-133">Authorization</span></span>|<span data-ttu-id="b5bf5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5bf5-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5bf5-136">Request body</span></span>
<span data-ttu-id="b5bf5-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5bf5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5bf5-138">Response</span></span>

<span data-ttu-id="b5bf5-139">В случае успешной работы эта функция возвращает код ответа и коллекцию `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-139">If successful, this function returns a `200 OK` response code and a [archivedPrintJob](../resources/archivedprintjob.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5bf5-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5bf5-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5bf5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5bf5-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getuserarchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getUserArchivedPrintJobs(userId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
```

### <a name="response"></a><span data-ttu-id="b5bf5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5bf5-142">Response</span></span>
<span data-ttu-id="b5bf5-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b5bf5-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

