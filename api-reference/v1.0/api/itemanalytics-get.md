---
author: daspek
title: Get itemAnalytics
description: Получите itemAnalytics о представлениях, которые произошли в этом ресурсе.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2307df47b5c914a1b9257e30d39c3fe2b539bf32
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238829"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="2d809-103">Get itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="2d809-103">Get itemAnalytics</span></span>

<span data-ttu-id="2d809-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d809-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d809-105">Получите [itemAnalytics][] о представлениях, которые произошли в этом ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2d809-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="2d809-106">Ресурс **itemAnalytics** — удобный способ получить статистику активности `allTime` для и `lastSevenDays` .</span><span class="sxs-lookup"><span data-stu-id="2d809-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="2d809-107">Для настраиваемого диапазона времени или интервала используйте API [getActivitiesByInterval.][]</span><span class="sxs-lookup"><span data-stu-id="2d809-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="2d809-108">**Примечание.** Ресурс **itemAnalytics** пока не доступен во всех [национальных развертываниях.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="2d809-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="2d809-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d809-111">Permissions</span></span>

<span data-ttu-id="2d809-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d809-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d809-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d809-114">Permission type</span></span>                        | <span data-ttu-id="2d809-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d809-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="2d809-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d809-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d809-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d809-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="2d809-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d809-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d809-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d809-119">Not supported.</span></span>
|<span data-ttu-id="2d809-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d809-120">Application</span></span>                            | <span data-ttu-id="2d809-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d809-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2d809-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d809-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d809-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d809-123">Optional query parameters</span></span>
<span data-ttu-id="2d809-124">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2d809-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d809-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d809-125">Request headers</span></span>

| <span data-ttu-id="2d809-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2d809-126">Name</span></span>      |<span data-ttu-id="2d809-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2d809-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d809-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d809-128">Authorization</span></span>  | <span data-ttu-id="2d809-129">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="2d809-129">Bearer {code}.</span></span> <span data-ttu-id="2d809-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2d809-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d809-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d809-131">Request body</span></span>

<span data-ttu-id="2d809-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d809-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d809-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d809-133">Response</span></span> 

<span data-ttu-id="2d809-134">В случае успеха этот метод возвращает код отклика и коллекцию объекта `200 OK` [itemAnalytics][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d809-134">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="2d809-135">Пример</span><span class="sxs-lookup"><span data-stu-id="2d809-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d809-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d809-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2d809-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d809-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="2d809-138">C#</span><span class="sxs-lookup"><span data-stu-id="2d809-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d809-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d809-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d809-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d809-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d809-141">Java</span><span class="sxs-lookup"><span data-stu-id="2d809-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d809-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d809-142">Response</span></span>

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

