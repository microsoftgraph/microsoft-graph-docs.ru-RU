---
title: 'Ветвь обновлений '
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d3d5fc3fbe63844e814dd0ce29d2cb656df2f22f
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843713"
---
# <a name="update-channel"></a><span data-ttu-id="3478e-103">Ветвь обновлений </span><span class="sxs-lookup"><span data-stu-id="3478e-103">Update channel</span></span>

<span data-ttu-id="3478e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3478e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3478e-105">Обновление свойств указанного [канала.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="3478e-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3478e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3478e-106">Permissions</span></span>

<span data-ttu-id="3478e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3478e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3478e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3478e-109">Permission type</span></span>      | <span data-ttu-id="3478e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3478e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3478e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3478e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3478e-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3478e-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3478e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3478e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3478e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3478e-114">Not supported.</span></span>    |
|<span data-ttu-id="3478e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3478e-115">Application</span></span> | <span data-ttu-id="3478e-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3478e-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="3478e-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="3478e-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="3478e-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3478e-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3478e-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="3478e-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3478e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3478e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3478e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3478e-121">Request headers</span></span>
| <span data-ttu-id="3478e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3478e-122">Header</span></span>       | <span data-ttu-id="3478e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3478e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3478e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3478e-124">Authorization</span></span>  | <span data-ttu-id="3478e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3478e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3478e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3478e-127">Content-Type</span></span>  | <span data-ttu-id="3478e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3478e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3478e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3478e-130">Request body</span></span>

<span data-ttu-id="3478e-131">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3478e-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="3478e-132">**Примечание.** Невозможно обновить значение `membershipType` существующего канала.</span><span class="sxs-lookup"><span data-stu-id="3478e-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="3478e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3478e-133">Response</span></span>

<span data-ttu-id="3478e-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3478e-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3478e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3478e-135">Example</span></span>

### <a name="example-1-update-channel"></a><span data-ttu-id="3478e-136">Пример 1. Канал обновления</span><span class="sxs-lookup"><span data-stu-id="3478e-136">Example 1: Update channel</span></span>

#### <a name="request"></a><span data-ttu-id="3478e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="3478e-137">Request</span></span>

<span data-ttu-id="3478e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3478e-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3478e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3478e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="3478e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3478e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3478e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3478e-141">Response</span></span>

<span data-ttu-id="3478e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3478e-142">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-channel-with-moderation-settings"></a><span data-ttu-id="3478e-143">Пример 2. Обновление канала с помощью параметров модерации</span><span class="sxs-lookup"><span data-stu-id="3478e-143">Example 2: Update channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="3478e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3478e-144">Request</span></span>

<span data-ttu-id="3478e-145">В следующем примере показан [](../resources/channelmoderationsettings.md) запрос на обновление параметров модерации канала.</span><span class="sxs-lookup"><span data-stu-id="3478e-145">The following example shows a request to update the [moderation settings](../resources/channelmoderationsettings.md) of a channel.</span></span> <span data-ttu-id="3478e-146">Эту операцию может выполнить только владелец команды.</span><span class="sxs-lookup"><span data-stu-id="3478e-146">This operation can only be performed by a team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="3478e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3478e-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3478e-148">C#</span><span class="sxs-lookup"><span data-stu-id="3478e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-channel-with-moderationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3478e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3478e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-channel-with-moderationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3478e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3478e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-with-moderationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3478e-151">Java</span><span class="sxs-lookup"><span data-stu-id="3478e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-channel-with-moderationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="3478e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3478e-152">Response</span></span>

<span data-ttu-id="3478e-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3478e-153">Here is an example of the response.</span></span> 

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


