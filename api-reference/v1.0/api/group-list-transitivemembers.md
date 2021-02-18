---
title: Перечисление транзитивных участников группы
description: Получите список членов группы. В качестве членов группы могут быть пользователи, устройства, контакты организации и другие группы. Эта операция является транзитивной и возвращает плоский список всех вложенных членов.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0b428dd011937473d1c860e15b95d11e7171eb92
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272179"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="39cae-105">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="39cae-105">List group transitive members</span></span>

<span data-ttu-id="39cae-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39cae-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39cae-107">Получите список членов группы.</span><span class="sxs-lookup"><span data-stu-id="39cae-107">Get a list of the group's members.</span></span> <span data-ttu-id="39cae-108">В качестве членов группы могут быть пользователи, устройства, контакты организации и другие группы.</span><span class="sxs-lookup"><span data-stu-id="39cae-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="39cae-109">Эта операция является транзитивной и возвращает плоский список всех вложенных членов.</span><span class="sxs-lookup"><span data-stu-id="39cae-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="39cae-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39cae-110">Permissions</span></span>

<span data-ttu-id="39cae-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39cae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39cae-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39cae-113">Permission type</span></span>      | <span data-ttu-id="39cae-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39cae-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39cae-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39cae-115">Delegated (work or school account)</span></span> | <span data-ttu-id="39cae-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39cae-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="39cae-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39cae-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39cae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39cae-118">Not supported.</span></span>    |
|<span data-ttu-id="39cae-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39cae-119">Application</span></span> | <span data-ttu-id="39cae-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="39cae-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

><span data-ttu-id="39cae-121">**Примечание.** Для получения списка участников скрытой группы членства требуется разрешение Member.Read.Hidden.</span><span class="sxs-lookup"><span data-stu-id="39cae-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="39cae-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39cae-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39cae-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39cae-123">Optional query parameters</span></span>

<span data-ttu-id="39cae-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="39cae-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="39cae-125">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="39cae-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="39cae-126">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="39cae-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="39cae-127">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="39cae-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39cae-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39cae-128">Request headers</span></span>

| <span data-ttu-id="39cae-129">Имя</span><span class="sxs-lookup"><span data-stu-id="39cae-129">Name</span></span> | <span data-ttu-id="39cae-130">Описание</span><span class="sxs-lookup"><span data-stu-id="39cae-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="39cae-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39cae-131">Authorization</span></span>  | <span data-ttu-id="39cae-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39cae-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39cae-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="39cae-134">ConsistencyLevel</span></span> | <span data-ttu-id="39cae-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="39cae-135">eventual.</span></span> <span data-ttu-id="39cae-136">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="39cae-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="39cae-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="39cae-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39cae-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39cae-138">Request body</span></span>

<span data-ttu-id="39cae-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39cae-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39cae-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="39cae-140">Response</span></span>

<span data-ttu-id="39cae-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39cae-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39cae-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="39cae-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="39cae-143">Пример 1. Просмотр транзитивного членства в группе</span><span class="sxs-lookup"><span data-stu-id="39cae-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="39cae-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="39cae-144">Request</span></span>

<span data-ttu-id="39cae-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39cae-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39cae-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="39cae-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="39cae-147">C#</span><span class="sxs-lookup"><span data-stu-id="39cae-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39cae-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39cae-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39cae-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39cae-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39cae-150">Java</span><span class="sxs-lookup"><span data-stu-id="39cae-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="39cae-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="39cae-151">Response</span></span>

<span data-ttu-id="39cae-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39cae-152">The following is an example of the response.</span></span>

><span data-ttu-id="39cae-153">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="39cae-153">**Note**: The response object shown here might be shortened for readability.</span></span>

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
      "@odata.type": "#microsoft.graph.user",
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="39cae-154">Пример 2. Получить только число транзитивных членства</span><span class="sxs-lookup"><span data-stu-id="39cae-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="39cae-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="39cae-155">Request</span></span>

<span data-ttu-id="39cae-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39cae-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="39cae-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="39cae-157">Response</span></span>

<span data-ttu-id="39cae-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39cae-158">The following is an example of the response.</span></span>

><span data-ttu-id="39cae-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39cae-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="39cae-161">Пример 3. Использование cast и $search OData для получения членства в группах с отображаемой и отображаемой именами, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="39cae-161">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="39cae-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="39cae-162">Request</span></span>

<span data-ttu-id="39cae-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39cae-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="39cae-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="39cae-164">Response</span></span>

<span data-ttu-id="39cae-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39cae-165">The following is an example of the response.</span></span>

><span data-ttu-id="39cae-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39cae-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,id)",
  "@odata.count":7,
  "value":[
    {
      "displayName":"Joseph Price",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="39cae-168">Пример 4. Использование cast и $filter OData для получения членства пользователей в группах с отображаемой именем, которая начинается с "A", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="39cae-168">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="39cae-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="39cae-169">Request</span></span>

<span data-ttu-id="39cae-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39cae-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="39cae-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="39cae-171">Response</span></span>

<span data-ttu-id="39cae-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39cae-172">The following is an example of the response.</span></span>

><span data-ttu-id="39cae-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39cae-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Users",
      "mail":"AADContoso_Users@contoso.com"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
