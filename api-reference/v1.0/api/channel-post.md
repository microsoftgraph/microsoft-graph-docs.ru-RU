---
title: Создание канала
description: Создайте новый канал в команде Майкрософт, как указано в теле запроса.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ec64a58a88d410abf84acbbb6fd92ccaf3940b3e
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848936"
---
# <a name="create-channel"></a><span data-ttu-id="cc49b-103">Создание канала</span><span class="sxs-lookup"><span data-stu-id="cc49b-103">Create channel</span></span>

<span data-ttu-id="cc49b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc49b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc49b-105">Создайте новый [канал](../resources/channel.md) в команде, как указано в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="cc49b-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc49b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc49b-106">Permissions</span></span>

<span data-ttu-id="cc49b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc49b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc49b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc49b-109">Permission type</span></span>      | <span data-ttu-id="cc49b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc49b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc49b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc49b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc49b-112">Channel. Create, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cc49b-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="cc49b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc49b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc49b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc49b-114">Not supported.</span></span>    |
|<span data-ttu-id="cc49b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc49b-115">Application</span></span> | <span data-ttu-id="cc49b-116">Channel. Create. Group \*, Channel. Create, Branch. Migrate. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cc49b-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cc49b-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="cc49b-117">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="cc49b-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="cc49b-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cc49b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc49b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="cc49b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc49b-120">Request headers</span></span>

| <span data-ttu-id="cc49b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc49b-121">Header</span></span>       | <span data-ttu-id="cc49b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc49b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc49b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc49b-123">Authorization</span></span>  | <span data-ttu-id="cc49b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc49b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc49b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc49b-126">Content-Type</span></span>  | <span data-ttu-id="cc49b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc49b-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc49b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc49b-129">Request body</span></span>

<span data-ttu-id="cc49b-130">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc49b-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc49b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc49b-131">Response</span></span>

<span data-ttu-id="cc49b-132">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc49b-132">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc49b-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc49b-133">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="cc49b-134">Пример 1: создание стандартного канала</span><span class="sxs-lookup"><span data-stu-id="cc49b-134">Example 1: Create a standard channel</span></span>
#### <a name="request"></a><span data-ttu-id="cc49b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc49b-135">Request</span></span>

<span data-ttu-id="cc49b-136">В приведенном ниже примере показан запрос на создание стандартного канала.</span><span class="sxs-lookup"><span data-stu-id="cc49b-136">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc49b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc49b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[<span data-ttu-id="cc49b-138">C#</span><span class="sxs-lookup"><span data-stu-id="cc49b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc49b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc49b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc49b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc49b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc49b-141">Java</span><span class="sxs-lookup"><span data-stu-id="cc49b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
---
#### <a name="response"></a><span data-ttu-id="cc49b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc49b-142">Response</span></span>

<span data-ttu-id="cc49b-143">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc49b-143">The following example shows the response.</span></span>

> <span data-ttu-id="cc49b-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc49b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="cc49b-146">Пример 2: создание закрытого канала от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="cc49b-146">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="cc49b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc49b-147">Request</span></span>

<span data-ttu-id="cc49b-148">В приведенном ниже примере показан запрос на создание закрытого канала и Добавление пользователя в качестве владельца группы.</span><span class="sxs-lookup"><span data-stu-id="cc49b-148">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc49b-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc49b-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{group_id}/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Graph.channel",
  "membershipType": "private",
  "displayName": "My First Private Channel",
  "description": "This is my first private channels",
  "members":
     [
        {
           "@odata.type":"#microsoft.graph.aadUserConversationMember",
           "user@odata.bind":"https://graph.microsoft.com/v1.0/users('{user_id}')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="c"></a>[<span data-ttu-id="cc49b-150">C#</span><span class="sxs-lookup"><span data-stu-id="cc49b-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc49b-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc49b-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc49b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc49b-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc49b-153">Java</span><span class="sxs-lookup"><span data-stu-id="cc49b-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cc49b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc49b-154">Response</span></span>

<span data-ttu-id="cc49b-155">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cc49b-155">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('{group_id}')/channels/$entity",
    "id": "{channel_id}",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/{channel_id}/My%20First%20Private%20Channel?groupId={group_id}&tenantId={tenant_id}",
    "membershipType": "private"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
