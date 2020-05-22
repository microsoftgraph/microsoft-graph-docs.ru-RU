---
author: daspek
ms.author: dspektor
title: Получение статистики по действиям элемента по интервалу
description: Получение Итеманалитицистатс для действий, выполненных с этим ресурсом в течение указанного интервала времени.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f39fdcb00b367bed4044bad521b658c897fdc016
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345711"
---
# <a name="get-item-activity-stats-by-interval"></a><span data-ttu-id="32289-103">Получение статистики по действиям элемента по интервалу</span><span class="sxs-lookup"><span data-stu-id="32289-103">Get item activity stats by interval</span></span>

<span data-ttu-id="32289-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32289-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32289-105">Получение коллекции ресурсов [итемактивитистатс][] для действий, выполняемых с этим ресурсом в течение указанного интервала времени.</span><span class="sxs-lookup"><span data-stu-id="32289-105">Get a collection of [itemActivityStats][] resources for the activities that took place on this resource within the specified time interval.</span></span>

><span data-ttu-id="32289-106">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="32289-106">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

<span data-ttu-id="32289-107">Статистические функции аналитики могут быть недоступны для всех типов действий.</span><span class="sxs-lookup"><span data-stu-id="32289-107">Analytics aggregates might not be available for all action types.</span></span>

## <a name="permissions"></a><span data-ttu-id="32289-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32289-108">Permissions</span></span>

<span data-ttu-id="32289-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32289-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32289-111">Permission type</span></span>                        | <span data-ttu-id="32289-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32289-112">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="32289-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32289-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="32289-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32289-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="32289-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32289-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32289-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32289-116">Not supported.</span></span>
|<span data-ttu-id="32289-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32289-117">Application</span></span>                            | <span data-ttu-id="32289-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32289-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="32289-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32289-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016-01-01',endDateTime='2017-05-20',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a><span data-ttu-id="32289-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="32289-120">Function parameters</span></span>

| <span data-ttu-id="32289-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="32289-121">Parameter</span></span>      | <span data-ttu-id="32289-122">Тип</span><span class="sxs-lookup"><span data-stu-id="32289-122">Type</span></span>               | <span data-ttu-id="32289-123">Описание</span><span class="sxs-lookup"><span data-stu-id="32289-123">Description</span></span>
|:---------------|:-------------------|:---------------------------------------
| <span data-ttu-id="32289-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="32289-124">startDateTime</span></span>  | <span data-ttu-id="32289-125">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="32289-125">string (timestamp)</span></span> | <span data-ttu-id="32289-126">Время начала агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="32289-126">The start time over which to aggregate activities.</span></span>
| <span data-ttu-id="32289-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="32289-127">endDateTime</span></span>    | <span data-ttu-id="32289-128">строка (timestamp)</span><span class="sxs-lookup"><span data-stu-id="32289-128">string (timestamp)</span></span> | <span data-ttu-id="32289-129">Время окончания агрегирования действий.</span><span class="sxs-lookup"><span data-stu-id="32289-129">The end time over which to aggregate activities.</span></span>
| <span data-ttu-id="32289-130">interval</span><span class="sxs-lookup"><span data-stu-id="32289-130">interval</span></span>       | <span data-ttu-id="32289-131">string</span><span class="sxs-lookup"><span data-stu-id="32289-131">string</span></span>             | <span data-ttu-id="32289-132">Интервал объединения.</span><span class="sxs-lookup"><span data-stu-id="32289-132">The aggregation interval.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="32289-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32289-133">Optional query parameters</span></span>
<span data-ttu-id="32289-134">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="32289-134">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32289-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32289-135">Request headers</span></span>

| <span data-ttu-id="32289-136">Имя</span><span class="sxs-lookup"><span data-stu-id="32289-136">Name</span></span>      |<span data-ttu-id="32289-137">Описание</span><span class="sxs-lookup"><span data-stu-id="32289-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32289-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32289-138">Authorization</span></span>  | <span data-ttu-id="32289-139">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="32289-139">Bearer {code}.</span></span> <span data-ttu-id="32289-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="32289-140">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32289-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32289-141">Request body</span></span>

<span data-ttu-id="32289-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32289-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32289-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="32289-143">Response</span></span> 

<span data-ttu-id="32289-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объекта [итемактивитистатс][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32289-144">If successful, this method returns a `200 OK` response code and a collection of [itemActivityStats][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="32289-145">Пример</span><span class="sxs-lookup"><span data-stu-id="32289-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="32289-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="32289-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="32289-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="32289-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```
# <a name="c"></a>[<span data-ttu-id="32289-148">C#</span><span class="sxs-lookup"><span data-stu-id="32289-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activities-by-interval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32289-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32289-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activities-by-interval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32289-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32289-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activities-by-interval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32289-151">Java</span><span class="sxs-lookup"><span data-stu-id="32289-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activities-by-interval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="32289-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="32289-152">Response</span></span>

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
