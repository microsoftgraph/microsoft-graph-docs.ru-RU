---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 9984cfbaf303013bf06094b40b873137209c858a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959178"
---
# <a name="list-channels"></a><span data-ttu-id="cee08-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="cee08-103">List channels</span></span>

<span data-ttu-id="cee08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cee08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cee08-105">Получение списка [каналов](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="cee08-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cee08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cee08-106">Permissions</span></span>

<span data-ttu-id="cee08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cee08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cee08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cee08-109">Permission type</span></span>      | <span data-ttu-id="cee08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cee08-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cee08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cee08-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cee08-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee08-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="cee08-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cee08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cee08-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cee08-114">Not supported.</span></span>    |
|<span data-ttu-id="cee08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cee08-115">Application</span></span> | <span data-ttu-id="cee08-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group* , Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee08-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group* , Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cee08-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="cee08-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="cee08-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="cee08-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="cee08-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="cee08-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cee08-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cee08-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cee08-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cee08-121">Optional query parameters</span></span>
<span data-ttu-id="cee08-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cee08-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cee08-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cee08-123">Request headers</span></span>

| <span data-ttu-id="cee08-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cee08-124">Header</span></span>       | <span data-ttu-id="cee08-125">Значение</span><span class="sxs-lookup"><span data-stu-id="cee08-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cee08-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cee08-126">Authorization</span></span>  | <span data-ttu-id="cee08-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cee08-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cee08-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cee08-129">Request body</span></span>

<span data-ttu-id="cee08-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cee08-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cee08-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cee08-131">Response</span></span>

<span data-ttu-id="cee08-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cee08-132">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cee08-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="cee08-133">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="cee08-134">Пример 1. Список всех каналов</span><span class="sxs-lookup"><span data-stu-id="cee08-134">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="cee08-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cee08-135">Request</span></span>

<span data-ttu-id="cee08-136">Ниже показан пример запроса для получения списка всех каналов.</span><span class="sxs-lookup"><span data-stu-id="cee08-136">The following example shows a request to list all channels.</span></span>

# <a name="http"></a>[<span data-ttu-id="cee08-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cee08-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="c"></a>[<span data-ttu-id="cee08-138">C#</span><span class="sxs-lookup"><span data-stu-id="cee08-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cee08-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cee08-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cee08-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cee08-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cee08-141">Java</span><span class="sxs-lookup"><span data-stu-id="cee08-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cee08-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cee08-142">Response</span></span>

<span data-ttu-id="cee08-143">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="cee08-143">The following is the response.</span></span>

> <span data-ttu-id="cee08-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cee08-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cee08-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cee08-145">All the properties will be returned from an actual call.</span></span>

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
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
    }
  ]
}
```

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="cee08-146">Пример 2. Список всех закрытых каналов</span><span class="sxs-lookup"><span data-stu-id="cee08-146">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="cee08-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="cee08-147">Request</span></span>

<span data-ttu-id="cee08-148">Ниже показан пример запроса для получения списка всех закрытых каналов.</span><span class="sxs-lookup"><span data-stu-id="cee08-148">The following example shows a request to list all private channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="cee08-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="cee08-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="cee08-150">C#</span><span class="sxs-lookup"><span data-stu-id="cee08-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cee08-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cee08-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cee08-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cee08-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cee08-153">Java</span><span class="sxs-lookup"><span data-stu-id="cee08-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-private-channels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cee08-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="cee08-154">Response</span></span>

<span data-ttu-id="cee08-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cee08-155">The following is an example of the response.</span></span>

> <span data-ttu-id="cee08-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cee08-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value",
      "membershipType": "membership-type-value",
      "isFavoriteByDefault": false,
      "webUrl": "webUrl-value",
      "email": "email-value"
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


