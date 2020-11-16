---
title: Перечисление group transitive memberOf
description: Получение групп и административных единиц, участником которых является группа.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 87e6245f6470646a11257f5c4b1c7a7926ad693c
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082057"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="812ae-103">Перечисление group transitive memberOf</span><span class="sxs-lookup"><span data-stu-id="812ae-103">List group transitive memberOf</span></span>

<span data-ttu-id="812ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="812ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="812ae-105">Получение групп и административных единиц, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="812ae-105">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="812ae-106">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="812ae-106">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="812ae-107">В отличие от того, что получает группы Microsoft 365 пользователя, возвращаются все типы групп, а не только группы Майкрософт 365.</span><span class="sxs-lookup"><span data-stu-id="812ae-107">Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="812ae-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="812ae-108">Permissions</span></span>

<span data-ttu-id="812ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="812ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="812ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="812ae-111">Permission type</span></span> | <span data-ttu-id="812ae-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="812ae-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="812ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="812ae-113">Delegated (work or school account)</span></span> | <span data-ttu-id="812ae-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="812ae-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="812ae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="812ae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="812ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="812ae-116">Not supported.</span></span> |
| <span data-ttu-id="812ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="812ae-117">Application</span></span> | <span data-ttu-id="812ae-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="812ae-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="812ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="812ae-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="812ae-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="812ae-120">Optional query parameters</span></span>

<span data-ttu-id="812ae-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="812ae-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="812ae-122">Приведение OData также включено, например, можно выполнить приведение для получения только транзитивных участников группы.</span><span class="sxs-lookup"><span data-stu-id="812ae-122">OData cast is also enabled, for example, you can cast to get just the transitive group members of a group.</span></span> <span data-ttu-id="812ae-123">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="812ae-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="812ae-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="812ae-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="812ae-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="812ae-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="812ae-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="812ae-126">Request headers</span></span>

| <span data-ttu-id="812ae-127">Имя</span><span class="sxs-lookup"><span data-stu-id="812ae-127">Name</span></span> | <span data-ttu-id="812ae-128">Описание</span><span class="sxs-lookup"><span data-stu-id="812ae-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="812ae-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="812ae-129">Authorization</span></span>  | <span data-ttu-id="812ae-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="812ae-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="812ae-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="812ae-132">ConsistencyLevel</span></span> | <span data-ttu-id="812ae-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="812ae-133">eventual.</span></span> <span data-ttu-id="812ae-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="812ae-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="812ae-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="812ae-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="812ae-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="812ae-136">Request body</span></span>

<span data-ttu-id="812ae-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="812ae-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="812ae-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ae-138">Response</span></span>

<span data-ttu-id="812ae-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="812ae-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="812ae-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="812ae-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-transitive-member-of"></a><span data-ttu-id="812ae-141">Пример 1: получение групп и административных единиц, в которых группа является транзитивным участником</span><span class="sxs-lookup"><span data-stu-id="812ae-141">Example 1: Get groups and administrative units that the group is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="812ae-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="812ae-142">Request</span></span>

<span data-ttu-id="812ae-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="812ae-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="812ae-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="812ae-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="812ae-145">C#</span><span class="sxs-lookup"><span data-stu-id="812ae-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="812ae-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="812ae-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="812ae-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="812ae-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="812ae-148">Java</span><span class="sxs-lookup"><span data-stu-id="812ae-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="812ae-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ae-149">Response</span></span>

<span data-ttu-id="812ae-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="812ae-150">The following is an example of the response.</span></span>
><span data-ttu-id="812ae-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="812ae-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="812ae-153">Пример 2: Получение только количества транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="812ae-153">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="812ae-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="812ae-154">Request</span></span>

<span data-ttu-id="812ae-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="812ae-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="812ae-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ae-156">Response</span></span>

<span data-ttu-id="812ae-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="812ae-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="812ae-158">294</span><span class="sxs-lookup"><span data-stu-id="812ae-158">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="812ae-159">Пример 3. Использование OData cast для получения только количества транзитивных участников в группах</span><span class="sxs-lookup"><span data-stu-id="812ae-159">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="812ae-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="812ae-160">Request</span></span>

<span data-ttu-id="812ae-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="812ae-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="812ae-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ae-162">Response</span></span>

<span data-ttu-id="812ae-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="812ae-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="812ae-164">294</span><span class="sxs-lookup"><span data-stu-id="812ae-164">294</span></span>


### <a name="example-4-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="812ae-165">Пример 4: использование функции CAST и $search для получения членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="812ae-165">Example 4: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="812ae-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="812ae-166">Request</span></span>

<span data-ttu-id="812ae-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="812ae-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="812ae-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ae-168">Response</span></span>

<span data-ttu-id="812ae-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="812ae-169">The following is an example of the response.</span></span>
><span data-ttu-id="812ae-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="812ae-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="812ae-172">Пример 5: использование функции CAST и $filter для получения членства с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="812ae-172">Example 5: Use OData cast and $filter to get membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="812ae-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="812ae-173">Request</span></span>

<span data-ttu-id="812ae-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="812ae-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="812ae-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="812ae-175">Response</span></span>

<span data-ttu-id="812ae-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="812ae-176">The following is an example of the response.</span></span>
><span data-ttu-id="812ae-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="812ae-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


