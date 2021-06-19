---
title: Создание чата
description: Создайте новый объект чата.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ea5de5a32754125c5016bee536c8b8d1802a8d1
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030819"
---
# <a name="create-chat"></a><span data-ttu-id="9304f-103">Создание чата</span><span class="sxs-lookup"><span data-stu-id="9304f-103">Create chat</span></span>
<span data-ttu-id="9304f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9304f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9304f-105">Создайте новый [объект чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="9304f-105">Create a new [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9304f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9304f-106">Permissions</span></span>
<span data-ttu-id="9304f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9304f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9304f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9304f-109">Permission type</span></span>|<span data-ttu-id="9304f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9304f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9304f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9304f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9304f-112">Chat.Create, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9304f-112">Chat.Create, Chat.ReadWrite</span></span>|
|<span data-ttu-id="9304f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9304f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9304f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9304f-114">Not supported.</span></span> |
|<span data-ttu-id="9304f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9304f-115">Application</span></span> | <span data-ttu-id="9304f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9304f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9304f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9304f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats
```

## <a name="request-headers"></a><span data-ttu-id="9304f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9304f-118">Request headers</span></span>
|<span data-ttu-id="9304f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9304f-119">Name</span></span>|<span data-ttu-id="9304f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9304f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9304f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9304f-121">Authorization</span></span>|<span data-ttu-id="9304f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9304f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9304f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9304f-124">Content-Type</span></span>|<span data-ttu-id="9304f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9304f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9304f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9304f-127">Request body</span></span>
<span data-ttu-id="9304f-128">В теле запроса поставляем JSON-представление объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="9304f-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="9304f-129">В следующей таблице перечислены свойства, необходимые для создания объекта чата.</span><span class="sxs-lookup"><span data-stu-id="9304f-129">The following table lists the properties that are required to create a chat object.</span></span>

|<span data-ttu-id="9304f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9304f-130">Property</span></span>|<span data-ttu-id="9304f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9304f-131">Type</span></span>|<span data-ttu-id="9304f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9304f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9304f-133">topic</span><span class="sxs-lookup"><span data-stu-id="9304f-133">topic</span></span>|<span data-ttu-id="9304f-134">(Необязательный) String</span><span class="sxs-lookup"><span data-stu-id="9304f-134">(Optional) String</span></span>|<span data-ttu-id="9304f-135">Название чата.</span><span class="sxs-lookup"><span data-stu-id="9304f-135">The title of the chat.</span></span> <span data-ttu-id="9304f-136">Название чата может быть предоставлено только в том случае, если чат имеет `group` тип.</span><span class="sxs-lookup"><span data-stu-id="9304f-136">The chat title can be provided only if the chat is of `group` type.</span></span>|
|<span data-ttu-id="9304f-137">chatType</span><span class="sxs-lookup"><span data-stu-id="9304f-137">chatType</span></span>|[<span data-ttu-id="9304f-138">chatType</span><span class="sxs-lookup"><span data-stu-id="9304f-138">chatType</span></span>](../resources/chat.md#chattype-values)| <span data-ttu-id="9304f-139">Указывает тип чата.</span><span class="sxs-lookup"><span data-stu-id="9304f-139">Specifies the type of chat.</span></span> <span data-ttu-id="9304f-140">Возможные значения: `group` и `oneOnOne` .</span><span class="sxs-lookup"><span data-stu-id="9304f-140">Possible values are: `group` and `oneOnOne`.</span></span> |
|<span data-ttu-id="9304f-141">members</span><span class="sxs-lookup"><span data-stu-id="9304f-141">members</span></span>|<span data-ttu-id="9304f-142">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="9304f-142">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="9304f-143">Список участников беседы, которых следует добавить.</span><span class="sxs-lookup"><span data-stu-id="9304f-143">List of conversation members that should be added.</span></span> <span data-ttu-id="9304f-144">Каждый пользователь, включая пользователя, инициавшего запрос на создание, который будет участвовать в чате, должен быть указан в этом списке.</span><span class="sxs-lookup"><span data-stu-id="9304f-144">Every single user, including the user initiating the create request, who will participate in the chat must be specified in this list.</span></span>|
|<span data-ttu-id="9304f-145">installedApps</span><span class="sxs-lookup"><span data-stu-id="9304f-145">installedApps</span></span>| <span data-ttu-id="9304f-146">Коллекция [teamsApp](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="9304f-146">[teamsApp](../resources/teamsapp.md) collection</span></span>|<span data-ttu-id="9304f-147">Список приложений, которые необходимо установить в чате.</span><span class="sxs-lookup"><span data-stu-id="9304f-147">List of apps that should be installed in the chat.</span></span>|

> <span data-ttu-id="9304f-148">**Примечание:** В настоящее время поддерживается только одна установка приложения.</span><span class="sxs-lookup"><span data-stu-id="9304f-148">**Note:** Currently, only one app installation is supported.</span></span> <span data-ttu-id="9304f-149">Если в запросе перечислены несколько установок приложений, ответ будет `Bad Request` ошибкой.</span><span class="sxs-lookup"><span data-stu-id="9304f-149">If multiple app installations are listed in the request, the response will be a `Bad Request` error.</span></span>

## <a name="response"></a><span data-ttu-id="9304f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9304f-150">Response</span></span>

### <a name="response-for-creating-a-one-on-one-chat-without-installed-apps"></a><span data-ttu-id="9304f-151">Ответ на создание единого чата без установленных приложений</span><span class="sxs-lookup"><span data-stu-id="9304f-151">Response for creating a one-on-one chat without installed apps</span></span>
<span data-ttu-id="9304f-152">В случае успешного использования этот метод возвращает код отклика и вновь созданный ресурс чата `201 Created` в тексте [](../resources/chat.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="9304f-152">If successful, this method returns a `201 Created` response code and the newly created [chat](../resources/chat.md) resource in the response body.</span></span>

### <a name="response-for-creating-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="9304f-153">Ответ на создание единого чата с установленными приложениями</span><span class="sxs-lookup"><span data-stu-id="9304f-153">Response for creating a one-on-one chat with installed apps</span></span>
<span data-ttu-id="9304f-154">В случае успешной работы этот метод возвращает код ответа и загон расположения, содержащий ссылку на `202 Accepted` [teamsAsyncOperation.](../resources/teamsasyncoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9304f-154">If successful, this method returns a `202 Accepted` response code and Location header that contains a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="9304f-155">Ссылку можно использовать для получения состояния и сведений об операции.</span><span class="sxs-lookup"><span data-stu-id="9304f-155">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="9304f-156">Подробные сведения см. в [материале Get operation on chat.](teamsasyncoperation-get.md#example-get-operation-on-chat)</span><span class="sxs-lookup"><span data-stu-id="9304f-156">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="examples"></a><span data-ttu-id="9304f-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="9304f-157">Examples</span></span>

### <a name="example-1-create-a-one-on-one-chat"></a><span data-ttu-id="9304f-158">Пример 1. Создание чата один на один</span><span class="sxs-lookup"><span data-stu-id="9304f-158">Example 1: Create a one-on-one chat</span></span>

#### <a name="request"></a><span data-ttu-id="9304f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9304f-159">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="9304f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9304f-160">Response</span></span>
><span data-ttu-id="9304f-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9304f-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "chatType": "oneOnOne",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A82fe7758-5bb3-4f0d-a43f-e555fd399c6f_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

### <a name="example-2-create-a-group-chat"></a><span data-ttu-id="9304f-162">Пример 2. Создание группового чата</span><span class="sxs-lookup"><span data-stu-id="9304f-162">Example 2: Create a group chat</span></span>

#### <a name="request"></a><span data-ttu-id="9304f-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9304f-163">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="9304f-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="9304f-164">Response</span></span>
><span data-ttu-id="9304f-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9304f-165">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "chatType": "group",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A1c5b01696d2e4a179c292bc9cf04e63b@thread.v2/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

### <a name="example-3-create-a-one-on-one-chat-with-installed-apps"></a><span data-ttu-id="9304f-166">Пример 3. Создание чата один на один с установленными приложениями</span><span class="sxs-lookup"><span data-stu-id="9304f-166">Example 3: Create a one-on-one chat with installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="9304f-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="9304f-167">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chat_oneOnOne_with_installed_apps"
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
  ],
  "installedApps": [
    {
      "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4"
    }
  ]
}
```

---

#### <a name="response"></a><span data-ttu-id="9304f-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="9304f-168">Response</span></span>
><span data-ttu-id="9304f-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9304f-169">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /chats('19:82fe7758-5bb3-4f0d-a43f-e555fd399c6f_bfb5bb25-3a8d-487d-9828-7875ced51a30@unq.gbl.spaces')/operations('2432b57b-0abd-43db-aa7b-16eadd115d34-861f06db-0208-4815-b67a-965df0d28b7f-10adc8a6-60db-42e2-9761-e56a7e4c7bc9')
```

<span data-ttu-id="9304f-170">Инициирована операция async, и в ответе содержится загон Location, который включает ссылку на [teamsAsyncOperation.](../resources/teamsasyncoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9304f-170">The async operation is initiated, and the response contains a Location header which includes a link to the to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span> <span data-ttu-id="9304f-171">Ссылку можно использовать для получения состояния и сведений об операции.</span><span class="sxs-lookup"><span data-stu-id="9304f-171">The link can be used to get the operation status and details.</span></span> <span data-ttu-id="9304f-172">Подробные сведения см. в [материале Get operation on chat.](teamsasyncoperation-get.md#example-get-operation-on-chat)</span><span class="sxs-lookup"><span data-stu-id="9304f-172">For details, see [Get operation on chat](teamsasyncoperation-get.md#example-get-operation-on-chat).</span></span>

## <a name="see-also"></a><span data-ttu-id="9304f-173">См. также</span><span class="sxs-lookup"><span data-stu-id="9304f-173">See also</span></span>
- [<span data-ttu-id="9304f-174">Get teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="9304f-174">Get teamsAsyncOperation</span></span>](teamsasyncoperation-get.md)
