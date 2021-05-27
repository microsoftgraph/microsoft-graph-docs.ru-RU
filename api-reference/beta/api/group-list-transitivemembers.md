---
title: Перечисление транзитивных участников группы
description: Получите список участников группы.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 540f7ffd80512504291240f2c4a94db5670d73c5
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681486"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="5809a-103">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="5809a-103">List group transitive members</span></span>

<span data-ttu-id="5809a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5809a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5809a-105">Получите список участников группы.</span><span class="sxs-lookup"><span data-stu-id="5809a-105">Get a list of the group's members.</span></span> <span data-ttu-id="5809a-106">В группе могут быть пользователи, контакты, устройства, директора службы и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="5809a-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="5809a-107">Эта операция является транзитной и также возвращает плоский список всех вложенных членов.</span><span class="sxs-lookup"><span data-stu-id="5809a-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="5809a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5809a-108">Permissions</span></span>

<span data-ttu-id="5809a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5809a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5809a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5809a-111">Permission type</span></span> | <span data-ttu-id="5809a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5809a-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="5809a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5809a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5809a-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5809a-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="5809a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5809a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5809a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5809a-116">Not supported.</span></span> |
| <span data-ttu-id="5809a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5809a-117">Application</span></span> | <span data-ttu-id="5809a-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5809a-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

> <span data-ttu-id="5809a-119">**Примечание:** Чтобы перечислить членов скрытой группы членства, требуется разрешение Member.Read.Hidden.</span><span class="sxs-lookup"><span data-stu-id="5809a-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="5809a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5809a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5809a-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5809a-121">Optional query parameters</span></span>

<span data-ttu-id="5809a-122">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5809a-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="5809a-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="5809a-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="5809a-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="5809a-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="5809a-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="5809a-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5809a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5809a-126">Request headers</span></span>

| <span data-ttu-id="5809a-127">Имя</span><span class="sxs-lookup"><span data-stu-id="5809a-127">Name</span></span> | <span data-ttu-id="5809a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5809a-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="5809a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5809a-129">Authorization</span></span>  | <span data-ttu-id="5809a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5809a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5809a-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="5809a-132">ConsistencyLevel</span></span> | <span data-ttu-id="5809a-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="5809a-133">eventual.</span></span> <span data-ttu-id="5809a-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="5809a-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="5809a-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="5809a-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5809a-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5809a-136">Request body</span></span>

<span data-ttu-id="5809a-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5809a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5809a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5809a-138">Response</span></span>

<span data-ttu-id="5809a-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5809a-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5809a-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="5809a-140">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="5809a-141">Пример 1. Получить транзитное членство группы</span><span class="sxs-lookup"><span data-stu-id="5809a-141">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="5809a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5809a-142">Request</span></span>

<span data-ttu-id="5809a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5809a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5809a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="5809a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="5809a-145">C#</span><span class="sxs-lookup"><span data-stu-id="5809a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5809a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5809a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5809a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5809a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5809a-148">Java</span><span class="sxs-lookup"><span data-stu-id="5809a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5809a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="5809a-149">Response</span></span>

<span data-ttu-id="5809a-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5809a-150">The following is an example of the response.</span></span>

><span data-ttu-id="5809a-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5809a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="5809a-152">Пример 2. Получить только число транзитных членов</span><span class="sxs-lookup"><span data-stu-id="5809a-152">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="5809a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="5809a-153">Request</span></span>

<span data-ttu-id="5809a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5809a-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5809a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5809a-155">Response</span></span>

<span data-ttu-id="5809a-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5809a-156">The following is an example of the response.</span></span>
><span data-ttu-id="5809a-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5809a-157">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="5809a-158">893</span><span class="sxs-lookup"><span data-stu-id="5809a-158">893</span></span>


### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="5809a-159">Пример 3. Использование литых и $search OData для получения членства в группах с именами отображения, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="5809a-159">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5809a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="5809a-160">Request</span></span>

<span data-ttu-id="5809a-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5809a-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5809a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="5809a-162">Response</span></span>

<span data-ttu-id="5809a-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5809a-163">The following is an example of the response.</span></span>
><span data-ttu-id="5809a-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5809a-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="5809a-165">Пример 4. Использование литых и $filter OData для получения членства пользователя в группах с отображаемой именем, которая начинается с "A", включая количество возвращенных объектов.</span><span class="sxs-lookup"><span data-stu-id="5809a-165">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="5809a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="5809a-166">Request</span></span>

<span data-ttu-id="5809a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5809a-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="5809a-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="5809a-168">Response</span></span>

<span data-ttu-id="5809a-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5809a-169">The following is an example of the response.</span></span>
><span data-ttu-id="5809a-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5809a-170">**Note:** The response object shown here might be shortened for readability.</span></span>

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


