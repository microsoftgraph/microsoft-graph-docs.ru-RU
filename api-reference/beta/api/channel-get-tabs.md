---
title: Получение вкладки на канале
description: 'Извлечение свойств и связей указанной вкладки в канале в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9a81cd2009266ed09ed723d7171aef54a04ed405
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200956"
---
# <a name="get-tab-in-channel"></a><span data-ttu-id="9f137-103">Получение вкладки на канале</span><span class="sxs-lookup"><span data-stu-id="9f137-103">Get tab in channel</span></span>

<span data-ttu-id="9f137-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f137-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f137-105">Извлечение свойств и связей [](../resources/teamstab.md) указанной вкладки в [канале](../resources/channel.md) в [команде.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="9f137-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md) in a [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="9f137-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f137-106">Permissions</span></span>
<span data-ttu-id="9f137-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f137-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f137-109">Permission type</span></span>      | <span data-ttu-id="9f137-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f137-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f137-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f137-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f137-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f137-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9f137-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f137-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f137-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f137-114">Not supported.</span></span>    |
|<span data-ttu-id="9f137-115">Application</span><span class="sxs-lookup"><span data-stu-id="9f137-115">Application</span></span> | <span data-ttu-id="9f137-116">TeamsTab.Read.Group,*TeamsTab.ReadWrite.Group,* TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f137-116">TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="9f137-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="9f137-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="9f137-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="9f137-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9f137-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="9f137-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f137-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f137-120">HTTP request</span></span>
```http
GET /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f137-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f137-121">Optional query parameters</span></span>

<span data-ttu-id="9f137-122">Этот метод поддерживает параметры $select и $expand [OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f137-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f137-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f137-123">Request headers</span></span>
| <span data-ttu-id="9f137-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f137-124">Header</span></span>       | <span data-ttu-id="9f137-125">Значение</span><span class="sxs-lookup"><span data-stu-id="9f137-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f137-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f137-126">Authorization</span></span>  | <span data-ttu-id="9f137-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f137-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f137-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f137-129">Request body</span></span>
<span data-ttu-id="9f137-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f137-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f137-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f137-131">Response</span></span>

<span data-ttu-id="9f137-132">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [вкладки](../resources/teamstab.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9f137-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f137-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f137-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f137-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f137-134">Request</span></span>
<span data-ttu-id="9f137-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f137-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
### <a name="response"></a><span data-ttu-id="9f137-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f137-136">Response</span></span>
<span data-ttu-id="9f137-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f137-137">The following is an example of the response.</span></span> 

><span data-ttu-id="9f137-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f137-138">**Note:** The response object shown here might be shortened for readability.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


