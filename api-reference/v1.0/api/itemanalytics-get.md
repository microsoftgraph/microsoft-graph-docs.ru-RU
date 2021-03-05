---
author: daspek
title: Get itemAnalytics
description: Получите itemAnalytics о представлениях, которые произошли в этом ресурсе.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 25965acd48ca69b68f0715d9e075a5e71d5d1529
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471691"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="e326e-103">Get itemAnalytics</span><span class="sxs-lookup"><span data-stu-id="e326e-103">Get itemAnalytics</span></span>

<span data-ttu-id="e326e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e326e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e326e-105">Получите [itemAnalytics][] о представлениях, которые произошли в этом ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e326e-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="e326e-106">Ресурс **itemAnalytics** — это удобный способ получения статистики активности для `allTime` и `lastSevenDays` .</span><span class="sxs-lookup"><span data-stu-id="e326e-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="e326e-107">Для настраиваемого диапазона времени или интервала используйте [API getActivitiesByInterval.][]</span><span class="sxs-lookup"><span data-stu-id="e326e-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="e326e-108">**Примечание:** Ресурс **itemAnalytics** еще не доступен во всех [национальных развертываниях.](/graph/deployments)</span><span class="sxs-lookup"><span data-stu-id="e326e-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="e326e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e326e-111">Permissions</span></span>

<span data-ttu-id="e326e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e326e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e326e-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e326e-114">Permission type</span></span>                        | <span data-ttu-id="e326e-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e326e-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="e326e-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e326e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e326e-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e326e-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="e326e-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e326e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e326e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e326e-119">Not supported.</span></span>
|<span data-ttu-id="e326e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e326e-120">Application</span></span>                            | <span data-ttu-id="e326e-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e326e-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e326e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e326e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e326e-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e326e-123">Optional query parameters</span></span>
<span data-ttu-id="e326e-124">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e326e-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e326e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e326e-125">Request headers</span></span>

| <span data-ttu-id="e326e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e326e-126">Name</span></span>      |<span data-ttu-id="e326e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e326e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e326e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e326e-128">Authorization</span></span>  | <span data-ttu-id="e326e-129">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="e326e-129">Bearer {code}.</span></span> <span data-ttu-id="e326e-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e326e-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e326e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e326e-131">Request body</span></span>

<span data-ttu-id="e326e-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e326e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e326e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e326e-133">Response</span></span> 

<span data-ttu-id="e326e-134">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объекта itemAnalytics][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e326e-134">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="e326e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e326e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="e326e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e326e-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e326e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e326e-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="e326e-138">C#</span><span class="sxs-lookup"><span data-stu-id="e326e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e326e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e326e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e326e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e326e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e326e-141">Java</span><span class="sxs-lookup"><span data-stu-id="e326e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e326e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e326e-142">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```http
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

