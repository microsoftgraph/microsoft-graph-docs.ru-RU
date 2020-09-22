---
author: daspek
ms.author: dspektor
title: Получение статистики по действиям элемента по интервалу
description: Получение Итеманалитицистатс для действий, выполненных с этим ресурсом в течение указанного интервала времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a26892aac83aa28b7a4769f2ad678643a3c417ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087227"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="c4c88-103">Получение статистики по действиям элемента по интервалу</span><span class="sxs-lookup"><span data-stu-id="c4c88-103">Get item activity stats by interval</span></span>

<span data-ttu-id="c4c88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4c88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4c88-105">Получение коллекции ресурсов [итемактивитистатс][] для действий, выполняемых с этим ресурсом в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="c4c88-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="c4c88-106">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="c4c88-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span> 

<span data-ttu-id="c4c88-107">Статистические функции аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="c4c88-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4c88-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4c88-108">Permissions</span></span>

<span data-ttu-id="c4c88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4c88-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4c88-111">Permission type</span></span>                        | <span data-ttu-id="c4c88-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4c88-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c4c88-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4c88-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4c88-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c88-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c4c88-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4c88-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4c88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4c88-116">Not supported.</span></span>
|<span data-ttu-id="c4c88-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4c88-117">Application</span></span>                            | <span data-ttu-id="c4c88-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c88-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c4c88-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4c88-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="c4c88-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c4c88-120">Function parameters</span></span>

| <span data-ttu-id="c4c88-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4c88-121">Parameter</span></span>      | <span data-ttu-id="c4c88-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c4c88-122">Type</span></span>               | <span data-ttu-id="c4c88-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c4c88-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="c4c88-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c4c88-124">startDateTime</span></span>  | <span data-ttu-id="c4c88-125">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="c4c88-125">string (timestamp)</span></span> | <span data-ttu-id="c4c88-126">Время начала агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="c4c88-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="c4c88-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c4c88-127">endDateTime</span></span>    | <span data-ttu-id="c4c88-128">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="c4c88-128">string (timestamp)</span></span> | <span data-ttu-id="c4c88-129">Время окончания агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="c4c88-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="c4c88-130">interval</span><span class="sxs-lookup"><span data-stu-id="c4c88-130">interval</span></span>       | <span data-ttu-id="c4c88-131">string</span><span class="sxs-lookup"><span data-stu-id="c4c88-131">string</span></span>             | <span data-ttu-id="c4c88-132">Интервал объединения.</span><span class="sxs-lookup"><span data-stu-id="c4c88-132">The aggregation interval.</span></span>

><span data-ttu-id="c4c88-133">**Примечание:** Этот API поддерживает только диапазон времени 90 дней для ежедневных счетчиков.</span><span class="sxs-lookup"><span data-stu-id="c4c88-133">**Note:** This API only supports a time range of 90 days for daily counts.</span></span> <span data-ttu-id="c4c88-134">Значение `startDateTime` `endDateTime` параметра и должно представлять собой диапазон времени менее 90 дней.</span><span class="sxs-lookup"><span data-stu-id="c4c88-134">The value of the `startDateTime` and `endDateTime` parameters must represent a time range of less than 90 days.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c4c88-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4c88-135">Optional query parameters</span></span>
<span data-ttu-id="c4c88-136">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c4c88-136">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4c88-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4c88-137">Request headers</span></span>

| <span data-ttu-id="c4c88-138">Имя</span><span class="sxs-lookup"><span data-stu-id="c4c88-138">Name</span></span>      |<span data-ttu-id="c4c88-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c4c88-139">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4c88-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4c88-140">Authorization</span></span>  | <span data-ttu-id="c4c88-141">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="c4c88-141">Bearer {code}.</span></span> <span data-ttu-id="c4c88-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c4c88-142">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4c88-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4c88-143">Request body</span></span>

<span data-ttu-id="c4c88-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4c88-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4c88-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4c88-145">Response</span></span> 

<span data-ttu-id="c4c88-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объекта [итемактивитистатс][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4c88-146">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="c4c88-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c4c88-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4c88-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4c88-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c4c88-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4c88-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="c4c88-150">C#</span><span class="sxs-lookup"><span data-stu-id="c4c88-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4c88-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4c88-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4c88-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4c88-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4c88-153">Java</span><span class="sxs-lookup"><span data-stu-id="c4c88-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4c88-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4c88-154">Response</span></span>

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
[итемактивитистатс]: ../resources/itemactivitystat.md
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

