---
title: Создание команды из группы
description: Создание новой команды из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 685f727a6d70f691c23e28f82ee7642d0f3a7c70
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812987"
---
# <a name="create-team-from-group"></a><span data-ttu-id="3cf10-103">Создание команды из группы</span><span class="sxs-lookup"><span data-stu-id="3cf10-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> <span data-ttu-id="3cf10-104">Этот API-интерфейс находится в процессе замены на интерфейс [Создание команды](../api/team-post.md) и будет удален до конца 2019.</span><span class="sxs-lookup"><span data-stu-id="3cf10-104">This API is in the process of being depracated in favor of [Create team](../api/team-post.md), and will be removed by the end of 2019.</span></span> <span data-ttu-id="3cf10-105">Сведения о создании команды из группы см. в примерах 4 и 5 статьи [Создание команды](../api/team-post.md).</span><span class="sxs-lookup"><span data-stu-id="3cf10-105">For details about how to create a team from a group, see examples 4 and 5 in [Create team](../api/team-post.md).</span></span>

<span data-ttu-id="3cf10-106">Создание новой [команды](../resources/team.md) из [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="3cf10-106">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="3cf10-107">Чтобы создать команду, в группе должен быть хотя бы один владелец.</span><span class="sxs-lookup"><span data-stu-id="3cf10-107">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="3cf10-108">Если группа создана менее 15 минут назад, вызов метода "Создание команды" может завершиться ошибкой с кодом 404 из-за задержек репликации.</span><span class="sxs-lookup"><span data-stu-id="3cf10-108">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="3cf10-109">В качестве рекомендуемого шаблона следует повторить вызов метода "Создание команды" три раза с 10-секундной задержкой между вызовами.</span><span class="sxs-lookup"><span data-stu-id="3cf10-109">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cf10-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf10-110">Permissions</span></span>

<span data-ttu-id="3cf10-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cf10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cf10-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cf10-113">Permission type</span></span>      | <span data-ttu-id="3cf10-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cf10-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cf10-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cf10-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3cf10-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cf10-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3cf10-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cf10-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cf10-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cf10-118">Not supported.</span></span>    |
|<span data-ttu-id="3cf10-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cf10-119">Application</span></span> | <span data-ttu-id="3cf10-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cf10-120">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="3cf10-121">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3cf10-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3cf10-122">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к группам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="3cf10-122">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3cf10-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cf10-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="3cf10-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cf10-124">Request headers</span></span>

| <span data-ttu-id="3cf10-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cf10-125">Header</span></span>       | <span data-ttu-id="3cf10-126">Значение</span><span class="sxs-lookup"><span data-stu-id="3cf10-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cf10-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cf10-127">Authorization</span></span>  | <span data-ttu-id="3cf10-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cf10-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3cf10-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cf10-130">Content-Type</span></span>  | <span data-ttu-id="3cf10-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3cf10-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cf10-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cf10-132">Request body</span></span>

<span data-ttu-id="3cf10-133">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cf10-133">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3cf10-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf10-134">Response</span></span>

<span data-ttu-id="3cf10-135">При успешном выполнении этот метод должен вернуть код отклика `201 Created` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cf10-135">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cf10-136">Пример</span><span class="sxs-lookup"><span data-stu-id="3cf10-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3cf10-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cf10-137">Request</span></span>

<span data-ttu-id="3cf10-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cf10-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/beta/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```

#### <a name="response"></a><span data-ttu-id="3cf10-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cf10-139">Response</span></span>

<span data-ttu-id="3cf10-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3cf10-140">The following is an example of the response.</span></span> 

><span data-ttu-id="3cf10-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cf10-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="3cf10-143">См. также</span><span class="sxs-lookup"><span data-stu-id="3cf10-143">See also</span></span>

- [<span data-ttu-id="3cf10-144">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="3cf10-144">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
