---
title: Список транзитивных членов группы
description: Получение списка членов группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a6d92f50380706f912bdb86102d3236ae812997c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333292"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="54b15-103">Список транзитивных членов группы</span><span class="sxs-lookup"><span data-stu-id="54b15-103">List group transitive members</span></span>

<span data-ttu-id="54b15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54b15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54b15-105">Получение списка членов группы.</span><span class="sxs-lookup"><span data-stu-id="54b15-105">Get a list of the group's members.</span></span> <span data-ttu-id="54b15-106">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="54b15-106">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="54b15-107">Эта операция является транзитивным и также возвращает плоский список всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="54b15-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="54b15-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54b15-108">Permissions</span></span>

<span data-ttu-id="54b15-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54b15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54b15-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54b15-111">Permission type</span></span> | <span data-ttu-id="54b15-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54b15-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="54b15-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54b15-113">Delegated (work or school account)</span></span> | <span data-ttu-id="54b15-114">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="54b15-114">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
| <span data-ttu-id="54b15-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54b15-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54b15-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54b15-116">Not supported.</span></span> |
| <span data-ttu-id="54b15-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54b15-117">Application</span></span> | <span data-ttu-id="54b15-118">Directory. Read. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="54b15-118">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="54b15-119">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="54b15-119">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="54b15-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54b15-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54b15-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54b15-121">Optional query parameters</span></span>

<span data-ttu-id="54b15-122">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="54b15-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="54b15-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="54b15-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="54b15-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="54b15-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="54b15-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="54b15-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54b15-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54b15-126">Request headers</span></span>

| <span data-ttu-id="54b15-127">Имя</span><span class="sxs-lookup"><span data-stu-id="54b15-127">Name</span></span> | <span data-ttu-id="54b15-128">Описание</span><span class="sxs-lookup"><span data-stu-id="54b15-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="54b15-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54b15-129">Authorization</span></span>  | <span data-ttu-id="54b15-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54b15-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54b15-132">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="54b15-132">ConsistencyLevel</span></span> | <span data-ttu-id="54b15-133">закончить.</span><span class="sxs-lookup"><span data-stu-id="54b15-133">eventual.</span></span> <span data-ttu-id="54b15-134">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="54b15-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="54b15-135">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="54b15-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54b15-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54b15-136">Request body</span></span>

<span data-ttu-id="54b15-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54b15-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54b15-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b15-138">Response</span></span>

<span data-ttu-id="54b15-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54b15-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54b15-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="54b15-140">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="54b15-141">Пример 1: получение транзитивного членства в группе</span><span class="sxs-lookup"><span data-stu-id="54b15-141">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="54b15-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="54b15-142">Request</span></span>

<span data-ttu-id="54b15-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54b15-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54b15-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="54b15-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="54b15-145">C#</span><span class="sxs-lookup"><span data-stu-id="54b15-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54b15-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54b15-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54b15-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54b15-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="54b15-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b15-148">Response</span></span>

<span data-ttu-id="54b15-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54b15-149">The following is an example of the response.</span></span>

><span data-ttu-id="54b15-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54b15-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="54b15-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54b15-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="54b15-152">Пример 2: получение только числа транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="54b15-152">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="54b15-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="54b15-153">Request</span></span>

<span data-ttu-id="54b15-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54b15-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54b15-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="54b15-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="54b15-156">C#</span><span class="sxs-lookup"><span data-stu-id="54b15-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54b15-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54b15-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54b15-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54b15-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54b15-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b15-159">Response</span></span>

<span data-ttu-id="54b15-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54b15-160">The following is an example of the response.</span></span>
><span data-ttu-id="54b15-161">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54b15-161">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="54b15-162">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54b15-162">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="54b15-163">893</span><span class="sxs-lookup"><span data-stu-id="54b15-163">893</span></span>


### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="54b15-164">Пример 3: использование функции CAST и $search для получения членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="54b15-164">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="54b15-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="54b15-165">Request</span></span>

<span data-ttu-id="54b15-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54b15-166">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54b15-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="54b15-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="54b15-168">C#</span><span class="sxs-lookup"><span data-stu-id="54b15-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tier-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54b15-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54b15-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tier-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54b15-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54b15-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tier-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54b15-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b15-171">Response</span></span>

<span data-ttu-id="54b15-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54b15-172">The following is an example of the response.</span></span>
><span data-ttu-id="54b15-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54b15-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="54b15-175">Пример 4: использование функции CAST и $filter для получения членства пользователя в группах с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="54b15-175">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="54b15-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="54b15-176">Request</span></span>

<span data-ttu-id="54b15-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54b15-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="54b15-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="54b15-178">Response</span></span>

<span data-ttu-id="54b15-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54b15-179">The following is an example of the response.</span></span>
><span data-ttu-id="54b15-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54b15-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
