---
title: Перечисление каналов
description: Получение списка каналов в команде.
author: clearab
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1113880beb3386f5cd0c220028caa5e85f4de30b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288615"
---
# <a name="list-channels"></a><span data-ttu-id="37a5d-103">Перечисление каналов</span><span class="sxs-lookup"><span data-stu-id="37a5d-103">List channels</span></span>

<span data-ttu-id="37a5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a5d-105">Получение списка [каналов](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="37a5d-105">Retrieve the list of [channels](../resources/channel.md) in this [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37a5d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37a5d-106">Permissions</span></span>

<span data-ttu-id="37a5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37a5d-109">Permission type</span></span>      | <span data-ttu-id="37a5d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37a5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37a5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37a5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37a5d-112">Channel. ReadBasic. ALL, Чаннелсеттингс. Read. ALL, Чаннелсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37a5d-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="37a5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37a5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a5d-114">Not supported.</span></span>    |
|<span data-ttu-id="37a5d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37a5d-115">Application</span></span> | <span data-ttu-id="37a5d-116">Channel. ReadBasic. ALL, Чаннелсеттингс. Read. ALL, Чаннелсеттингс. ReadWrite. ALL, Чаннелсеттингс. Read. Group ([RSC](https://aka.ms/teams-rsc)), Чаннелсеттингс. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37a5d-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, ChannelSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), ChannelSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="37a5d-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="37a5d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="37a5d-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="37a5d-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="37a5d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37a5d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37a5d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37a5d-120">Optional query parameters</span></span>
<span data-ttu-id="37a5d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="37a5d-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37a5d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37a5d-122">Request headers</span></span>

| <span data-ttu-id="37a5d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37a5d-123">Header</span></span>       | <span data-ttu-id="37a5d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="37a5d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37a5d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37a5d-125">Authorization</span></span>  | <span data-ttu-id="37a5d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37a5d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37a5d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37a5d-128">Request body</span></span>

<span data-ttu-id="37a5d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37a5d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37a5d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a5d-130">Response</span></span>

<span data-ttu-id="37a5d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37a5d-131">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37a5d-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="37a5d-132">Examples</span></span>

### <a name="example-1-list-all-channels"></a><span data-ttu-id="37a5d-133">Пример 1. Список всех каналов</span><span class="sxs-lookup"><span data-stu-id="37a5d-133">Example 1: List all channels</span></span>

#### <a name="request"></a><span data-ttu-id="37a5d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a5d-134">Request</span></span>

<span data-ttu-id="37a5d-135">Ниже показан пример запроса для получения списка всех каналов.</span><span class="sxs-lookup"><span data-stu-id="37a5d-135">The following example shows a request to list all channels.</span></span>

# <a name="http"></a>[<span data-ttu-id="37a5d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a5d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
# <a name="c"></a>[<span data-ttu-id="37a5d-137">C#</span><span class="sxs-lookup"><span data-stu-id="37a5d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a5d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a5d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a5d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a5d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="37a5d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a5d-140">Response</span></span>

<span data-ttu-id="37a5d-141">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="37a5d-141">The following is the response.</span></span>

> <span data-ttu-id="37a5d-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37a5d-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="37a5d-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37a5d-143">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-all-private-channels"></a><span data-ttu-id="37a5d-144">Пример 2. Список всех закрытых каналов</span><span class="sxs-lookup"><span data-stu-id="37a5d-144">Example 2: List all private channels</span></span>

#### <a name="request"></a><span data-ttu-id="37a5d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a5d-145">Request</span></span>

<span data-ttu-id="37a5d-146">Ниже показан пример запроса для получения списка всех закрытых каналов.</span><span class="sxs-lookup"><span data-stu-id="37a5d-146">The following example shows a request to list all private channels.</span></span>


# <a name="http"></a>[<span data-ttu-id="37a5d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a5d-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_private_channels"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels?$filter=membershipType eq 'private'
```
# <a name="c"></a>[<span data-ttu-id="37a5d-148">C#</span><span class="sxs-lookup"><span data-stu-id="37a5d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-private-channels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a5d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a5d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-private-channels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a5d-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a5d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-private-channels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37a5d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a5d-151">Response</span></span>

<span data-ttu-id="37a5d-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="37a5d-152">The following is an example of the response.</span></span>

> <span data-ttu-id="37a5d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37a5d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
