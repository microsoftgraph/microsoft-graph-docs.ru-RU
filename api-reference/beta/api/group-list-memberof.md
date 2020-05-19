---
title: Группа списка memberOf
description: Получение групп и административных единиц, непосредственным участником которых является группа.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d5371bd0dffe343a844c6ea8a7ac5fec2a6fef1a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289632"
---
# <a name="list-group-memberof"></a><span data-ttu-id="d47f5-103">Группа списка memberOf</span><span class="sxs-lookup"><span data-stu-id="d47f5-103">List group memberOf</span></span>

<span data-ttu-id="d47f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d47f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d47f5-105">Получение групп и административных единиц, непосредственным участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="d47f5-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="d47f5-p101">Эта операция не является транзитивным. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="d47f5-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d47f5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d47f5-108">Permissions</span></span>

<span data-ttu-id="d47f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d47f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d47f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d47f5-111">Permission type</span></span> | <span data-ttu-id="d47f5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d47f5-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="d47f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d47f5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d47f5-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d47f5-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
| <span data-ttu-id="d47f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d47f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d47f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d47f5-116">Not supported.</span></span> |
| <span data-ttu-id="d47f5-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d47f5-117">Application</span></span> | <span data-ttu-id="d47f5-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47f5-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d47f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d47f5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d47f5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d47f5-120">Optional query parameters</span></span>

<span data-ttu-id="d47f5-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="d47f5-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="d47f5-122">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только те группы, участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="d47f5-122">OData cast is also enabled, for example, you can cast to get just the groups the group is a member of.</span></span> <span data-ttu-id="d47f5-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="d47f5-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="d47f5-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="d47f5-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="d47f5-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="d47f5-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d47f5-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d47f5-126">Request headers</span></span>

| <span data-ttu-id="d47f5-127">Имя</span><span class="sxs-lookup"><span data-stu-id="d47f5-127">Name</span></span> | <span data-ttu-id="d47f5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d47f5-128">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="d47f5-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d47f5-129">Authorization</span></span>  | <span data-ttu-id="d47f5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d47f5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d47f5-132">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="d47f5-132">ConsistencyLevel</span></span> | <span data-ttu-id="d47f5-133">закончить.</span><span class="sxs-lookup"><span data-stu-id="d47f5-133">eventual.</span></span> <span data-ttu-id="d47f5-134">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="d47f5-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="d47f5-135">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="d47f5-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d47f5-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d47f5-136">Request body</span></span>

<span data-ttu-id="d47f5-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d47f5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d47f5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d47f5-138">Response</span></span>

<span data-ttu-id="d47f5-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d47f5-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d47f5-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="d47f5-140">Examples</span></span>

### <a name="example-1-get-groups-and-administrative-units-that-the-group-is-a-direct-member-of"></a><span data-ttu-id="d47f5-141">Пример 1: получение групп и административных единиц, непосредственным участником которых является группа</span><span class="sxs-lookup"><span data-stu-id="d47f5-141">Example 1: Get groups and administrative units that the group is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="d47f5-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d47f5-142">Request</span></span>

<span data-ttu-id="d47f5-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d47f5-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d47f5-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d47f5-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="d47f5-145">C#</span><span class="sxs-lookup"><span data-stu-id="d47f5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d47f5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d47f5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d47f5-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d47f5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d47f5-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d47f5-148">Response</span></span>

<span data-ttu-id="d47f5-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d47f5-149">The following is an example of the response.</span></span>
><span data-ttu-id="d47f5-150">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d47f5-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d47f5-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d47f5-151">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="d47f5-152">Пример 2: получение только количества всех членств</span><span class="sxs-lookup"><span data-stu-id="d47f5-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="d47f5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="d47f5-153">Request</span></span>

<span data-ttu-id="d47f5-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d47f5-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d47f5-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="d47f5-155">Response</span></span>

<span data-ttu-id="d47f5-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d47f5-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="d47f5-157">394</span><span class="sxs-lookup"><span data-stu-id="d47f5-157">394</span></span>


### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="d47f5-158">Пример 3: Использование приведения OData для получения только количества участников группы</span><span class="sxs-lookup"><span data-stu-id="d47f5-158">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="d47f5-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="d47f5-159">Request</span></span>

<span data-ttu-id="d47f5-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d47f5-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d47f5-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="d47f5-161">Response</span></span>

<span data-ttu-id="d47f5-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d47f5-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="d47f5-163">394</span><span class="sxs-lookup"><span data-stu-id="d47f5-163">394</span></span>

### <a name="example-4-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="d47f5-164">Пример 4: использование функции CAST и $search для получения членства с отображаемыми именами, содержащими "видео", в том числе от числа возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="d47f5-164">Example 4: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d47f5-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="d47f5-165">Request</span></span>

<span data-ttu-id="d47f5-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d47f5-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d47f5-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="d47f5-167">Response</span></span>

<span data-ttu-id="d47f5-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d47f5-168">The following is an example of the response.</span></span>
><span data-ttu-id="d47f5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d47f5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
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

### <a name="example-5-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="d47f5-171">Пример 5: использование функции CAST и $filter для получения членства с отображаемым именем, начинающимся с буквы "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="d47f5-171">Example 5: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="d47f5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="d47f5-172">Request</span></span>

<span data-ttu-id="d47f5-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d47f5-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="d47f5-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="d47f5-174">Response</span></span>

<span data-ttu-id="d47f5-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d47f5-175">The following is an example of the response.</span></span>
><span data-ttu-id="d47f5-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d47f5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
