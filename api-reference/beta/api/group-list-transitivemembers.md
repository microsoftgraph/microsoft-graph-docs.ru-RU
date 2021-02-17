---
title: Перечисление транзитивных участников группы
description: Получите список членов группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9b7f5a95498ca9a7e5bd502d5a1d9f40479d0cf3
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271973"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="79328-103">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="79328-103">List group transitive members</span></span>

<span data-ttu-id="79328-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79328-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79328-105">Получите список членов группы.</span><span class="sxs-lookup"><span data-stu-id="79328-105">Get a list of the group's members.</span></span> <span data-ttu-id="79328-106">В качестве членов группы могут быть пользователи, контакты, устройства, участники-службы и другие группы.</span><span class="sxs-lookup"><span data-stu-id="79328-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="79328-107">Эта операция является транзитивной и также возвращает плоский список всех вложенных членов.</span><span class="sxs-lookup"><span data-stu-id="79328-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="79328-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79328-108">Permissions</span></span>

<span data-ttu-id="79328-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79328-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79328-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79328-111">Permission type</span></span> | <span data-ttu-id="79328-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79328-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="79328-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79328-113">Delegated (work or school account)</span></span> | <span data-ttu-id="79328-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="79328-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="79328-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79328-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79328-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79328-116">Not supported.</span></span> |
| <span data-ttu-id="79328-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79328-117">Application</span></span> | <span data-ttu-id="79328-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="79328-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="79328-119">**Примечание.** Для получения списка участников скрытой группы членства требуется разрешение Member.Read.Hidden.</span><span class="sxs-lookup"><span data-stu-id="79328-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="79328-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79328-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79328-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79328-121">Optional query parameters</span></span>

<span data-ttu-id="79328-122">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="79328-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="79328-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="79328-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="79328-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="79328-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="79328-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="79328-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79328-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79328-126">Request headers</span></span>

| <span data-ttu-id="79328-127">Имя</span><span class="sxs-lookup"><span data-stu-id="79328-127">Name</span></span> | <span data-ttu-id="79328-128">Описание</span><span class="sxs-lookup"><span data-stu-id="79328-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="79328-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79328-129">Authorization</span></span>  | <span data-ttu-id="79328-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79328-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79328-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="79328-132">ConsistencyLevel</span></span> | <span data-ttu-id="79328-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="79328-133">eventual.</span></span> <span data-ttu-id="79328-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="79328-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="79328-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="79328-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79328-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79328-136">Request body</span></span>

<span data-ttu-id="79328-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79328-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79328-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="79328-138">Response</span></span>

<span data-ttu-id="79328-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79328-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79328-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="79328-140">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="79328-141">Пример 1. Получите транзитивное членство в группе</span><span class="sxs-lookup"><span data-stu-id="79328-141">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="79328-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="79328-142">Request</span></span>

<span data-ttu-id="79328-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79328-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79328-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="79328-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="79328-145">C#</span><span class="sxs-lookup"><span data-stu-id="79328-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79328-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79328-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79328-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79328-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79328-148">Java</span><span class="sxs-lookup"><span data-stu-id="79328-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="79328-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="79328-149">Response</span></span>

<span data-ttu-id="79328-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79328-150">The following is an example of the response.</span></span>

><span data-ttu-id="79328-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79328-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "Contoso1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="79328-153">Пример 2. Получить только число транзитивных членства</span><span class="sxs-lookup"><span data-stu-id="79328-153">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="79328-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="79328-154">Request</span></span>

<span data-ttu-id="79328-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79328-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="79328-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="79328-156">Response</span></span>

<span data-ttu-id="79328-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79328-157">The following is an example of the response.</span></span>
><span data-ttu-id="79328-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79328-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="79328-160">893</span><span class="sxs-lookup"><span data-stu-id="79328-160">893</span></span>


### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="79328-161">Пример 3. Использование cast и $search OData для получения членства в группах с отображаемой и отображаемой именами, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="79328-161">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="79328-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="79328-162">Request</span></span>

<span data-ttu-id="79328-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79328-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="79328-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="79328-164">Response</span></span>

<span data-ttu-id="79328-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79328-165">The following is an example of the response.</span></span>
><span data-ttu-id="79328-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79328-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Contoso-tier Query Notification",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="79328-168">Пример 4. Использование cast и $filter OData для получения членства пользователей в группах с отображаемой именем, которая начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="79328-168">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="79328-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="79328-169">Request</span></span>

<span data-ttu-id="79328-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79328-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="79328-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="79328-171">Response</span></span>

<span data-ttu-id="79328-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79328-172">The following is an example of the response.</span></span>
><span data-ttu-id="79328-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79328-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Users",
      "securityEnabled":true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


