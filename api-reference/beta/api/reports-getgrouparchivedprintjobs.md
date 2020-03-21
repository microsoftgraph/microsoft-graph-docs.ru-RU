---
title: 'отчеты: Жетграупарчиведпринтжобс'
description: Получение списка архивных заданий печати для определенной группы.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6ca705555bb912daa8710315ab8dc4766c7ffb4c
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896131"
---
# <a name="reports-getgrouparchivedprintjobs"></a><span data-ttu-id="b4fd2-103">отчеты: Жетграупарчиведпринтжобс</span><span class="sxs-lookup"><span data-stu-id="b4fd2-103">reports: getGroupArchivedPrintJobs</span></span>

<span data-ttu-id="b4fd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4fd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4fd2-105">Получение списка архивных заданий печати для определенной группы.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-105">Get a list of archived print jobs for a particular group.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4fd2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4fd2-106">Permissions</span></span>
<span data-ttu-id="b4fd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4fd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b4fd2-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b4fd2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4fd2-110">Permission type</span></span> | <span data-ttu-id="b4fd2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4fd2-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b4fd2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4fd2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b4fd2-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b4fd2-113">Users.Read.All</span></span> |
|<span data-ttu-id="b4fd2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4fd2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4fd2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-115">Not Supported.</span></span>|
|<span data-ttu-id="b4fd2-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b4fd2-116">Application</span></span>|<span data-ttu-id="b4fd2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4fd2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4fd2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getGroupArchivedPrintJobs
GET /reports/getGroupArchivedPrintJobs
```
## <a name="request-headers"></a><span data-ttu-id="b4fd2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4fd2-119">Request headers</span></span>
| <span data-ttu-id="b4fd2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b4fd2-120">Name</span></span>          | <span data-ttu-id="b4fd2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b4fd2-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b4fd2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4fd2-122">Authorization</span></span> | <span data-ttu-id="b4fd2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="b4fd2-125">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b4fd2-125">Function parameters</span></span>

|<span data-ttu-id="b4fd2-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="b4fd2-126">Parameter</span></span>|<span data-ttu-id="b4fd2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b4fd2-127">Type</span></span>|<span data-ttu-id="b4fd2-128">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="b4fd2-128">Required?</span></span>|<span data-ttu-id="b4fd2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b4fd2-129">Description</span></span>|
|-|-|-|-|-|
|`groupId`|`Edm.String`|<span data-ttu-id="b4fd2-130">Да</span><span class="sxs-lookup"><span data-stu-id="b4fd2-130">Yes</span></span>|<span data-ttu-id="b4fd2-131">Идентификатор группы, для которой требуется возвратить данные.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-131">The ID of the group to return data for.</span></span>|
|`periodStart`|`Edm.DateTimeOffset`|<span data-ttu-id="b4fd2-132">Нет</span><span class="sxs-lookup"><span data-stu-id="b4fd2-132">No</span></span>|<span data-ttu-id="b4fd2-133">Дата начала (включительно) периода времени, из которого требуется включить данные.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-133">The start date (inclusive) for the time period to include data from.</span></span>|
|`periodEnd`|`Edm.DateTimeOffset`|<span data-ttu-id="b4fd2-134">Нет</span><span class="sxs-lookup"><span data-stu-id="b4fd2-134">No</span></span>|<span data-ttu-id="b4fd2-135">Дата окончания (включительно) периода времени, из которого требуется включить данные.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-135">The end date (inclusive) for the time period to include data from.</span></span>|

## <a name="response"></a><span data-ttu-id="b4fd2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4fd2-136">Response</span></span>
<span data-ttu-id="b4fd2-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [арчиведпринтжоб](../resources/archivedprintjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4fd2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b4fd2-138">Example</span></span>
<span data-ttu-id="b4fd2-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b4fd2-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4fd2-140">Request</span></span>
<span data-ttu-id="b4fd2-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getgrouparchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getGroupArchivedPrintJobs(groupId='{id}',periodStart=<timestamp>,periodEnd=<timestamp>)
```

##### <a name="response"></a><span data-ttu-id="b4fd2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4fd2-142">Response</span></span>
<span data-ttu-id="b4fd2-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-143">The following is an example of the response.</span></span>
><span data-ttu-id="b4fd2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4fd2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
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
  "description": "printJob: getGroupArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->