---
title: Список memberOf
description: 'Получение групп, непосредственным членом которых является данная группа. '
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ca1eb32932ba75910a462c43a29d5a6fd77a7c61
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797104"
---
# <a name="list-memberof"></a><span data-ttu-id="dfa37-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="dfa37-103">List memberOf</span></span>

<span data-ttu-id="dfa37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfa37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfa37-105">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="dfa37-105">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="dfa37-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Microsoft 365", эта операция возвращает группы всех типов, а не только группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dfa37-p101">This operation is not transitive. Unlike getting a user's Microsoft 365 groups, this returns all types of groups, not just Microsoft 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfa37-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa37-108">Permissions</span></span>
<span data-ttu-id="dfa37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa37-111">Permission type</span></span>      | <span data-ttu-id="dfa37-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfa37-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfa37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfa37-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dfa37-114">GroupMember.Read.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfa37-114">GroupMember.Read.All, Group.Read.All</span></span>    |
|<span data-ttu-id="dfa37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfa37-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa37-116">Not supported.</span></span>    |
|<span data-ttu-id="dfa37-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="dfa37-117">Application</span></span> | <span data-ttu-id="dfa37-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfa37-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="dfa37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfa37-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfa37-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfa37-120">Optional query parameters</span></span>

<span data-ttu-id="dfa37-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="dfa37-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="dfa37-122">Кроме того, включено приведение к OData, например, вы можете получить только группы, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="dfa37-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="dfa37-123">Вы можете использовать `$search` в свойствах **displayName** и **description** .</span><span class="sxs-lookup"><span data-stu-id="dfa37-123">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="dfa37-124">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="dfa37-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="dfa37-125">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="dfa37-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfa37-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfa37-126">Request headers</span></span>

| <span data-ttu-id="dfa37-127">Имя</span><span class="sxs-lookup"><span data-stu-id="dfa37-127">Name</span></span> | <span data-ttu-id="dfa37-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa37-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="dfa37-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfa37-129">Authorization</span></span>  | <span data-ttu-id="dfa37-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa37-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfa37-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="dfa37-132">ConsistencyLevel</span></span> | <span data-ttu-id="dfa37-133">необязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa37-133">eventual.</span></span> <span data-ttu-id="dfa37-134">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="dfa37-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="dfa37-135">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="dfa37-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfa37-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfa37-136">Request body</span></span>
<span data-ttu-id="dfa37-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfa37-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfa37-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa37-138">Response</span></span>
<span data-ttu-id="dfa37-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa37-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfa37-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="dfa37-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="dfa37-141">Пример 1. Получение групп и административных единиц, в которых группа является непосредственным участником</span><span class="sxs-lookup"><span data-stu-id="dfa37-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="dfa37-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa37-142">Request</span></span>

<span data-ttu-id="dfa37-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa37-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfa37-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfa37-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="dfa37-145">C#</span><span class="sxs-lookup"><span data-stu-id="dfa37-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfa37-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfa37-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfa37-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfa37-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfa37-148">Java</span><span class="sxs-lookup"><span data-stu-id="dfa37-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="dfa37-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa37-149">Response</span></span>

<span data-ttu-id="dfa37-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa37-150">The following is an example of the response.</span></span>

><span data-ttu-id="dfa37-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfa37-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="dfa37-153">Пример 2: Получение только количества участников</span><span class="sxs-lookup"><span data-stu-id="dfa37-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="dfa37-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa37-154">Request</span></span>

<span data-ttu-id="dfa37-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa37-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="dfa37-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa37-156">Response</span></span>

<span data-ttu-id="dfa37-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa37-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="dfa37-158">Пример 3. Использование OData cast для получения только количества участия в группах</span><span class="sxs-lookup"><span data-stu-id="dfa37-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="dfa37-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa37-159">Request</span></span>

<span data-ttu-id="dfa37-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa37-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="dfa37-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa37-161">Response</span></span>

<span data-ttu-id="dfa37-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa37-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`394`

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="dfa37-163">Пример 4. Использование приведения к OData и параметра $search для получения сведений об участии с отображаемыми именами, содержащими буквы "Video", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="dfa37-163">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="dfa37-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa37-164">Request</span></span>

<span data-ttu-id="dfa37-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa37-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="dfa37-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa37-166">Response</span></span>

<span data-ttu-id="dfa37-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa37-167">The following is an example of the response.</span></span>

><span data-ttu-id="dfa37-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfa37-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="dfa37-170">Пример 5: Использование приведения к OData и параметра $search для получения сведений об участии с отображаемым именем, которое начинается на "А", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="dfa37-170">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="dfa37-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa37-171">Request</span></span>

<span data-ttu-id="dfa37-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa37-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="dfa37-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa37-173">Response</span></span>

<span data-ttu-id="dfa37-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa37-174">The following is an example of the response.</span></span>

><span data-ttu-id="dfa37-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfa37-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
