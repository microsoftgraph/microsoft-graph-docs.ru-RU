---
author: learafa
description: Перечислите сайты, за которыми подписан пользователь.
title: Список отслеживаемых сайтов
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: 750c69af83ffbd95d29385d6e97d0ea2a40e5d9d
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934915"
---
# <a name="list-followed-sites"></a><span data-ttu-id="0577d-103">Список отслеживаемых сайтов</span><span class="sxs-lookup"><span data-stu-id="0577d-103">List followed sites</span></span>

<span data-ttu-id="0577d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0577d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0577d-105">Перечислите [сайты](../resources/site.md) , за которыми подписан пользователь.</span><span class="sxs-lookup"><span data-stu-id="0577d-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="0577d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0577d-106">Permissions</span></span>

<span data-ttu-id="0577d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0577d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0577d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0577d-109">Permission type</span></span>      | <span data-ttu-id="0577d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0577d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0577d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0577d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0577d-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0577d-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="0577d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0577d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0577d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0577d-114">Not supported.</span></span>    |
|<span data-ttu-id="0577d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0577d-115">Application</span></span> | <span data-ttu-id="0577d-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0577d-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0577d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0577d-117">HTTP request</span></span>

<span data-ttu-id="0577d-118">Этот метод доступен только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0577d-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/followedSites
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0577d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0577d-119">Optional query parameters</span></span>
<span data-ttu-id="0577d-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0577d-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0577d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0577d-121">Request headers</span></span>

| <span data-ttu-id="0577d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0577d-122">Name</span></span>      |<span data-ttu-id="0577d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0577d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0577d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0577d-124">Authorization</span></span>  | <span data-ttu-id="0577d-125">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="0577d-125">Bearer {code}.</span></span> <span data-ttu-id="0577d-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0577d-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0577d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0577d-127">Request Body</span></span>

<span data-ttu-id="0577d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0577d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0577d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0577d-129">Response</span></span>

<span data-ttu-id="0577d-130">Этот метод возвращает коллекцию ресурсов [сайта](../resources/site.md) , которые подписаны пользователем.</span><span class="sxs-lookup"><span data-stu-id="0577d-130">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="0577d-131">Если сайты не найдены, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="0577d-131">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="0577d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0577d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0577d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0577d-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
POST /me/followedSites
```

### <a name="response"></a><span data-ttu-id="0577d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0577d-134">Response</span></span>
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
