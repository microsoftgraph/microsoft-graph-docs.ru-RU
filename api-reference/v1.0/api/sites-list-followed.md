---
author: learafa
description: Перечисление сайтов, отслеживаемых вошедшим пользователем.
title: Перечисление отслеживаемых сайтов
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: e1f1d781897802eab62674d4bbed18507ec4d2c6
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006697"
---
# <a name="list-followed-sites"></a><span data-ttu-id="da2f5-103">Перечисление отслеживаемых сайтов</span><span class="sxs-lookup"><span data-stu-id="da2f5-103">List followed sites</span></span>

<span data-ttu-id="da2f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da2f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da2f5-105">Перечислите [сайты](../resources/site.md) , за которыми подписан пользователь.</span><span class="sxs-lookup"><span data-stu-id="da2f5-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="da2f5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da2f5-106">Permissions</span></span>

<span data-ttu-id="da2f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da2f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da2f5-109">Permission type</span></span>      | <span data-ttu-id="da2f5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da2f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da2f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da2f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da2f5-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2f5-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="da2f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da2f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da2f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da2f5-114">Not supported.</span></span>    |
|<span data-ttu-id="da2f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da2f5-115">Application</span></span> | <span data-ttu-id="da2f5-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2f5-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da2f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da2f5-117">HTTP request</span></span>

<span data-ttu-id="da2f5-118">Этот метод доступен только в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="da2f5-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/followedSites
```
<span data-ttu-id="da2f5-119">Получение списка сайтов, за которыми следует целевой пользователь, в зависимости от его идентификатора.</span><span class="sxs-lookup"><span data-stu-id="da2f5-119">Get a list of the sites followed by a target user, based on its ID.</span></span>

```http
GET /users/{user-id}/followedSites
```
<span data-ttu-id="da2f5-120">**Примечание:** Чтобы получить доступ к списку отслеживаемых сайтов другого пользователя, необходимы разрешения приложения.</span><span class="sxs-lookup"><span data-stu-id="da2f5-120">**Note:** To access another targeted user's list of followed sites, you need application permissions.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="da2f5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da2f5-121">Optional query parameters</span></span>
<span data-ttu-id="da2f5-122">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="da2f5-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da2f5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da2f5-123">Request headers</span></span>

| <span data-ttu-id="da2f5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="da2f5-124">Name</span></span>      |<span data-ttu-id="da2f5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="da2f5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da2f5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da2f5-126">Authorization</span></span>  | <span data-ttu-id="da2f5-127">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="da2f5-127">Bearer {code}.</span></span> <span data-ttu-id="da2f5-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="da2f5-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da2f5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da2f5-129">Request Body</span></span>

<span data-ttu-id="da2f5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da2f5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da2f5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2f5-131">Response</span></span>

<span data-ttu-id="da2f5-132">Этот метод возвращает коллекцию ресурсов [сайта](../resources/site.md) , которые подписаны пользователем.</span><span class="sxs-lookup"><span data-stu-id="da2f5-132">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="da2f5-133">Если сайты не найдены, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="da2f5-133">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="da2f5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="da2f5-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="da2f5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="da2f5-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="da2f5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="da2f5-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "sites-list-followed", "scopes": "sites.readwrite.all" } -->

```msgraph-interactive
GET /me/followedSites
```
# <a name="javascript"></a>[<span data-ttu-id="da2f5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da2f5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sites-list-followed-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da2f5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da2f5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sites-list-followed-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="da2f5-139">C#</span><span class="sxs-lookup"><span data-stu-id="da2f5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sites-list-followed-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da2f5-140">Java</span><span class="sxs-lookup"><span data-stu-id="da2f5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sites-list-followed-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da2f5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2f5-141">Response</span></span>
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
