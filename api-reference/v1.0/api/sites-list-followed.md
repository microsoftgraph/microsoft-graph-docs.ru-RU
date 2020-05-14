---
author: learafa
description: Перечисление сайтов, отслеживаемых вошедшим пользователем.
title: Перечисление отслеживаемых сайтов
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: c08def6b72869cdc1886a71d1083dfdef51dbebd
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052336"
---
# <a name="list-followed-sites"></a><span data-ttu-id="f50e9-103">Перечисление отслеживаемых сайтов</span><span class="sxs-lookup"><span data-stu-id="f50e9-103">List followed sites</span></span>

<span data-ttu-id="f50e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f50e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f50e9-105">Перечислите [сайты](../resources/site.md) , за которыми подписан пользователь.</span><span class="sxs-lookup"><span data-stu-id="f50e9-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="f50e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f50e9-106">Permissions</span></span>

<span data-ttu-id="f50e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f50e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f50e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f50e9-109">Permission type</span></span>      | <span data-ttu-id="f50e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f50e9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f50e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f50e9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f50e9-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f50e9-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="f50e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f50e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f50e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f50e9-114">Not supported.</span></span>    |
|<span data-ttu-id="f50e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f50e9-115">Application</span></span> | <span data-ttu-id="f50e9-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f50e9-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f50e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f50e9-117">HTTP request</span></span>

<span data-ttu-id="f50e9-118">Этот метод доступен только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f50e9-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/followedSites
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f50e9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f50e9-119">Optional query parameters</span></span>
<span data-ttu-id="f50e9-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f50e9-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f50e9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f50e9-121">Request headers</span></span>

| <span data-ttu-id="f50e9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f50e9-122">Name</span></span>      |<span data-ttu-id="f50e9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f50e9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f50e9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f50e9-124">Authorization</span></span>  | <span data-ttu-id="f50e9-125">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="f50e9-125">Bearer {code}.</span></span> <span data-ttu-id="f50e9-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f50e9-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f50e9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f50e9-127">Request Body</span></span>

<span data-ttu-id="f50e9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f50e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f50e9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f50e9-129">Response</span></span>

<span data-ttu-id="f50e9-130">Этот метод возвращает коллекцию ресурсов [сайта](../resources/site.md) , которые подписаны пользователем.</span><span class="sxs-lookup"><span data-stu-id="f50e9-130">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="f50e9-131">Если сайты не найдены, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="f50e9-131">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="f50e9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f50e9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f50e9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f50e9-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f50e9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f50e9-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
POST /me/followedSites
```
# <a name="javascript"></a>[<span data-ttu-id="f50e9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f50e9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f50e9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f50e9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f50e9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f50e9-137">Response</span></span>
<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.site)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
            "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site",
            "webUrl": "https://contoso.sharepoint.com/teams/1drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "2C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/1drvteam",
                "webId": "2D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,1C712604-1370-44E7-A1F5-426573FDA80A,1D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site1",
            "webUrl": "https://contoso.sharepoint.com/teams/2drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "1C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/2drvteam",
                "webId": "1D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the sites a user is following.",
  "keywords": "site,onedrive.site,list followed sites, followedSites",
  "section": "documentation",
  "tocPath": "Sites/List followed sites",
  "suppressions": [
  ]
}
-->
