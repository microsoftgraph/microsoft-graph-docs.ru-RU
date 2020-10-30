---
title: Перечисление транзитивных участников группы
description: Получение списка членов группы. У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников. Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bcd666c743d50b0e8d263510fe7b33297fc16940
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796656"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="3b576-105">Перечисление транзитивных участников группы</span><span class="sxs-lookup"><span data-stu-id="3b576-105">List group transitive members</span></span>

<span data-ttu-id="3b576-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b576-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b576-107">Получение списка членов группы.</span><span class="sxs-lookup"><span data-stu-id="3b576-107">Get a list of the group's members.</span></span> <span data-ttu-id="3b576-108">У группы могут быть пользователи, устройства, организационные контакты и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="3b576-108">A group can have users, devices, organizational contacts, and other groups as members.</span></span> <span data-ttu-id="3b576-109">Эта операция является транзитивным и возвращает плоский список всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="3b576-109">This operation is transitive and returns a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b576-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b576-110">Permissions</span></span>

<span data-ttu-id="3b576-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b576-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b576-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b576-113">Permission type</span></span>      | <span data-ttu-id="3b576-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b576-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b576-115">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b576-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3b576-116">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3b576-116">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All, Application.Read.All</span></span>  |
|<span data-ttu-id="3b576-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b576-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b576-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b576-118">Not supported.</span></span>    |
|<span data-ttu-id="3b576-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="3b576-119">Application</span></span> | <span data-ttu-id="3b576-120">Directory. Read. ALL, User. Read. ALL, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3b576-120">Directory.Read.All, User.Read.All, Application.Read.All</span></span> |

><span data-ttu-id="3b576-121">**Примечание:** Чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="3b576-121">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3b576-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b576-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b576-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b576-123">Optional query parameters</span></span>

<span data-ttu-id="3b576-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="3b576-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="3b576-125">Можно использовать `$search` в свойствах **DisplayName** и **Description** .</span><span class="sxs-lookup"><span data-stu-id="3b576-125">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="3b576-126">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="3b576-126">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="3b576-127">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="3b576-127">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b576-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b576-128">Request headers</span></span>

| <span data-ttu-id="3b576-129">Имя</span><span class="sxs-lookup"><span data-stu-id="3b576-129">Name</span></span> | <span data-ttu-id="3b576-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3b576-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="3b576-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b576-131">Authorization</span></span>  | <span data-ttu-id="3b576-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b576-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b576-134">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="3b576-134">ConsistencyLevel</span></span> | <span data-ttu-id="3b576-135">необязательный.</span><span class="sxs-lookup"><span data-stu-id="3b576-135">eventual.</span></span> <span data-ttu-id="3b576-136">Этот заголовок и `$count` требуются при использовании `$search`, `$filter`, `$orderby` или с параметрами запросов OData cast.</span><span class="sxs-lookup"><span data-stu-id="3b576-136">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="3b576-137">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="3b576-137">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b576-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b576-138">Request body</span></span>

<span data-ttu-id="3b576-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b576-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b576-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b576-140">Response</span></span>

<span data-ttu-id="3b576-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b576-141">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b576-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="3b576-142">Examples</span></span>

### <a name="example-1-get-the-transitive-membership-of-a-group"></a><span data-ttu-id="3b576-143">Пример 1: получение транзитивного членства в группе</span><span class="sxs-lookup"><span data-stu-id="3b576-143">Example 1: Get the transitive membership of a group</span></span>

#### <a name="request"></a><span data-ttu-id="3b576-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b576-144">Request</span></span>

<span data-ttu-id="3b576-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b576-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b576-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b576-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="3b576-147">C#</span><span class="sxs-lookup"><span data-stu-id="3b576-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b576-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b576-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b576-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b576-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b576-150">Java</span><span class="sxs-lookup"><span data-stu-id="3b576-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3b576-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b576-151">Response</span></span>

<span data-ttu-id="3b576-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b576-152">The following is an example of the response.</span></span>

><span data-ttu-id="3b576-153">**Примечание** . Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3b576-153">**Note** : The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-transitive-membership"></a><span data-ttu-id="3b576-154">Пример 2: получение только числа транзитивных участников</span><span class="sxs-lookup"><span data-stu-id="3b576-154">Example 2: Get only a count of transitive membership</span></span>

#### <a name="request"></a><span data-ttu-id="3b576-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b576-155">Request</span></span>

<span data-ttu-id="3b576-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b576-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b576-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b576-157">Response</span></span>

<span data-ttu-id="3b576-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b576-158">The following is an example of the response.</span></span>

><span data-ttu-id="3b576-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b576-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-3-use-odata-cast-and-search-to-get-membership-in-groups-with-display-names-that-contain-the-letters-tier-including-a-count-of-returned-objects"></a><span data-ttu-id="3b576-161">Пример 3: использование функции CAST и $search для получения членства в группах с отображаемыми именами, содержащими уровень, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="3b576-161">Example 3: Use OData cast and $search to get membership in groups with display names that contain the letters 'tier' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3b576-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b576-162">Request</span></span>

<span data-ttu-id="3b576-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b576-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tier_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.user?$count=true&$orderBy=displayName&$search="displayName:tier"&$select=displayName,id
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b576-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b576-164">Response</span></span>

<span data-ttu-id="3b576-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b576-165">The following is an example of the response.</span></span>

><span data-ttu-id="3b576-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b576-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-user-membership-in-groups-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="3b576-168">Пример 4: использование функции CAST и $filter для получения членства пользователя в группах с отображаемым именем, начинающимся с "A", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="3b576-168">Example 4: Use OData cast and $filter to get user membership in groups with a display name that starts with 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="3b576-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b576-169">Request</span></span>

<span data-ttu-id="3b576-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b576-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers/microsoft.graph.users?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'a')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="3b576-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b576-171">Response</span></span>

<span data-ttu-id="3b576-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b576-172">The following is an example of the response.</span></span>

><span data-ttu-id="3b576-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b576-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
