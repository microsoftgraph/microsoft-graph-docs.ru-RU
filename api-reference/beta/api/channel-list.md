---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: akjo
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: c864e2dd8da2dbf3e5239ecbaa747c28fb96c05e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059961"
---
# <a name="list-channels"></a><span data-ttu-id="ea270-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="ea270-103">List channels</span></span>

<span data-ttu-id="ea270-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea270-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea270-105">Получение списка [каналов](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ea270-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea270-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea270-106">Permissions</span></span>

<span data-ttu-id="ea270-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea270-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea270-109">Permission type</span></span>      | <span data-ttu-id="ea270-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea270-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea270-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea270-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea270-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea270-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ea270-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea270-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea270-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea270-114">Not supported.</span></span>    |
|<span data-ttu-id="ea270-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea270-115">Application</span></span> | <span data-ttu-id="ea270-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea270-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ea270-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="ea270-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="ea270-p102">**Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="ea270-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ea270-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea270-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea270-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea270-121">Optional query parameters</span></span>
<span data-ttu-id="ea270-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ea270-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

### <a name="use-select-for-better-performance"></a><span data-ttu-id="ea270-123">Использование $select для повышения производительности</span><span class="sxs-lookup"><span data-stu-id="ea270-123">Use $select for better performance</span></span>
<span data-ttu-id="ea270-124">Заполнение свойств **email** и **moderationSettings** для канала является затратной операцией, снижающей производительность.</span><span class="sxs-lookup"><span data-stu-id="ea270-124">Populating the **email** and **moderationSettings** properties for a channel is an expensive operation that results in slow performance.</span></span> <span data-ttu-id="ea270-125">Используйте `$select`, чтобы исключить свойства **email** и **moderationSettings** для повышения производительности.</span><span class="sxs-lookup"><span data-stu-id="ea270-125">Use `$select` to exclude the **email** and **moderationSettings** properties to improve performance.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ea270-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea270-126">Request headers</span></span>

| <span data-ttu-id="ea270-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea270-127">Header</span></span>       | <span data-ttu-id="ea270-128">Значение</span><span class="sxs-lookup"><span data-stu-id="ea270-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea270-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea270-129">Authorization</span></span>  | <span data-ttu-id="ea270-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea270-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea270-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea270-132">Request body</span></span>

<span data-ttu-id="ea270-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea270-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea270-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea270-134">Response</span></span>

<span data-ttu-id="ea270-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea270-135">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea270-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="ea270-136">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="ea270-137">Пример 1. Список всех каналов</span><span class="sxs-lookup"><span data-stu-id="ea270-137">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="ea270-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea270-138">Request</span></span>

<span data-ttu-id="ea270-139">Ниже показан пример запроса для получения списка всех каналов.</span><span class="sxs-lookup"><span data-stu-id="ea270-139">The following example shows a request to list all channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea270-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea270-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels
```
# <a name="c"></a>[<span data-ttu-id="ea270-141">C#</span><span class="sxs-lookup"><span data-stu-id="ea270-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea270-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea270-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea270-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea270-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea270-144">Java</span><span class="sxs-lookup"><span data-stu-id="ea270-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ea270-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea270-145">Response</span></span>

<span data-ttu-id="ea270-146">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="ea270-146">The following is the response.</span></span>

> <span data-ttu-id="ea270-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea270-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
      "membershipType": "standard"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="ea270-148">Пример 2. Список всех закрытых каналов</span><span class="sxs-lookup"><span data-stu-id="ea270-148">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="ea270-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea270-149">Request</span></span>

<span data-ttu-id="ea270-150">Ниже показан пример запроса для получения списка всех закрытых каналов.</span><span class="sxs-lookup"><span data-stu-id="ea270-150">The following example shows a request to list all private channels.</span></span>



# <a name="http"></a>[<span data-ttu-id="ea270-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea270-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="ea270-152">C#</span><span class="sxs-lookup"><span data-stu-id="ea270-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea270-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea270-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea270-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea270-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea270-155">Java</span><span class="sxs-lookup"><span data-stu-id="ea270-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="ea270-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea270-156">Response</span></span>

<span data-ttu-id="ea270-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ea270-157">The following is an example of the response.</span></span>

> <span data-ttu-id="ea270-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea270-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "id": "19:982abbfca323a582f0a6d00ae2deca@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "test private team",
      "membershipType": "private"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


