---
author: daspek
ms.author: dspektor
title: Получение статистики по действиям элемента по интервалу
description: Получение Итеманалитицистатс для действий, выполненных с этим ресурсом в течение указанного интервала времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 30f06f9bcdfb96f61f39b81152f0c9cd23872e49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025535"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="1fc6e-103">Получение статистики по действиям элемента по интервалу</span><span class="sxs-lookup"><span data-stu-id="1fc6e-103">Get item activity stats by interval</span></span>

<span data-ttu-id="1fc6e-104">Получение коллекции ресурсов [итемактивитистатс][] для действий, выполняемых с этим ресурсом в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-104">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="1fc6e-105">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="1fc6e-105">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="1fc6e-106">Статистические функции аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-106">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fc6e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fc6e-107">Permissions</span></span>

<span data-ttu-id="1fc6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fc6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fc6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fc6e-110">Permission type</span></span>                        | <span data-ttu-id="1fc6e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fc6e-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="1fc6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fc6e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fc6e-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc6e-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="1fc6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fc6e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fc6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-115">Not supported.</span></span>
|<span data-ttu-id="1fc6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fc6e-116">Application</span></span>                            | <span data-ttu-id="1fc6e-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc6e-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="1fc6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fc6e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="1fc6e-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1fc6e-119">Function parameters</span></span>

| <span data-ttu-id="1fc6e-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="1fc6e-120">Parameter</span></span>      | <span data-ttu-id="1fc6e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1fc6e-121">Type</span></span>               | <span data-ttu-id="1fc6e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1fc6e-122">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="1fc6e-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1fc6e-123">startDateTime</span></span>  | <span data-ttu-id="1fc6e-124">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="1fc6e-124">string (timestamp)</span></span> | <span data-ttu-id="1fc6e-125">Время начала агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-125">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="1fc6e-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1fc6e-126">endDateTime</span></span>    | <span data-ttu-id="1fc6e-127">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="1fc6e-127">string (timestamp)</span></span> | <span data-ttu-id="1fc6e-128">Время окончания агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-128">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="1fc6e-129">interval</span><span class="sxs-lookup"><span data-stu-id="1fc6e-129">interval</span></span>       | <span data-ttu-id="1fc6e-130">string</span><span class="sxs-lookup"><span data-stu-id="1fc6e-130">string</span></span>             | <span data-ttu-id="1fc6e-131">Интервал объединения.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-131">The aggregation interval.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1fc6e-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1fc6e-132">Optional query parameters</span></span>
<span data-ttu-id="1fc6e-133">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-133">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fc6e-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fc6e-134">Request headers</span></span>

| <span data-ttu-id="1fc6e-135">Имя</span><span class="sxs-lookup"><span data-stu-id="1fc6e-135">Name</span></span>      |<span data-ttu-id="1fc6e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1fc6e-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1fc6e-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fc6e-137">Authorization</span></span>  | <span data-ttu-id="1fc6e-138">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-138">Bearer {code}.</span></span> <span data-ttu-id="1fc6e-139">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-139">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fc6e-140">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="1fc6e-140">Request body</span></span>

<span data-ttu-id="1fc6e-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fc6e-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="1fc6e-142">Response</span></span> 

<span data-ttu-id="1fc6e-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объекта [итемактивитистатс][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fc6e-143">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="1fc6e-144">Пример</span><span class="sxs-lookup"><span data-stu-id="1fc6e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fc6e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc6e-145">Request</span></span>

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

### <a name="response"></a><span data-ttu-id="1fc6e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc6e-146">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
        }
    ]
}
```
[Итемактивитистатс]: ../resources/itemactivitystat.md
[itemActivityStats]: ../resources/itemactivitystat.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": []
}
-->
