---
title: Перечисление транзитивных servicePrincipal memberOf
description: Получение групп и ролей каталогов, членом которых является данный участник службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: f9807af8d7eda17eceec6a69113bafbcafbe1a7b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290049"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="b1e49-103">Перечисление транзитивных servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="b1e49-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="b1e49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1e49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1e49-105">Получение групп и ролей каталогов, участником которых является данный [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="b1e49-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="b1e49-106">Эта операция является транзитивным и включает все группы, вложенные в состав участника службы.</span><span class="sxs-lookup"><span data-stu-id="b1e49-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1e49-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1e49-107">Permissions</span></span>
<span data-ttu-id="b1e49-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1e49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1e49-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1e49-110">Permission type</span></span>      | <span data-ttu-id="b1e49-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1e49-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1e49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1e49-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1e49-113">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="b1e49-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b1e49-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1e49-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1e49-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1e49-115">Not supported.</span></span>    |
|<span data-ttu-id="b1e49-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1e49-116">Application</span></span> | <span data-ttu-id="b1e49-117">Application. Read. ALL, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b1e49-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b1e49-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1e49-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1e49-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1e49-119">Optional query parameters</span></span>
<span data-ttu-id="b1e49-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="b1e49-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="b1e49-121">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только перечисление directoryrole, членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="b1e49-121">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="b1e49-122">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="b1e49-122">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="b1e49-123">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e49-123">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b1e49-124">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="b1e49-124">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1e49-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1e49-125">Request headers</span></span>

| <span data-ttu-id="b1e49-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b1e49-126">Name</span></span>       | <span data-ttu-id="b1e49-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b1e49-127">Type</span></span> | <span data-ttu-id="b1e49-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b1e49-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1e49-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1e49-129">Authorization</span></span>  | <span data-ttu-id="b1e49-130">string</span><span class="sxs-lookup"><span data-stu-id="b1e49-130">string</span></span>  | <span data-ttu-id="b1e49-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1e49-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1e49-133">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="b1e49-133">ConsistencyLevel</span></span> | <span data-ttu-id="b1e49-134">закончить.</span><span class="sxs-lookup"><span data-stu-id="b1e49-134">eventual.</span></span> <span data-ttu-id="b1e49-135">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="b1e49-135">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="b1e49-136">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="b1e49-136">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1e49-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1e49-137">Request body</span></span>
<span data-ttu-id="b1e49-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1e49-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1e49-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e49-139">Response</span></span>

<span data-ttu-id="b1e49-140">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e49-140">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1e49-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="b1e49-141">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-transitive-member-of"></a><span data-ttu-id="b1e49-142">Пример 1: получение групп и ролей каталогов, членом которых является транзитивное участник службы</span><span class="sxs-lookup"><span data-stu-id="b1e49-142">Example 1: Get groups and directory roles that the service principal is a transitive member of</span></span>

#### <a name="request"></a><span data-ttu-id="b1e49-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1e49-143">Request</span></span>

<span data-ttu-id="b1e49-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e49-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```

#### <a name="response"></a><span data-ttu-id="b1e49-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e49-145">Response</span></span>

<span data-ttu-id="b1e49-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e49-146">The following is an example of the response.</span></span> 
> <span data-ttu-id="b1e49-147">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b1e49-147">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b1e49-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1e49-148">All of the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-transitive-membership"></a><span data-ttu-id="b1e49-149">Пример 2: получение только количества всех транзитивных членств</span><span class="sxs-lookup"><span data-stu-id="b1e49-149">Example 2: Get only a count of all transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="b1e49-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1e49-150">Request</span></span>

<span data-ttu-id="b1e49-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e49-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b1e49-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e49-152">Response</span></span>

<span data-ttu-id="b1e49-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e49-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="b1e49-154">294</span><span class="sxs-lookup"><span data-stu-id="b1e49-154">294</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-transitive-membership-in-groups"></a><span data-ttu-id="b1e49-155">Пример 3: Использование приведения OData для получения только счетчика транзитивного членства в группах</span><span class="sxs-lookup"><span data-stu-id="b1e49-155">Example 3: Use OData cast to get only a count of transitive membership in groups</span></span>

#### <a name="request"></a><span data-ttu-id="b1e49-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1e49-156">Request</span></span>

<span data-ttu-id="b1e49-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e49-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b1e49-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e49-158">Response</span></span>

<span data-ttu-id="b1e49-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e49-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="b1e49-160">294</span><span class="sxs-lookup"><span data-stu-id="b1e49-160">294</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="b1e49-161">Пример 4: использование $search и функции OData для получения сведений о членстве в группах с отображаемыми именами, содержащими "видео", в том числе от числа возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="b1e49-161">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b1e49-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1e49-162">Request</span></span>

<span data-ttu-id="b1e49-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e49-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search="displayName:Video"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b1e49-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e49-164">Response</span></span>

<span data-ttu-id="b1e49-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e49-165">The following is an example of the response.</span></span>
><span data-ttu-id="b1e49-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1e49-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "displayName":"Contoso Videos",
      "id":"11111111-2222-3333-4444-555555555555"
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b1e49-168">Пример 5: используйте $filter и приведение OData для получения сведений о членстве в группах с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="b1e49-168">Example 5: Use $filter and OData cast to get group membership with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b1e49-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1e49-169">Request</span></span>

<span data-ttu-id="b1e49-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e49-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b1e49-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e49-171">Response</span></span>

<span data-ttu-id="b1e49-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e49-172">The following is an example of the response.</span></span>
><span data-ttu-id="b1e49-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1e49-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List servicePrincipal transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
