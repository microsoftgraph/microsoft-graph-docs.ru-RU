---
title: Создание группы из группы
description: Создание новой группы из группы.
author: nkramer
ms.openlocfilehash: c9b3b686d9327872f7e5a68fe325141e256c6f53
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330298"
---
# <a name="create-team-from-group"></a><span data-ttu-id="539dc-103">Создание группы из группы</span><span class="sxs-lookup"><span data-stu-id="539dc-103">Create team from group</span></span>

> <span data-ttu-id="539dc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="539dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="539dc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="539dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="539dc-106">Создание новой [группы](../resources/team.md) из [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="539dc-106">Create a new [team](../resources/team.md) from a [group](../resources/group.md).</span></span>

<span data-ttu-id="539dc-107">Чтобы создать группу, группа должна иметь как минимум одной владелец.</span><span class="sxs-lookup"><span data-stu-id="539dc-107">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="539dc-108">Если группа была создана не превышает 15 минут, можно для вызова команды Создать завершаются с кодом 404 ошибки из-за задержки репликации.</span><span class="sxs-lookup"><span data-stu-id="539dc-108">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="539dc-109">Рекомендуемый шаблон является попыток вызова команды Создать в три раза с 10 секунда между вызовами.</span><span class="sxs-lookup"><span data-stu-id="539dc-109">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="539dc-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="539dc-110">Permissions</span></span>

<span data-ttu-id="539dc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="539dc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="539dc-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="539dc-113">Permission type</span></span>      | <span data-ttu-id="539dc-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="539dc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="539dc-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="539dc-115">Delegated (work or school account)</span></span> | <span data-ttu-id="539dc-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="539dc-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="539dc-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="539dc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="539dc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="539dc-118">Not supported.</span></span>    |
|<span data-ttu-id="539dc-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="539dc-119">Application</span></span> | <span data-ttu-id="539dc-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="539dc-120">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="539dc-121">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="539dc-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="539dc-122">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к групп, которые они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="539dc-122">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="539dc-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="539dc-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="539dc-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="539dc-124">Request headers</span></span>

| <span data-ttu-id="539dc-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="539dc-125">Header</span></span>       | <span data-ttu-id="539dc-126">Значение</span><span class="sxs-lookup"><span data-stu-id="539dc-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="539dc-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="539dc-127">Authorization</span></span>  | <span data-ttu-id="539dc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="539dc-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="539dc-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="539dc-130">Content-Type</span></span>  | <span data-ttu-id="539dc-131">application/json</span><span class="sxs-lookup"><span data-stu-id="539dc-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="539dc-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="539dc-132">Request body</span></span>

<span data-ttu-id="539dc-133">В тексте запроса укажите представление JSON объекта [группы](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="539dc-133">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="539dc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="539dc-134">Response</span></span>

<span data-ttu-id="539dc-135">Если успешно завершена, этот метод должен возвращать `201 Created` код ответа и объекта [группы](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="539dc-135">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="539dc-136">Пример</span><span class="sxs-lookup"><span data-stu-id="539dc-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="539dc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="539dc-137">Request</span></span>

<span data-ttu-id="539dc-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="539dc-138">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="539dc-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="539dc-139">Response</span></span>

<span data-ttu-id="539dc-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="539dc-140">The following is an example of the response.</span></span> 

><span data-ttu-id="539dc-p106">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="539dc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="539dc-143">См. также</span><span class="sxs-lookup"><span data-stu-id="539dc-143">See also</span></span>

- [<span data-ttu-id="539dc-144">Создание группы с группой</span><span class="sxs-lookup"><span data-stu-id="539dc-144">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
