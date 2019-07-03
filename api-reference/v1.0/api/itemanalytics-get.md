---
author: daspek
ms.author: dspektor
title: Получение Итеманалитикс
description: Получение Итеманалитикс о представлениях, которые были выполнены для этого ресурса.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 08c214feef8b5ea539401466866f71cf0841bbe3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455373"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="88bcb-103">Получение Итеманалитикс</span><span class="sxs-lookup"><span data-stu-id="88bcb-103">Get itemAnalytics</span></span>

<span data-ttu-id="88bcb-104">Получение [итеманалитикс][] о представлениях, которые были выполнены для этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="88bcb-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="88bcb-105">Ресурс **итеманалитикс** — это удобный способ получения статистики действий `allTime` и. `lastSevenDays`</span><span class="sxs-lookup"><span data-stu-id="88bcb-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="88bcb-106">Для настраиваемого диапазона или интервала времени используйте API [getActivitiesByInterval][] .</span><span class="sxs-lookup"><span data-stu-id="88bcb-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="88bcb-107">**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="88bcb-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="88bcb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88bcb-110">Permissions</span></span>

<span data-ttu-id="88bcb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88bcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88bcb-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88bcb-113">Permission type</span></span>                        | <span data-ttu-id="88bcb-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88bcb-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="88bcb-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88bcb-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="88bcb-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88bcb-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="88bcb-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88bcb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88bcb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88bcb-118">Not supported.</span></span>
|<span data-ttu-id="88bcb-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88bcb-119">Application</span></span>                            | <span data-ttu-id="88bcb-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88bcb-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="88bcb-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88bcb-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88bcb-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="88bcb-122">Optional query parameters</span></span>
<span data-ttu-id="88bcb-123">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="88bcb-123">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88bcb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88bcb-124">Request headers</span></span>

| <span data-ttu-id="88bcb-125">Имя</span><span class="sxs-lookup"><span data-stu-id="88bcb-125">Name</span></span>      |<span data-ttu-id="88bcb-126">Описание</span><span class="sxs-lookup"><span data-stu-id="88bcb-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88bcb-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88bcb-127">Authorization</span></span>  | <span data-ttu-id="88bcb-128">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="88bcb-128">Bearer {code}.</span></span> <span data-ttu-id="88bcb-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="88bcb-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88bcb-130">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="88bcb-130">Request body</span></span>

<span data-ttu-id="88bcb-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88bcb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88bcb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="88bcb-132">Response</span></span> 

<span data-ttu-id="88bcb-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объекта [итеманалитикс][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88bcb-133">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="88bcb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="88bcb-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="88bcb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="88bcb-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="88bcb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="88bcb-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="88bcb-137">C#</span><span class="sxs-lookup"><span data-stu-id="88bcb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88bcb-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="88bcb-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88bcb-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="88bcb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88bcb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="88bcb-140">Response</span></span>

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
