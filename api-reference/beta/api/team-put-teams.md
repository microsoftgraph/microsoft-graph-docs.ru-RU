---
title: Создание команды из группы
description: Создание новой команды из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9950b92acb28d8138bba363170c8e1e89b5f1d5a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335273"
---
# <a name="create-team-from-group"></a><span data-ttu-id="51daf-103">Создание команды из группы</span><span class="sxs-lookup"><span data-stu-id="51daf-103">Create team from group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51daf-104">Создание новой [команды](../resources/team.md) из [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="51daf-104">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="51daf-105">Чтобы создать команду, в группе должен быть хотя бы один владелец.</span><span class="sxs-lookup"><span data-stu-id="51daf-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="51daf-106">Если группа создана менее 15 минут назад, вызов метода "Создание команды" может завершиться ошибкой с кодом 404 из-за задержек репликации.</span><span class="sxs-lookup"><span data-stu-id="51daf-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="51daf-107">В качестве рекомендуемого шаблона следует повторить вызов метода "Создание команды" три раза с 10-секундной задержкой между вызовами.</span><span class="sxs-lookup"><span data-stu-id="51daf-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="51daf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51daf-108">Permissions</span></span>

<span data-ttu-id="51daf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51daf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51daf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51daf-111">Permission type</span></span>      | <span data-ttu-id="51daf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51daf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51daf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51daf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="51daf-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51daf-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="51daf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51daf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51daf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51daf-116">Not supported.</span></span>    |
|<span data-ttu-id="51daf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51daf-117">Application</span></span> | <span data-ttu-id="51daf-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51daf-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="51daf-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="51daf-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="51daf-120">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к группам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="51daf-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="51daf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51daf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="51daf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51daf-122">Request headers</span></span>

| <span data-ttu-id="51daf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51daf-123">Header</span></span>       | <span data-ttu-id="51daf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="51daf-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51daf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51daf-125">Authorization</span></span>  | <span data-ttu-id="51daf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51daf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51daf-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51daf-128">Content-Type</span></span>  | <span data-ttu-id="51daf-129">application/json</span><span class="sxs-lookup"><span data-stu-id="51daf-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51daf-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51daf-130">Request body</span></span>

<span data-ttu-id="51daf-131">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51daf-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="51daf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="51daf-132">Response</span></span>

<span data-ttu-id="51daf-133">При успешном выполнении этот метод должен вернуть код отклика `201 Created` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51daf-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51daf-134">Пример</span><span class="sxs-lookup"><span data-stu-id="51daf-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="51daf-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="51daf-135">Request</span></span>

<span data-ttu-id="51daf-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51daf-136">The following is an example of the request.</span></span>
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
  }
}
```

#### <a name="response"></a><span data-ttu-id="51daf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="51daf-137">Response</span></span>

<span data-ttu-id="51daf-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51daf-138">The following is an example of the response.</span></span> 

><span data-ttu-id="51daf-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51daf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="51daf-141">См. также</span><span class="sxs-lookup"><span data-stu-id="51daf-141">See also</span></span>

- [<span data-ttu-id="51daf-142">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="51daf-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
