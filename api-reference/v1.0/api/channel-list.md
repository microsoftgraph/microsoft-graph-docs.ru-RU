---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 967a8cbfc1a3ec909b3fb7e5e36c7c3e7f00730a
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509247"
---
# <a name="list-channels"></a><span data-ttu-id="522f6-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="522f6-103">List channels</span></span>

<span data-ttu-id="522f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="522f6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="522f6-105">Получение списка [каналов](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="522f6-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="522f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="522f6-106">Permissions</span></span>

<span data-ttu-id="522f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="522f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="522f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="522f6-109">Permission type</span></span>      | <span data-ttu-id="522f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="522f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="522f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="522f6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="522f6-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522f6-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="522f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="522f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="522f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="522f6-114">Not supported.</span></span>    |
|<span data-ttu-id="522f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="522f6-115">Application</span></span> | <span data-ttu-id="522f6-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522f6-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="522f6-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="522f6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="522f6-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="522f6-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="522f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="522f6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="522f6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="522f6-120">Optional query parameters</span></span>

<span data-ttu-id="522f6-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="522f6-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="522f6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="522f6-122">Request headers</span></span>

| <span data-ttu-id="522f6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="522f6-123">Header</span></span>       | <span data-ttu-id="522f6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="522f6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="522f6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="522f6-125">Authorization</span></span>  | <span data-ttu-id="522f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="522f6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="522f6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="522f6-128">Request body</span></span>

<span data-ttu-id="522f6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="522f6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="522f6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="522f6-130">Response</span></span>

<span data-ttu-id="522f6-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="522f6-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="522f6-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="522f6-132">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="522f6-133">Пример 1. Список всех каналов</span><span class="sxs-lookup"><span data-stu-id="522f6-133">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="522f6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="522f6-134">Request</span></span>

<span data-ttu-id="522f6-135">Ниже показан пример запроса для получения списка всех каналов.</span><span class="sxs-lookup"><span data-stu-id="522f6-135">The following example shows a request to list all channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="522f6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="522f6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels
```
# <a name="c"></a>[<span data-ttu-id="522f6-137">C#</span><span class="sxs-lookup"><span data-stu-id="522f6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="522f6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="522f6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="522f6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="522f6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="522f6-140">Java</span><span class="sxs-lookup"><span data-stu-id="522f6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="522f6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="522f6-141">Response</span></span>

<span data-ttu-id="522f6-142">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="522f6-142">The following is the response.</span></span>

> <span data-ttu-id="522f6-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="522f6-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="522f6-144">Пример 2. Список всех закрытых каналов</span><span class="sxs-lookup"><span data-stu-id="522f6-144">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="522f6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="522f6-145">Request</span></span>

<span data-ttu-id="522f6-146">Ниже показан пример запроса для получения списка всех закрытых каналов.</span><span class="sxs-lookup"><span data-stu-id="522f6-146">The following example shows a request to list all private channels.</span></span>



# <a name="http"></a>[<span data-ttu-id="522f6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="522f6-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="522f6-148">C#</span><span class="sxs-lookup"><span data-stu-id="522f6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="522f6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="522f6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="522f6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="522f6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="522f6-151">Java</span><span class="sxs-lookup"><span data-stu-id="522f6-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="522f6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="522f6-152">Response</span></span>

<span data-ttu-id="522f6-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="522f6-153">The following is an example of the response.</span></span>

> <span data-ttu-id="522f6-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="522f6-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
