---
title: Создание команды из группы
description: Создание новой команды из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6a4009c5fc6d9a421cfd5ffdae8c7ab4cc31d393
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054772"
---
# <a name="create-team-from-group"></a><span data-ttu-id="361b3-103">Создание команды из группы</span><span class="sxs-lookup"><span data-stu-id="361b3-103">Create team from group</span></span>

<span data-ttu-id="361b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="361b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> <span data-ttu-id="361b3-105">Этот API-интерфейс находится в процессе замены на интерфейс [Создание команды](../api/team-post.md) и будет удален до конца 2019.</span><span class="sxs-lookup"><span data-stu-id="361b3-105">This API is in the process of being deprecated in favor of [Create team](../api/team-post.md), and will be removed by the end of 2019.</span></span> <span data-ttu-id="361b3-106">Сведения о создании команды из группы см. в примерах 4 и 5 статьи [Создание команды](../api/team-post.md).</span><span class="sxs-lookup"><span data-stu-id="361b3-106">For details about how to create a team from a group, see examples 4 and 5 in [Create team](../api/team-post.md).</span></span>

<span data-ttu-id="361b3-107">Создание новой [команды](../resources/team.md) из [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="361b3-107">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="361b3-108">Чтобы создать команду, в группе должен быть хотя бы один владелец.</span><span class="sxs-lookup"><span data-stu-id="361b3-108">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="361b3-109">Если группа создана менее 15 минут назад, вызов метода "Создание команды" может завершиться ошибкой с кодом 404 из-за задержек репликации.</span><span class="sxs-lookup"><span data-stu-id="361b3-109">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="361b3-110">В качестве рекомендуемого шаблона следует повторить вызов метода "Создание команды" три раза с 10-секундной задержкой между вызовами.</span><span class="sxs-lookup"><span data-stu-id="361b3-110">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="361b3-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="361b3-111">Permissions</span></span>

<span data-ttu-id="361b3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="361b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="361b3-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="361b3-114">Permission type</span></span>      | <span data-ttu-id="361b3-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="361b3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="361b3-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="361b3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="361b3-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="361b3-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="361b3-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="361b3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="361b3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="361b3-119">Not supported.</span></span>    |
|<span data-ttu-id="361b3-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="361b3-120">Application</span></span> | <span data-ttu-id="361b3-121">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="361b3-121">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="361b3-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="361b3-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="361b3-123">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к группам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="361b3-123">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="361b3-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="361b3-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="361b3-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="361b3-125">Request headers</span></span>

| <span data-ttu-id="361b3-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="361b3-126">Header</span></span>       | <span data-ttu-id="361b3-127">Значение</span><span class="sxs-lookup"><span data-stu-id="361b3-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="361b3-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="361b3-128">Authorization</span></span>  | <span data-ttu-id="361b3-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="361b3-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="361b3-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="361b3-131">Content-Type</span></span>  | <span data-ttu-id="361b3-132">application/json</span><span class="sxs-lookup"><span data-stu-id="361b3-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="361b3-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="361b3-133">Request body</span></span>

<span data-ttu-id="361b3-134">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="361b3-134">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="361b3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="361b3-135">Response</span></span>

<span data-ttu-id="361b3-136">При успешном выполнении этот метод должен вернуть код отклика `201 Created` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="361b3-136">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="361b3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="361b3-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="361b3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="361b3-138">Request</span></span>

<span data-ttu-id="361b3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="361b3-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="361b3-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="361b3-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="361b3-141">C#</span><span class="sxs-lookup"><span data-stu-id="361b3-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="361b3-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="361b3-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="361b3-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="361b3-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="361b3-144">Java</span><span class="sxs-lookup"><span data-stu-id="361b3-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="361b3-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="361b3-145">Response</span></span>

<span data-ttu-id="361b3-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="361b3-146">The following is an example of the response.</span></span> 

><span data-ttu-id="361b3-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="361b3-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="see-also"></a><span data-ttu-id="361b3-148">См. также</span><span class="sxs-lookup"><span data-stu-id="361b3-148">See also</span></span>

- [<span data-ttu-id="361b3-149">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="361b3-149">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)


