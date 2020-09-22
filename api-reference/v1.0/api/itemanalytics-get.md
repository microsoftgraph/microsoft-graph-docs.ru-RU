---
author: daspek
ms.author: dspektor
title: Получение Итеманалитикс
description: Получение Итеманалитикс о представлениях, которые были выполнены для этого ресурса.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 311d7eea81ba3001af6cb94e2a3f837824a67fde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038475"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="82cfd-103">Получение Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="82cfd-103">Get itemAnalytics</span></span>

<span data-ttu-id="82cfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cfd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82cfd-105">Получение [итеманалитикс][] о представлениях, которые были выполнены для этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="82cfd-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="82cfd-106">Ресурс **итеманалитикс** — это удобный способ получения статистики действий `allTime` и `lastSevenDays` .</span><span class="sxs-lookup"><span data-stu-id="82cfd-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="82cfd-107">Для настраиваемого диапазона или интервала времени используйте API [getActivitiesByInterval][] .</span><span class="sxs-lookup"><span data-stu-id="82cfd-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="82cfd-108">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="82cfd-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="82cfd-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82cfd-111">Permissions</span></span>

<span data-ttu-id="82cfd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82cfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82cfd-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82cfd-114">Permission type</span></span>                        | <span data-ttu-id="82cfd-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82cfd-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="82cfd-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82cfd-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="82cfd-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cfd-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="82cfd-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82cfd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82cfd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82cfd-119">Not supported.</span></span>
|<span data-ttu-id="82cfd-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82cfd-120">Application</span></span>                            | <span data-ttu-id="82cfd-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82cfd-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="82cfd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82cfd-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="82cfd-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82cfd-123">Optional query parameters</span></span>
<span data-ttu-id="82cfd-124">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="82cfd-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82cfd-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82cfd-125">Request headers</span></span>

| <span data-ttu-id="82cfd-126">Имя</span><span class="sxs-lookup"><span data-stu-id="82cfd-126">Name</span></span>      |<span data-ttu-id="82cfd-127">Описание</span><span class="sxs-lookup"><span data-stu-id="82cfd-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82cfd-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82cfd-128">Authorization</span></span>  | <span data-ttu-id="82cfd-129">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="82cfd-129">Bearer {code}.</span></span> <span data-ttu-id="82cfd-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="82cfd-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82cfd-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82cfd-131">Request body</span></span>

<span data-ttu-id="82cfd-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82cfd-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82cfd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="82cfd-133">Response</span></span> 

<span data-ttu-id="82cfd-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объекта [итеманалитикс][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82cfd-134">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="82cfd-135">Пример</span><span class="sxs-lookup"><span data-stu-id="82cfd-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="82cfd-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="82cfd-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="82cfd-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="82cfd-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="82cfd-138">C#</span><span class="sxs-lookup"><span data-stu-id="82cfd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82cfd-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82cfd-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82cfd-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82cfd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82cfd-141">Java</span><span class="sxs-lookup"><span data-stu-id="82cfd-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82cfd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="82cfd-142">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
  ]
}
-->

