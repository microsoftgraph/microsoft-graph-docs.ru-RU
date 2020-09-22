---
title: Создание команды из группы
description: Создание команды в группе.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2d71b43b578e6952c6a454fd45fe8ce327d9f907
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978456"
---
# <a name="create-team-from-group"></a><span data-ttu-id="ca65e-103">Создание команды из группы</span><span class="sxs-lookup"><span data-stu-id="ca65e-103">Create team from group</span></span>

<span data-ttu-id="ca65e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca65e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ca65e-105">Создание [команды](../resources/team.md) в [группе](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="ca65e-105">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="ca65e-106">Чтобы создать команду, в группе должен быть хотя бы один владелец.</span><span class="sxs-lookup"><span data-stu-id="ca65e-106">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="ca65e-107">Если группа создана менее 15 минут назад, вызов метода "Создание команды" может завершиться ошибкой с кодом 404 из-за задержек репликации.</span><span class="sxs-lookup"><span data-stu-id="ca65e-107">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="ca65e-108">В качестве рекомендуемого шаблона следует повторить вызов метода "Создание команды" три раза с 10-секундной задержкой между вызовами.</span><span class="sxs-lookup"><span data-stu-id="ca65e-108">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca65e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca65e-109">Permissions</span></span>

<span data-ttu-id="ca65e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca65e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca65e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca65e-112">Permission type</span></span>      | <span data-ttu-id="ca65e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca65e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca65e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca65e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ca65e-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca65e-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ca65e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca65e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca65e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca65e-117">Not supported.</span></span>    |
|<span data-ttu-id="ca65e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca65e-118">Application</span></span> | <span data-ttu-id="ca65e-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca65e-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ca65e-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ca65e-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ca65e-121">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к группам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="ca65e-121">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca65e-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca65e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="ca65e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca65e-123">Request headers</span></span>

| <span data-ttu-id="ca65e-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca65e-124">Header</span></span>       | <span data-ttu-id="ca65e-125">Значение</span><span class="sxs-lookup"><span data-stu-id="ca65e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca65e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca65e-126">Authorization</span></span>  | <span data-ttu-id="ca65e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca65e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ca65e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca65e-129">Content-Type</span></span>  | <span data-ttu-id="ca65e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ca65e-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca65e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca65e-131">Request body</span></span>

<span data-ttu-id="ca65e-132">Предоставьте в тексте запроса описание объекта [team](../resources/team.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca65e-132">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ca65e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca65e-133">Response</span></span>

<span data-ttu-id="ca65e-134">При успешном выполнении этот метод должен вернуть код отклика `201 Created` и объект [team](../resources/team.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca65e-134">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca65e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ca65e-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ca65e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca65e-136">Request</span></span>

<span data-ttu-id="ca65e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca65e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca65e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca65e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreatePrivateChannels": true,
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
# <a name="c"></a>[<span data-ttu-id="ca65e-139">C#</span><span class="sxs-lookup"><span data-stu-id="ca65e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca65e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca65e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca65e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca65e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca65e-142">Java</span><span class="sxs-lookup"><span data-stu-id="ca65e-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca65e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca65e-143">Response</span></span>

<span data-ttu-id="ca65e-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca65e-144">The following is an example of the response.</span></span> 

><span data-ttu-id="ca65e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca65e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="ca65e-147">См. также</span><span class="sxs-lookup"><span data-stu-id="ca65e-147">See also</span></span>

- [<span data-ttu-id="ca65e-148">Создание группы с командой</span><span class="sxs-lookup"><span data-stu-id="ca65e-148">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)

