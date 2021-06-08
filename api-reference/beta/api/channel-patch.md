---
title: 'Ветвь обновлений '
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8527ae77c6198aea615aff8add5a569dc563bafa
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786217"
---
# <a name="update-channel"></a><span data-ttu-id="3ea49-103">Ветвь обновлений </span><span class="sxs-lookup"><span data-stu-id="3ea49-103">Update channel</span></span>

<span data-ttu-id="3ea49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ea49-105">Обновление свойств указанного [канала.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="3ea49-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ea49-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea49-106">Permissions</span></span>

<span data-ttu-id="3ea49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ea49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ea49-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea49-109">Permission type</span></span>      | <span data-ttu-id="3ea49-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ea49-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ea49-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ea49-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ea49-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ea49-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3ea49-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ea49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ea49-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ea49-114">Not supported.</span></span>    |
|<span data-ttu-id="3ea49-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3ea49-115">Application</span></span> | <span data-ttu-id="3ea49-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ea49-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="3ea49-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="3ea49-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="3ea49-p102">**Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="3ea49-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ea49-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ea49-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}/channels/{channel-id}
```
## <a name="request-headers"></a><span data-ttu-id="3ea49-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ea49-121">Request headers</span></span>
| <span data-ttu-id="3ea49-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ea49-122">Header</span></span>       | <span data-ttu-id="3ea49-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3ea49-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ea49-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ea49-124">Authorization</span></span>  | <span data-ttu-id="3ea49-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea49-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ea49-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ea49-127">Content-Type</span></span>  | <span data-ttu-id="3ea49-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea49-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ea49-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ea49-130">Request body</span></span>

<span data-ttu-id="3ea49-131">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ea49-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="3ea49-132">**Примечание:** Невозможно обновить `membershipType` значение для существующего канала.</span><span class="sxs-lookup"><span data-stu-id="3ea49-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="3ea49-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea49-133">Response</span></span>

<span data-ttu-id="3ea49-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3ea49-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3ea49-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3ea49-135">Example</span></span>

### <a name="example-1-update-channel"></a><span data-ttu-id="3ea49-136">Пример 1. Канал обновления</span><span class="sxs-lookup"><span data-stu-id="3ea49-136">Example 1: Update channel</span></span>

#### <a name="request"></a><span data-ttu-id="3ea49-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea49-137">Request</span></span>

<span data-ttu-id="3ea49-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ea49-138">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```


#### <a name="response"></a><span data-ttu-id="3ea49-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea49-139">Response</span></span>

<span data-ttu-id="3ea49-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ea49-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-channel-with-moderation-settings"></a><span data-ttu-id="3ea49-141">Пример 2. Обновление канала с настройками модерации</span><span class="sxs-lookup"><span data-stu-id="3ea49-141">Example 2: Update channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="3ea49-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea49-142">Request</span></span>

<span data-ttu-id="3ea49-143">В следующем примере показан запрос на обновление [параметров модерации](../resources/channelmoderationsettings.md) канала.</span><span class="sxs-lookup"><span data-stu-id="3ea49-143">The following example shows a request to update the [moderation settings](../resources/channelmoderationsettings.md) of a channel.</span></span> <span data-ttu-id="3ea49-144">Эта операция может выполняться только владельцем группы.</span><span class="sxs-lookup"><span data-stu-id="3ea49-144">This operation can only be performed by a team owner.</span></span>



# <a name="http"></a>[<span data-ttu-id="3ea49-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ea49-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel_with_moderationSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
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
# <a name="c"></a>[<span data-ttu-id="3ea49-146">C#</span><span class="sxs-lookup"><span data-stu-id="3ea49-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-channel-with-moderationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ea49-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ea49-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-channel-with-moderationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ea49-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ea49-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-with-moderationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ea49-149">Java</span><span class="sxs-lookup"><span data-stu-id="3ea49-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-channel-with-moderationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="3ea49-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea49-150">Response</span></span>

<span data-ttu-id="3ea49-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ea49-151">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
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


