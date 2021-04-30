---
title: Перечисление транзитивных участников группы
description: Получите список участников группы. В составе группы могут быть пользователи, устройства, организационные контакты и другие группы. Эта операция является транзитной и возвращает плоский список всех вложенных членов.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 35154e6fe6ef26588b8025febe1a57982d020b9a
ms.sourcegitcommit: 9bc1652890fe49d7ad5e5b7177c8a682b1759b75
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2021
ms.locfileid: "52100053"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="54baf-105">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="54baf-105">List group transitive members</span></span>

<span data-ttu-id="54baf-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54baf-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54baf-107">Получите список участников группы.</span><span class="sxs-lookup"><span data-stu-id="54baf-107">Get a list of the group's members.</span></span> <span data-ttu-id="54baf-108">В составе группы могут быть пользователи, устройства, организационные контакты и другие группы.</span><span class="sxs-lookup"><span data-stu-id="54baf-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="54baf-109">Эта операция является транзитной и возвращает плоский список всех вложенных членов.</span><span class="sxs-lookup"><span data-stu-id="54baf-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="54baf-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54baf-110">Permissions</span></span>

<span data-ttu-id="54baf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54baf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54baf-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54baf-113">Permission type</span></span>      | <span data-ttu-id="54baf-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54baf-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54baf-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54baf-115">Delegated (work or school account)</span></span> | <span data-ttu-id="54baf-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54baf-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="54baf-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54baf-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54baf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54baf-118">Not supported.</span></span>    |
|<span data-ttu-id="54baf-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54baf-119">Application</span></span> | <span data-ttu-id="54baf-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="54baf-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

><span data-ttu-id="54baf-121">**Примечание:** Чтобы перечислить членов скрытой группы членства, требуется разрешение Member.Read.Hidden.</span><span class="sxs-lookup"><span data-stu-id="54baf-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="54baf-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54baf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54baf-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54baf-123">Optional query parameters</span></span>

<span data-ttu-id="54baf-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="54baf-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="54baf-125">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="54baf-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="54baf-126">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="54baf-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="54baf-127">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="54baf-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54baf-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54baf-128">Request headers</span></span>

| <span data-ttu-id="54baf-129">Имя</span><span class="sxs-lookup"><span data-stu-id="54baf-129">Name</span></span> | <span data-ttu-id="54baf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="54baf-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="54baf-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54baf-131">Authorization</span></span>  | <span data-ttu-id="54baf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54baf-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54baf-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="54baf-134">ConsistencyLevel</span></span> | <span data-ttu-id="54baf-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="54baf-135">eventual.</span></span> <span data-ttu-id="54baf-136">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="54baf-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="54baf-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="54baf-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54baf-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54baf-138">Request body</span></span>

<span data-ttu-id="54baf-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54baf-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54baf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="54baf-140">Response</span></span>

<span data-ttu-id="54baf-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54baf-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54baf-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="54baf-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="54baf-143">Пример 1. Получить транзитное членство группы</span><span class="sxs-lookup"><span data-stu-id="54baf-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="54baf-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="54baf-144">Request</span></span>

<span data-ttu-id="54baf-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54baf-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54baf-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="54baf-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="54baf-147">C#</span><span class="sxs-lookup"><span data-stu-id="54baf-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54baf-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54baf-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54baf-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54baf-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54baf-150">Java</span><span class="sxs-lookup"><span data-stu-id="54baf-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="54baf-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="54baf-151">Response</span></span>

<span data-ttu-id="54baf-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54baf-152">The following is an example of the response.</span></span>

><span data-ttu-id="54baf-153">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54baf-153">**Note**: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="54baf-154">Пример 2. Получить только число транзитных членов</span><span class="sxs-lookup"><span data-stu-id="54baf-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="54baf-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="54baf-155">Request</span></span>

<span data-ttu-id="54baf-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54baf-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="54baf-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="54baf-157">Response</span></span>

<span data-ttu-id="54baf-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54baf-158">The following is an example of the response.</span></span>

><span data-ttu-id="54baf-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54baf-159">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="54baf-160">Пример 3. Использование литых и $search OData для получения членства в группах с именами отображения, которые содержат буквы "tier", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="54baf-160">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="54baf-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="54baf-161">Request</span></span>

<span data-ttu-id="54baf-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54baf-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="54baf-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="54baf-163">Response</span></span>

<span data-ttu-id="54baf-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54baf-164">The following is an example of the response.</span></span>

><span data-ttu-id="54baf-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54baf-165">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="54baf-166">Пример 4. Использование литых и $filter OData для получения членства пользователя в группах с отображаемой именем, которая начинается с "A", включая количество возвращенных объектов.</span><span class="sxs-lookup"><span data-stu-id="54baf-166">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="54baf-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="54baf-167">Request</span></span>

<span data-ttu-id="54baf-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54baf-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="54baf-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="54baf-169">Response</span></span>

<span data-ttu-id="54baf-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54baf-170">The following is an example of the response.</span></span>

><span data-ttu-id="54baf-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54baf-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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
