---
title: Получение команды
description: Получение свойств и связей указанной команды.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bcf63579b4ade651df30e4ace287aaa15baae6e4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202214"
---
# <a name="get-team"></a><span data-ttu-id="f0133-103">Получение команды</span><span class="sxs-lookup"><span data-stu-id="f0133-103">Get team</span></span>

<span data-ttu-id="f0133-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0133-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f0133-105">Получение свойств и связей указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f0133-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0133-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0133-106">Permissions</span></span>
<span data-ttu-id="f0133-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0133-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0133-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0133-109">Permission type</span></span>      | <span data-ttu-id="f0133-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0133-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0133-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0133-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0133-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0133-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f0133-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0133-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0133-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0133-114">Not supported.</span></span>    |
|<span data-ttu-id="f0133-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0133-115">Application</span></span> | <span data-ttu-id="f0133-116">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0133-116">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f0133-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="f0133-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="f0133-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f0133-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f0133-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="f0133-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f0133-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0133-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0133-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0133-121">Optional query parameters</span></span>
<span data-ttu-id="f0133-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f0133-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0133-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0133-123">Request headers</span></span>
| <span data-ttu-id="f0133-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0133-124">Header</span></span>       | <span data-ttu-id="f0133-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f0133-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0133-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0133-126">Authorization</span></span>  | <span data-ttu-id="f0133-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0133-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0133-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0133-129">Request body</span></span>
<span data-ttu-id="f0133-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0133-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0133-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0133-131">Response</span></span>

<span data-ttu-id="f0133-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0133-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0133-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f0133-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f0133-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0133-134">Request</span></span>
<span data-ttu-id="f0133-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0133-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265
```


#### <a name="response"></a><span data-ttu-id="f0133-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0133-136">Response</span></span>
<span data-ttu-id="f0133-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0133-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f0133-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f0133-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived": false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

