---
title: Список memberOf
description: 'Получение групп, непосредственным членом которых является данная группа. '
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4d97f7fe1fc4d2b2c6e3dddf6efb90d4ecb1fb7c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680646"
---
# <a name="list-memberof"></a><span data-ttu-id="0529a-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="0529a-103">List memberOf</span></span>

<span data-ttu-id="0529a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0529a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0529a-105">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="0529a-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="0529a-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Microsoft 365", эта операция возвращает группы всех типов, а не только группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0529a-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="0529a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0529a-108">Permissions</span></span>
<span data-ttu-id="0529a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0529a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0529a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0529a-111">Permission type</span></span>      | <span data-ttu-id="0529a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0529a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0529a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0529a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0529a-114">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0529a-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="0529a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0529a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0529a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0529a-116">Not supported.</span></span>    |
|<span data-ttu-id="0529a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0529a-117">Application</span></span> | <span data-ttu-id="0529a-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0529a-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0529a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0529a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0529a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0529a-120">Optional query parameters</span></span>

<span data-ttu-id="0529a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="0529a-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="0529a-122">Кроме того, включено приведение к OData, например, вы можете получить только группы, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="0529a-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="0529a-123">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="0529a-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="0529a-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="0529a-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="0529a-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="0529a-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0529a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0529a-126">Request headers</span></span>

| <span data-ttu-id="0529a-127">Имя</span><span class="sxs-lookup"><span data-stu-id="0529a-127">Name</span></span> | <span data-ttu-id="0529a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0529a-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0529a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0529a-129">Authorization</span></span>  | <span data-ttu-id="0529a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0529a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0529a-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="0529a-132">ConsistencyLevel</span></span> | <span data-ttu-id="0529a-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="0529a-133">eventual.</span></span> <span data-ttu-id="0529a-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="0529a-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="0529a-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="0529a-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0529a-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0529a-136">Request body</span></span>
<span data-ttu-id="0529a-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0529a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0529a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0529a-138">Response</span></span>
<span data-ttu-id="0529a-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0529a-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0529a-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="0529a-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="0529a-141">Пример 1. Получение групп и административных единиц, в которых группа является непосредственным участником</span><span class="sxs-lookup"><span data-stu-id="0529a-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="0529a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0529a-142">Request</span></span>

<span data-ttu-id="0529a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0529a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0529a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0529a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="0529a-145">C#</span><span class="sxs-lookup"><span data-stu-id="0529a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0529a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0529a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0529a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0529a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0529a-148">Java</span><span class="sxs-lookup"><span data-stu-id="0529a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0529a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0529a-149">Response</span></span>

<span data-ttu-id="0529a-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0529a-150">The following is an example of the response.</span></span>

><span data-ttu-id="0529a-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0529a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="0529a-152">Пример 2: Получение только количества участников</span><span class="sxs-lookup"><span data-stu-id="0529a-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="0529a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="0529a-153">Request</span></span>

<span data-ttu-id="0529a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0529a-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0529a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0529a-155">Response</span></span>

<span data-ttu-id="0529a-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0529a-156">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="0529a-157">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="0529a-157">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="0529a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0529a-158">Request</span></span>

<span data-ttu-id="0529a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0529a-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0529a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0529a-160">Response</span></span>

<span data-ttu-id="0529a-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0529a-161">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="0529a-162">Пример 4. Использование приведения к OData и параметра $search для получения сведений об участии с отображаемыми именами, содержащими буквы "Video", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="0529a-162">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0529a-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="0529a-163">Request</span></span>

<span data-ttu-id="0529a-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0529a-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0529a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="0529a-165">Response</span></span>

<span data-ttu-id="0529a-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0529a-166">The following is an example of the response.</span></span>

><span data-ttu-id="0529a-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0529a-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="0529a-168">Пример 5: Использование приведения к OData и параметра $search для получения сведений об участии с отображаемым именем, которое начинается на "А", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="0529a-168">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0529a-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="0529a-169">Request</span></span>

<span data-ttu-id="0529a-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0529a-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="0529a-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="0529a-171">Response</span></span>

<span data-ttu-id="0529a-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0529a-172">The following is an example of the response.</span></span>

><span data-ttu-id="0529a-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0529a-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
