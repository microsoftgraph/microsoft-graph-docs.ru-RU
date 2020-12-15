---
title: Список участников группы
description: Получение conversationMembers группы.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8afc1f6cadb6f8fc7227d279c8effe8e5b92ee2f
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660123"
---
# <a name="list-members-of-team"></a><span data-ttu-id="c3d37-103">Список участников группы</span><span class="sxs-lookup"><span data-stu-id="c3d37-103">List members of team</span></span>
<span data-ttu-id="c3d37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3d37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3d37-105">Получение коллекции [conversationMember](../resources/conversationmember.md) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c3d37-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="c3d37-106">Идентификаторы членства, возвращаемые сервером, должны рассматриваться как непрозрачные строки.</span><span class="sxs-lookup"><span data-stu-id="c3d37-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="c3d37-107">Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c3d37-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="c3d37-108">В дальнейшем результаты членства могут сопоставляться с пользователями различных клиентов, как указано в отклике.</span><span class="sxs-lookup"><span data-stu-id="c3d37-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="c3d37-109">Клиент не должен предполагать, что все участники относятся только к текущему клиенту.</span><span class="sxs-lookup"><span data-stu-id="c3d37-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3d37-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d37-110">Permissions</span></span>
<span data-ttu-id="c3d37-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3d37-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3d37-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3d37-113">Permission type</span></span>|<span data-ttu-id="c3d37-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3d37-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3d37-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3d37-115">Delegated (work or school account)</span></span>| <span data-ttu-id="c3d37-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3d37-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="c3d37-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3d37-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3d37-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3d37-118">Not supported.</span></span>    |
|<span data-ttu-id="c3d37-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3d37-119">Application</span></span>| <span data-ttu-id="c3d37-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3d37-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="c3d37-121">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="c3d37-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="c3d37-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3d37-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3d37-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3d37-123">Optional query parameters</span></span>
<span data-ttu-id="c3d37-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c3d37-124">This method supports the `$filter` and `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3d37-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3d37-125">Request headers</span></span>
|<span data-ttu-id="c3d37-126">Имя</span><span class="sxs-lookup"><span data-stu-id="c3d37-126">Name</span></span>|<span data-ttu-id="c3d37-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c3d37-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3d37-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3d37-128">Authorization</span></span>|<span data-ttu-id="c3d37-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3d37-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3d37-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3d37-131">Request body</span></span>
<span data-ttu-id="c3d37-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3d37-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3d37-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d37-133">Response</span></span>

<span data-ttu-id="c3d37-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3d37-134">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3d37-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="c3d37-135">Examples</span></span>

### <a name="example-1-get-list-of-members-in-team"></a><span data-ttu-id="c3d37-136">Пример 1. Получение списка участников команды</span><span class="sxs-lookup"><span data-stu-id="c3d37-136">Example 1: Get list of members in team</span></span>

#### <a name="request"></a><span data-ttu-id="c3d37-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d37-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```

#### <a name="response"></a><span data-ttu-id="c3d37-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d37-138">Response</span></span>
><span data-ttu-id="c3d37-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3d37-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 3,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyM3NTJmNTBiNy0yNTZmLTQ1MzktYjc3NS1jNGQxMmYyZTQ3MjI=",
            "roles": [],
            "displayName": "Harry Johnson",
            "userId": "752f50b7-256f-4539-b775-c4d12f2e4722",
            "email": "harry@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

### <a name="example-2-find-members-of-a-team-by-their-azure-ad-user-object-id"></a><span data-ttu-id="c3d37-140">Пример 2. Поиск участников команды по ИД объекта пользователя Azure AD</span><span class="sxs-lookup"><span data-stu-id="c3d37-140">Example 2: Find members of a team by their Azure AD user object ID</span></span>

<span data-ttu-id="c3d37-141">В следующем примере показан запрос на поиск ресурсов участия на основе `id` [пользователя Azure AD](../resources/user.md), связанного с [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="c3d37-141">The following example shows a request to find the membership resources based on `id` of the [Azure AD user](../resources/user.md) associated with the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="c3d37-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d37-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_userid"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')

```

#### <a name="response"></a><span data-ttu-id="c3d37-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d37-143">Response</span></span>
><span data-ttu-id="c3d37-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3d37-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_userid",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

### <a name="example-3-find-members-of-a-team-by-their-names-or-email"></a><span data-ttu-id="c3d37-145">Пример 3. Поиск участников команды по именам или адресам электронной почты</span><span class="sxs-lookup"><span data-stu-id="c3d37-145">Example 3: Find members of a team by their names or email</span></span>

<span data-ttu-id="c3d37-146">В следующем примере показан запрос на поиск ресурсов участия на основе `displayName` или `email` ресурса [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="c3d37-146">The following example shows a request to find the membership resources based on `displayName` or `email` of the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="c3d37-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d37-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_username_or_email"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')
```

#### <a name="response"></a><span data-ttu-id="c3d37-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d37-148">Response</span></span>
><span data-ttu-id="c3d37-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3d37-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_username_or_email",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyM3NTJmNTBiNy0yNTZmLTQ1MzktYjc3NS1jNGQxMmYyZTQ3MjI=",
            "roles": [],
            "displayName": "Harry Johnson",
            "userId": "752f50b7-256f-4539-b775-c4d12f2e4722",
            "email": "harry@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

### <a name="example-4-list-only-those-members-who-are-owners-of-the-team"></a><span data-ttu-id="c3d37-150">Пример 4. Перечисление только тех участников, которые являются *владельцами* команды</span><span class="sxs-lookup"><span data-stu-id="c3d37-150">Example 4: List only those members who are *owners* of the team</span></span>

<span data-ttu-id="c3d37-151">В следующем примере показан запрос на поиск всех участников, которым назначена роль *владельца*.</span><span class="sxs-lookup"><span data-stu-id="c3d37-151">The following example shows a request to find all the members who are have *owner* role attached to them.</span></span>

> [!NOTE]
> <span data-ttu-id="c3d37-152">С этой функцией связаны некоторые известные проблемы.</span><span class="sxs-lookup"><span data-stu-id="c3d37-152">There are some known issues with this functionality.</span></span> <span data-ttu-id="c3d37-153">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues.md#unable-to-filter-team-members-by-roles).</span><span class="sxs-lookup"><span data-stu-id="c3d37-153">For details, see [known issues](/graph/known-issues.md#unable-to-filter-team-members-by-roles).</span></span>

#### <a name="request"></a><span data-ttu-id="c3d37-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3d37-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_owner_role"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=roles/any(r:r eq 'owner')
```

#### <a name="response"></a><span data-ttu-id="c3d37-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3d37-155">Response</span></span>
><span data-ttu-id="c3d37-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3d37-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_owner_role",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="c3d37-157">См. также</span><span class="sxs-lookup"><span data-stu-id="c3d37-157">See also</span></span>

- [<span data-ttu-id="c3d37-158">Список участников в канале</span><span class="sxs-lookup"><span data-stu-id="c3d37-158">List members in channel</span></span>](channel-list-members.md)
