---
title: Создание группы
description: Создание новой группы в разделе группы.
ms.openlocfilehash: d7afffb331bf4a1714083ebb5f95147ec48a65d0
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222550"
---
# <a name="create-team"></a><span data-ttu-id="bfbcc-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="bfbcc-103">Create team</span></span>



<span data-ttu-id="bfbcc-104">Создание новой [группы](../resources/team.md) в разделе [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="bfbcc-104">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="bfbcc-105">Чтобы создать группу, группа должна иметь как минимум одной владелец.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="bfbcc-106">Если группа была создана не превышает 15 минут, можно для вызова команды Создать завершаются с кодом 404 ошибки из-за задержки репликации.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="bfbcc-107">Рекомендуемый шаблон является попыток вызова команды Создать в три раза с 10 секунда между вызовами.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfbcc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfbcc-108">Permissions</span></span>

<span data-ttu-id="bfbcc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfbcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfbcc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfbcc-111">Permission type</span></span>      | <span data-ttu-id="bfbcc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfbcc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfbcc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfbcc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bfbcc-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfbcc-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfbcc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfbcc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfbcc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-116">Not supported.</span></span>    |
|<span data-ttu-id="bfbcc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfbcc-117">Application</span></span> | <span data-ttu-id="bfbcc-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfbcc-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="bfbcc-119">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bfbcc-120">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к групп, которые они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bfbcc-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfbcc-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="bfbcc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfbcc-122">Request headers</span></span>

| <span data-ttu-id="bfbcc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfbcc-123">Header</span></span>       | <span data-ttu-id="bfbcc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bfbcc-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bfbcc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfbcc-125">Authorization</span></span>  | <span data-ttu-id="bfbcc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bfbcc-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfbcc-128">Content-Type</span></span>  | <span data-ttu-id="bfbcc-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bfbcc-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bfbcc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfbcc-130">Request body</span></span>

<span data-ttu-id="bfbcc-131">В тексте запроса укажите представление JSON объекта [группы](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="bfbcc-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bfbcc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfbcc-132">Response</span></span>

<span data-ttu-id="bfbcc-133">Если успешно завершена, этот метод должен возвращать `201 Created` код ответа и объекта [группы](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfbcc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="bfbcc-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bfbcc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfbcc-135">Request</span></span>

<span data-ttu-id="bfbcc-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
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

#### <a name="response"></a><span data-ttu-id="bfbcc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfbcc-137">Response</span></span>

<span data-ttu-id="bfbcc-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-138">The following is an example of the response.</span></span> 

><span data-ttu-id="bfbcc-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfbcc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bfbcc-141">См. также</span><span class="sxs-lookup"><span data-stu-id="bfbcc-141">See also</span></span>

- [<span data-ttu-id="bfbcc-142">Создание группы с группой</span><span class="sxs-lookup"><span data-stu-id="bfbcc-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
