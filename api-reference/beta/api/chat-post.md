---
title: Создание чата
description: Создание объекта чата.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1926ae37192a03ba8891aa321fa0c4f2da8c5796
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706355"
---
# <a name="create-chat"></a><span data-ttu-id="7ada8-103">Создание чата</span><span class="sxs-lookup"><span data-stu-id="7ada8-103">Create chat</span></span>
<span data-ttu-id="7ada8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ada8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ada8-105">Создание объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="7ada8-105">Create a new [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ada8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ada8-106">Permissions</span></span>
<span data-ttu-id="7ada8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ada8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ada8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ada8-109">Permission type</span></span>|<span data-ttu-id="7ada8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ada8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ada8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ada8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ada8-112">Chat.Create, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ada8-112">Chat.Create, Chat.ReadWrite</span></span>|
|<span data-ttu-id="7ada8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ada8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ada8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ada8-114">Not supported.</span></span> |
|<span data-ttu-id="7ada8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ada8-115">Application</span></span> | <span data-ttu-id="7ada8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ada8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ada8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ada8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats
```

## <a name="request-headers"></a><span data-ttu-id="7ada8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ada8-118">Request headers</span></span>
|<span data-ttu-id="7ada8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7ada8-119">Name</span></span>|<span data-ttu-id="7ada8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7ada8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7ada8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ada8-121">Authorization</span></span>|<span data-ttu-id="7ada8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ada8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7ada8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ada8-124">Content-Type</span></span>|<span data-ttu-id="7ada8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ada8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ada8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ada8-127">Request body</span></span>
<span data-ttu-id="7ada8-128">В теле запроса укажу представление объекта [чата](../resources/chat.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="7ada8-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="7ada8-129">В следующей таблице перечислены свойства, необходимые для создания объекта чата.</span><span class="sxs-lookup"><span data-stu-id="7ada8-129">The following table lists the properties that are required to create a chat object.</span></span>

|<span data-ttu-id="7ada8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ada8-130">Property</span></span>|<span data-ttu-id="7ada8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ada8-131">Type</span></span>|<span data-ttu-id="7ada8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ada8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ada8-133">topic</span><span class="sxs-lookup"><span data-stu-id="7ada8-133">topic</span></span>|<span data-ttu-id="7ada8-134">(Необязательно) Строка</span><span class="sxs-lookup"><span data-stu-id="7ada8-134">(Optional) String</span></span>|<span data-ttu-id="7ada8-135">Название чата.</span><span class="sxs-lookup"><span data-stu-id="7ada8-135">The title of the chat.</span></span> <span data-ttu-id="7ada8-136">Заголовок чата может быть предоставлен только в том случае, если чат имеет тип group.</span><span class="sxs-lookup"><span data-stu-id="7ada8-136">The chat title can be provided only if the chat is of 'group' type.</span></span>|
|<span data-ttu-id="7ada8-137">chatType</span><span class="sxs-lookup"><span data-stu-id="7ada8-137">chatType</span></span>|[<span data-ttu-id="7ada8-138">chatType</span><span class="sxs-lookup"><span data-stu-id="7ada8-138">chatType</span></span>](../resources/chat.md#chattype-values)| <span data-ttu-id="7ada8-139">Указывает тип чата.</span><span class="sxs-lookup"><span data-stu-id="7ada8-139">Specifies the type of chat.</span></span> <span data-ttu-id="7ada8-140">Возможные значения: `group` и `oneOnOne` .</span><span class="sxs-lookup"><span data-stu-id="7ada8-140">Possible values are:`group` and `oneOnOne`.</span></span> |
|<span data-ttu-id="7ada8-141">members</span><span class="sxs-lookup"><span data-stu-id="7ada8-141">members</span></span>|<span data-ttu-id="7ada8-142">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="7ada8-142">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="7ada8-143">Список участников беседы, которых следует добавить.</span><span class="sxs-lookup"><span data-stu-id="7ada8-143">List of conversation members that should be added.</span></span> <span data-ttu-id="7ada8-144">В этом списке должен быть указан каждый пользователь, включая пользователя, инициавшего запрос на создание, который будет участвовать в чате.</span><span class="sxs-lookup"><span data-stu-id="7ada8-144">Every single user, including the user initiating the create request, who will participate in the chat must be specified in this list.</span></span>|

## <a name="response"></a><span data-ttu-id="7ada8-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ada8-145">Response</span></span>

<span data-ttu-id="7ada8-146">В случае успеха этот метод возвращает код отклика 201 Created и новый ресурс **чата** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ada8-146">If successful, this method returns a 201 Created response code and the newly created **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ada8-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="7ada8-147">Examples</span></span>

### <a name="example-1-create-a-one-on-one-chat"></a><span data-ttu-id="7ada8-148">Пример 1. Создание чата с одним на одном</span><span class="sxs-lookup"><span data-stu-id="7ada8-148">Example 1: Create a one-on-one chat</span></span>

#### <a name="request"></a><span data-ttu-id="7ada8-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ada8-149">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chat_oneOnOne"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats
Content-Type: application/json

{
  "chatType": "oneOnOne",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"
    }
  ]
}
```
---

#### <a name="response"></a><span data-ttu-id="7ada8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ada8-150">Response</span></span>
><span data-ttu-id="7ada8-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7ada8-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2020-12-04T23:10:28.51Z",
    "lastUpdatedDateTime": "2020-12-04T23:10:28.51Z",
    "chatType": "oneOnOne"
}
```

### <a name="example-2-create-a-group-chat"></a><span data-ttu-id="7ada8-152">Пример 2. Создание группового чата</span><span class="sxs-lookup"><span data-stu-id="7ada8-152">Example 2: Create a group chat</span></span>

#### <a name="request"></a><span data-ttu-id="7ada8-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ada8-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chat_group"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats
Content-Type: application/json

{
  "chatType": "group",
  "topic": "Group chat title",
  "members": [
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
    },
    {
      "@odata.type": "#microsoft.graph.aadUserConversationMember",
      "roles": ["owner"],
      "user@odata.bind": "https://graph.microsoft.com/beta/users('3626a173-f2bc-4883-bcf7-01514c3bfb82')"
    }
  ]
}
```
---

#### <a name="response"></a><span data-ttu-id="7ada8-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ada8-154">Response</span></span>
><span data-ttu-id="7ada8-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7ada8-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:11:16.175Z",
    "chatType": "group"
}
```

