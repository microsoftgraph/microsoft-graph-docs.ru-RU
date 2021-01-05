---
title: 'Ветвь обновлений '
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a23916c9941afd17064e75add3e7c5ca5480fa54
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753471"
---
# <a name="update-channel"></a><span data-ttu-id="1bd8c-103">Ветвь обновлений </span><span class="sxs-lookup"><span data-stu-id="1bd8c-103">Update channel</span></span>

<span data-ttu-id="1bd8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bd8c-105">Обновление свойств указанного [канала.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="1bd8c-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bd8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd8c-106">Permissions</span></span>

<span data-ttu-id="1bd8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd8c-109">Permission type</span></span>      | <span data-ttu-id="1bd8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bd8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bd8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bd8c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1bd8c-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd8c-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1bd8c-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bd8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bd8c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-114">Not supported.</span></span>    |
|<span data-ttu-id="1bd8c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1bd8c-115">Application</span></span> | <span data-ttu-id="1bd8c-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd8c-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1bd8c-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1bd8c-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="1bd8c-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1bd8c-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1bd8c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bd8c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1bd8c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bd8c-121">Request headers</span></span>
| <span data-ttu-id="1bd8c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bd8c-122">Header</span></span>       | <span data-ttu-id="1bd8c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1bd8c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bd8c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bd8c-124">Authorization</span></span>  | <span data-ttu-id="1bd8c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1bd8c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1bd8c-127">Content-Type</span></span>  | <span data-ttu-id="1bd8c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bd8c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bd8c-130">Request body</span></span>

<span data-ttu-id="1bd8c-131">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="1bd8c-132">**Примечание.** Невозможно обновить значение `membershipType` существующего канала.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="1bd8c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bd8c-133">Response</span></span>

<span data-ttu-id="1bd8c-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1bd8c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="1bd8c-135">Example</span></span>

### <a name="example-1-update-channel"></a><span data-ttu-id="1bd8c-136">Пример 1. Канал обновления</span><span class="sxs-lookup"><span data-stu-id="1bd8c-136">Example 1: Update channel</span></span>

#### <a name="request"></a><span data-ttu-id="1bd8c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bd8c-137">Request</span></span>

<span data-ttu-id="1bd8c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1bd8c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd8c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="1bd8c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bd8c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1bd8c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bd8c-141">Response</span></span>

<span data-ttu-id="1bd8c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-channel-with-moderation-settings"></a><span data-ttu-id="1bd8c-143">Пример 2. Обновление канала с помощью параметров модерации</span><span class="sxs-lookup"><span data-stu-id="1bd8c-143">Example 2: Update channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="1bd8c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bd8c-144">Request</span></span>

<span data-ttu-id="1bd8c-145">В следующем примере показан [](../resources/channelmoderationsettings.md) запрос на обновление параметров модерации канала.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-145">The following example shows a request to update the [moderation settings](../resources/channelmoderationsettings.md) of a channel.</span></span> <span data-ttu-id="1bd8c-146">Эту операцию может выполнить только владелец команды.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-146">This operation can only be performed by a team owner.</span></span>

<!-- {
  "blockType": "request",
  "name": "patch_channel_with_moderationSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{team-id}/channels/{channel-id}
Content-type: application/json

{
    "displayName": "UpdateChannelModeration",
    "description": "Update channel moderation.",
    "moderationSettings": {
        "userNewMessageRestriction": "moderators",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```


#### <a name="response"></a><span data-ttu-id="1bd8c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bd8c-147">Response</span></span>

<span data-ttu-id="1bd8c-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1bd8c-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


