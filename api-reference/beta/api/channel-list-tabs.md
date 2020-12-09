---
title: Вкладки списка в канале
description: 'Получение списка вкладок в указанном канале в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2d07c9e3c59e13b376efa7eb11fa4aeae8f5cfcd
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607638"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="57ef5-103">Вкладки списка в канале</span><span class="sxs-lookup"><span data-stu-id="57ef5-103">List tabs in channel</span></span>

<span data-ttu-id="57ef5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57ef5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57ef5-105">Получение списка [вкладок](../resources/teamstab.md) в указанном [канале](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="57ef5-105">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="57ef5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57ef5-106">Permissions</span></span>
<span data-ttu-id="57ef5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ef5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57ef5-109">Permission type</span></span>      | <span data-ttu-id="57ef5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57ef5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57ef5-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57ef5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57ef5-112">TeamsTab. Read. ALL, TeamsTab. Реадвритефортеам, TeamsTab. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="57ef5-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="57ef5-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57ef5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57ef5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ef5-114">Not supported.</span></span>    |
|<span data-ttu-id="57ef5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="57ef5-115">Application</span></span> | <span data-ttu-id="57ef5-116">TeamsTab. Read. Group *, TeamsTab. ReadWrite. Group*, TeamsTab. Read. ALL, TeamsTab. Реадвритефортеам. ALL, TeamsTab. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="57ef5-116">TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="57ef5-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="57ef5-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="57ef5-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="57ef5-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="57ef5-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="57ef5-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="57ef5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57ef5-120">HTTP request</span></span>

```http
GET /teams/{team-id}/channels/{channel-id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57ef5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57ef5-121">Optional query parameters</span></span>

<span data-ttu-id="57ef5-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="57ef5-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57ef5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57ef5-123">Request headers</span></span>
| <span data-ttu-id="57ef5-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57ef5-124">Header</span></span>       | <span data-ttu-id="57ef5-125">Значение</span><span class="sxs-lookup"><span data-stu-id="57ef5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="57ef5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57ef5-126">Authorization</span></span>  | <span data-ttu-id="57ef5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57ef5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57ef5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57ef5-129">Request body</span></span>
<span data-ttu-id="57ef5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57ef5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57ef5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ef5-131">Response</span></span>
<span data-ttu-id="57ef5-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [вкладок](../resources/teamstab.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57ef5-132">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57ef5-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="57ef5-133">Examples</span></span>

### <a name="example-1-list-all-the-tabs-in-the-channel-along-with-associated-teams-app"></a><span data-ttu-id="57ef5-134">Пример 1: список всех вкладок в канале вместе со связанным приложением Teams</span><span class="sxs-lookup"><span data-stu-id="57ef5-134">Example 1: List all the tabs in the channel along with associated Teams app</span></span>
#### <a name="request"></a><span data-ttu-id="57ef5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="57ef5-135">Request</span></span>
<span data-ttu-id="57ef5-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57ef5-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tabs_in_channel"
}
-->

```http
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs?$expand=teamsApp
```

#### <a name="response"></a><span data-ttu-id="57ef5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ef5-137">Response</span></span>
<span data-ttu-id="57ef5-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="57ef5-138">The following is an example of the response.</span></span>
><span data-ttu-id="57ef5-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57ef5-139">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "displayName": "My Contoso Tab - updated",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": "20",
      "teamsApp": {
        "id": "06805b9e-77e3-4b93-ac81-525eb87513b8",
        "displayName": "Contoso",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```

### <a name="example-2-list-all-the-tabs-belonging-to-a-specific-app-in-a-channel"></a><span data-ttu-id="57ef5-140">Пример 2: список всех вкладок, принадлежащих конкретному приложению в канале</span><span class="sxs-lookup"><span data-stu-id="57ef5-140">Example 2: List all the tabs belonging to a specific app in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="57ef5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="57ef5-141">Request</span></span>
<span data-ttu-id="57ef5-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57ef5-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tabs_in_channel_app_filter"
}
-->

```http
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs?$expand=teamsApp&$filter=teamsApp/id eq 'com.microsoft.teamspace.tab.planner'
```

#### <a name="response"></a><span data-ttu-id="57ef5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ef5-143">Response</span></span>
<span data-ttu-id="57ef5-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="57ef5-144">The following is an example of the response.</span></span>
><span data-ttu-id="57ef5-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57ef5-145">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/channels('19%3A33b76eea88574bd1969dca37e2b7a819%40thread.skype')/tabs(teamsApp())",
  "@odata.count": 1,
  "value": [
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


