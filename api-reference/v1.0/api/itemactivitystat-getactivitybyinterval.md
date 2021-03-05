---
author: daspek
title: Получать статистику активности элементов по интервалу
description: Получите itemAnalyticyStats для действий, которые произошли на этом ресурсе в течение указанного интервала времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b339458fb65f457c44113957ef541828a1940724
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471700"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="2996c-103">Получать статистику активности элементов по интервалу</span><span class="sxs-lookup"><span data-stu-id="2996c-103">Get item activity stats by interval</span></span>

<span data-ttu-id="2996c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2996c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2996c-105">Получите коллекцию [ресурсов itemActivityStats][] для действий, которые произошли на этом ресурсе в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="2996c-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="2996c-106">**Примечание:** Ресурс **itemAnalytics** еще не доступен во всех [национальных развертываниях.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="2996c-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span> 

<span data-ttu-id="2996c-107">Агрегаты аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="2996c-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="2996c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2996c-108">Permissions</span></span>

<span data-ttu-id="2996c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2996c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2996c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2996c-111">Permission type</span></span>                        | <span data-ttu-id="2996c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2996c-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="2996c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2996c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2996c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2996c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="2996c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2996c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2996c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2996c-116">Not supported.</span></span>
|<span data-ttu-id="2996c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2996c-117">Application</span></span>                            | <span data-ttu-id="2996c-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2996c-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2996c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2996c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="2996c-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2996c-120">Function parameters</span></span>

| <span data-ttu-id="2996c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="2996c-121">Parameter</span></span>      | <span data-ttu-id="2996c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="2996c-122">Type</span></span>               | <span data-ttu-id="2996c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2996c-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="2996c-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2996c-124">startDateTime</span></span>  | <span data-ttu-id="2996c-125">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="2996c-125">string (timestamp)</span></span> | <span data-ttu-id="2996c-126">Время начала, за которое можно агрегировать действия.</span><span class="sxs-lookup"><span data-stu-id="2996c-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="2996c-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2996c-127">endDateTime</span></span>    | <span data-ttu-id="2996c-128">string (timestamp)</span><span class="sxs-lookup"><span data-stu-id="2996c-128">string (timestamp)</span></span> | <span data-ttu-id="2996c-129">Конечный период, за который можно агрегировать действия.</span><span class="sxs-lookup"><span data-stu-id="2996c-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="2996c-130">interval</span><span class="sxs-lookup"><span data-stu-id="2996c-130">interval</span></span>       | <span data-ttu-id="2996c-131">string</span><span class="sxs-lookup"><span data-stu-id="2996c-131">string</span></span>             | <span data-ttu-id="2996c-132">Интервал агрегации.</span><span class="sxs-lookup"><span data-stu-id="2996c-132">The aggregation interval.</span></span>

><span data-ttu-id="2996c-133">**Примечание:** Этот API поддерживает только диапазон времени в 90 дней для ежедневных подсчетов.</span><span class="sxs-lookup"><span data-stu-id="2996c-133">**Note:** This API only supports a time range of 90 days for daily counts.</span></span> <span data-ttu-id="2996c-134">Значение и параметры должны представлять диапазон времени менее `startDateTime` `endDateTime` 90 дней.</span><span class="sxs-lookup"><span data-stu-id="2996c-134">The value of the `startDateTime` and `endDateTime` parameters must represent a time range of less than 90 days.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2996c-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2996c-135">Optional query parameters</span></span>
<span data-ttu-id="2996c-136">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2996c-136">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2996c-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2996c-137">Request headers</span></span>

| <span data-ttu-id="2996c-138">Имя</span><span class="sxs-lookup"><span data-stu-id="2996c-138">Name</span></span>      |<span data-ttu-id="2996c-139">Описание</span><span class="sxs-lookup"><span data-stu-id="2996c-139">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2996c-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2996c-140">Authorization</span></span>  | <span data-ttu-id="2996c-141">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="2996c-141">Bearer {code}.</span></span> <span data-ttu-id="2996c-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2996c-142">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2996c-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2996c-143">Request body</span></span>

<span data-ttu-id="2996c-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2996c-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2996c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2996c-145">Response</span></span> 

<span data-ttu-id="2996c-146">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объекта itemActivityStats][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2996c-146">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="2996c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="2996c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="2996c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2996c-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2996c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="2996c-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="2996c-150">C#</span><span class="sxs-lookup"><span data-stu-id="2996c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2996c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2996c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2996c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2996c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2996c-153">Java</span><span class="sxs-lookup"><span data-stu-id="2996c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2996c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2996c-154">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```http
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

