---
title: Список servicePrincipal memberOf
description: Получение групп и ролей каталогов, непосредственным участником которых является данный участник службы. Эта операция не является транзитивной.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 31f40cc2abd804d29e63f7532542657a4d268d16
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291225"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="345f2-104">Список servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="345f2-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="345f2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="345f2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="345f2-106">Получение групп и ролей каталогов, непосредственным участником которых является [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="345f2-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="345f2-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="345f2-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="345f2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="345f2-108">Permissions</span></span>

<span data-ttu-id="345f2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="345f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="345f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="345f2-111">Permission type</span></span>      | <span data-ttu-id="345f2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="345f2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="345f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="345f2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="345f2-114">Application. Read. ALL, Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="345f2-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="345f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="345f2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="345f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="345f2-116">Not supported.</span></span>    |
|<span data-ttu-id="345f2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="345f2-117">Application</span></span> | <span data-ttu-id="345f2-118">Application. Read. ALL, Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="345f2-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="345f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="345f2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="345f2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="345f2-120">Optional query parameters</span></span>

<span data-ttu-id="345f2-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="345f2-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="345f2-122">Приведение OData также включено, например, можно выполнить приведение, чтобы получить только перечисление directoryrole, членом которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="345f2-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="345f2-123">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="345f2-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="345f2-124">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="345f2-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="345f2-125">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="345f2-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="345f2-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="345f2-126">Request headers</span></span>

| <span data-ttu-id="345f2-127">Имя</span><span class="sxs-lookup"><span data-stu-id="345f2-127">Name</span></span>       | <span data-ttu-id="345f2-128">Тип</span><span class="sxs-lookup"><span data-stu-id="345f2-128">Type</span></span> | <span data-ttu-id="345f2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="345f2-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="345f2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="345f2-130">Authorization</span></span>  | <span data-ttu-id="345f2-131">string</span><span class="sxs-lookup"><span data-stu-id="345f2-131">string</span></span>  | <span data-ttu-id="345f2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="345f2-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="345f2-134">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="345f2-134">ConsistencyLevel</span></span> | <span data-ttu-id="345f2-135">закончить.</span><span class="sxs-lookup"><span data-stu-id="345f2-135">eventual.</span></span> <span data-ttu-id="345f2-136">Этот заголовок и `$count` при использовании `$search` `$filter` `$orderby` параметров запроса на приведение,, или OData.</span><span class="sxs-lookup"><span data-stu-id="345f2-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="345f2-137">Он использует индекс, который может не быть актуальным с последними изменениями объекта.</span><span class="sxs-lookup"><span data-stu-id="345f2-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="345f2-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="345f2-138">Request body</span></span>
<span data-ttu-id="345f2-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="345f2-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="345f2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="345f2-140">Response</span></span>

<span data-ttu-id="345f2-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="345f2-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="345f2-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="345f2-142">Examples</span></span>

### <a name="example-1-get-groups-and-directory-roles-that-the-service-principal-is-a-direct-member-of"></a><span data-ttu-id="345f2-143">Пример 1: получение групп и ролей каталогов, непосредственным участником которых является участник службы</span><span class="sxs-lookup"><span data-stu-id="345f2-143">Example 1: Get groups and directory roles that the service principal is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="345f2-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="345f2-144">Request</span></span>

<span data-ttu-id="345f2-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="345f2-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="345f2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="345f2-146">Response</span></span>

<span data-ttu-id="345f2-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="345f2-147">The following is an example of the response.</span></span> 
> <span data-ttu-id="345f2-148">**Примечание.** Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="345f2-148">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="345f2-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="345f2-149">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="345f2-150">Пример 2: получение только количества всех членств</span><span class="sxs-lookup"><span data-stu-id="345f2-150">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="345f2-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="345f2-151">Request</span></span>

<span data-ttu-id="345f2-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="345f2-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="345f2-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="345f2-153">Response</span></span>

<span data-ttu-id="345f2-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="345f2-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="345f2-155">394</span><span class="sxs-lookup"><span data-stu-id="345f2-155">394</span></span>

### <a name="example-3-use-odata-cast-to-get-only-a-count-of-group-membership"></a><span data-ttu-id="345f2-156">Пример 3: Использование приведения OData для получения только количества участников группы</span><span class="sxs-lookup"><span data-stu-id="345f2-156">Example 3: Use OData cast to get only a count of group membership</span></span>

#### <a name="request"></a><span data-ttu-id="345f2-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="345f2-157">Request</span></span>

<span data-ttu-id="345f2-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="345f2-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_group_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="345f2-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="345f2-159">Response</span></span>

<span data-ttu-id="345f2-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="345f2-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="345f2-161">394</span><span class="sxs-lookup"><span data-stu-id="345f2-161">394</span></span>

### <a name="example-4-use-search-and-odata-cast-to-get-group-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="345f2-162">Пример 4: использование $search и функции OData для получения сведений о членстве в группах с отображаемыми именами, содержащими "видео", в том числе от числа возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="345f2-162">Example 4: Use $search and OData cast to get group membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="345f2-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="345f2-163">Request</span></span>

<span data-ttu-id="345f2-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="345f2-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET iv. https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$search=”displayName:Video" 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="345f2-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="345f2-165">Response</span></span>

<span data-ttu-id="345f2-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="345f2-166">The following is an example of the response.</span></span>
><span data-ttu-id="345f2-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="345f2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

### <a name="example-5-use-filter-and-odata-cast-to-get-group-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="345f2-169">Пример 5: используйте $filter и приведение OData для получения сведений о членстве в группах с отображаемым именем, начинающимся с буквы "A", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="345f2-169">Example 5: Use $filter and OData cast to get group membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="345f2-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="345f2-170">Request</span></span>

<span data-ttu-id="345f2-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="345f2-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="345f2-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="345f2-172">Response</span></span>

<span data-ttu-id="345f2-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="345f2-173">The following is an example of the response.</span></span>
><span data-ttu-id="345f2-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="345f2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All videos for the company",
      "displayName": "All Videos",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
