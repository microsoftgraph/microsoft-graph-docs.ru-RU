---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7b0fb758e0d852e4cf72dfb0c271dc0aae686e42
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332805"
---
# <a name="list-groups"></a><span data-ttu-id="44d13-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="44d13-103">List groups</span></span>

<span data-ttu-id="44d13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44d13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44d13-105">Список всех групп в организации, в том числе групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="44d13-105">List all the groups in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="44d13-106">Эта операция по умолчанию возвращает для каждой группы только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="44d13-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="44d13-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="44d13-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="44d13-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="44d13-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="44d13-109">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="44d13-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="44d13-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44d13-110">Permissions</span></span>

<span data-ttu-id="44d13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44d13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44d13-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44d13-113">Permission type</span></span> | <span data-ttu-id="44d13-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44d13-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="44d13-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44d13-115">Delegated (work or school account)</span></span> | <span data-ttu-id="44d13-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44d13-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="44d13-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44d13-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44d13-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d13-118">Not supported.</span></span> |
| <span data-ttu-id="44d13-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44d13-119">Application</span></span> | <span data-ttu-id="44d13-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d13-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44d13-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44d13-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44d13-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="44d13-122">Optional query parameters</span></span>

<span data-ttu-id="44d13-123">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="44d13-123">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="44d13-124">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="44d13-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```
<span data-ttu-id="44d13-125">Вы также можете использовать `$count` `$search` Параметры запроса и для ограничения отклика.</span><span class="sxs-lookup"><span data-stu-id="44d13-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="44d13-126">`$search`Параметр запроса поддерживает разметку только для полей **DisplayName** и **Description** .</span><span class="sxs-lookup"><span data-stu-id="44d13-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="44d13-127">Другие поля по умолчанию заменяют `$filter` поведение.</span><span class="sxs-lookup"><span data-stu-id="44d13-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="44d13-128">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="44d13-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="44d13-129">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="44d13-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="44d13-130">Для получения дополнительных сведений обратитесь к разделу [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="44d13-130">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="44d13-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44d13-131">Request headers</span></span>

| <span data-ttu-id="44d13-132">Имя</span><span class="sxs-lookup"><span data-stu-id="44d13-132">Name</span></span> | <span data-ttu-id="44d13-133">Описание</span><span class="sxs-lookup"><span data-stu-id="44d13-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="44d13-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44d13-134">Authorization</span></span>  | <span data-ttu-id="44d13-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44d13-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44d13-137">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="44d13-137">ConsistencyLevel</span></span> | <span data-ttu-id="44d13-138">закончить.</span><span class="sxs-lookup"><span data-stu-id="44d13-138">eventual.</span></span> <span data-ttu-id="44d13-139">Этот заголовок и `$count` обязательные при использовании `$search` `$filter` с `$orderby` параметром Query.</span><span class="sxs-lookup"><span data-stu-id="44d13-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="44d13-140">Он использует индекс, который может быть не последним в актуальном изменении объекта.</span><span class="sxs-lookup"><span data-stu-id="44d13-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44d13-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44d13-141">Request body</span></span>

<span data-ttu-id="44d13-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44d13-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44d13-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d13-143">Response</span></span>

<span data-ttu-id="44d13-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44d13-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="44d13-145">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="44d13-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="44d13-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="44d13-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="44d13-147">Пример 1: получение списка групп</span><span class="sxs-lookup"><span data-stu-id="44d13-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="44d13-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d13-148">Request</span></span>

<span data-ttu-id="44d13-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d13-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44d13-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="44d13-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="44d13-151">C#</span><span class="sxs-lookup"><span data-stu-id="44d13-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44d13-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44d13-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44d13-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44d13-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="44d13-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d13-154">Response</span></span>

<span data-ttu-id="44d13-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44d13-155">The following is an example of the response.</span></span>
><span data-ttu-id="44d13-156">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="44d13-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="44d13-157">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="44d13-157">All the default properties are returned for each group in an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
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

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="44d13-158">Пример 2: получение отфильтрованного списка групп, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="44d13-158">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="44d13-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d13-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="44d13-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="44d13-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="44d13-161">C#</span><span class="sxs-lookup"><span data-stu-id="44d13-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44d13-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44d13-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44d13-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44d13-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44d13-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d13-164">Response</span></span>

<span data-ttu-id="44d13-165">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="44d13-165">The following is an example of the response which includes only the requested properties.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
  "@odata.count":2,
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "displayName": "Contoso Group 1"
    },
    {
      "id": "22222222-3333-4444-5555-666666666666",
      "displayName": "Contoso Group 2"
    }
  ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="44d13-166">Пример 3: получение только количества групп</span><span class="sxs-lookup"><span data-stu-id="44d13-166">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="44d13-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d13-167">Request</span></span>

<span data-ttu-id="44d13-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d13-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="44d13-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="44d13-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="44d13-170">C#</span><span class="sxs-lookup"><span data-stu-id="44d13-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44d13-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44d13-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44d13-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44d13-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44d13-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d13-173">Response</span></span>

<span data-ttu-id="44d13-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44d13-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="44d13-175">893</span><span class="sxs-lookup"><span data-stu-id="44d13-175">893</span></span>


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="44d13-176">Пример 4: используйте $filter и $top, чтобы получить одну группу с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="44d13-176">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="44d13-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d13-177">Request</span></span>

<span data-ttu-id="44d13-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d13-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="44d13-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="44d13-179">Response</span></span>

<span data-ttu-id="44d13-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44d13-180">The following is an example of the response.</span></span>
><span data-ttu-id="44d13-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44d13-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mailNickname":"a241"
    }
  ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="44d13-183">Пример 5: использование $search для получения групп с отображаемыми именами, которые содержат видео "Video", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="44d13-183">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="44d13-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d13-184">Request</span></span>

<span data-ttu-id="44d13-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d13-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="44d13-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="44d13-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="44d13-187">C#</span><span class="sxs-lookup"><span data-stu-id="44d13-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44d13-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44d13-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44d13-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44d13-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44d13-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d13-190">Response</span></span>

<span data-ttu-id="44d13-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44d13-191">The following is an example of the response.</span></span>
><span data-ttu-id="44d13-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44d13-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="44d13-194">Пример 6: использование $search для получения групп с отображаемыми именами, содержащими "Video" или описание, которое содержит буквы "произ", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="44d13-194">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="44d13-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d13-195">Request</span></span>

<span data-ttu-id="44d13-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d13-196">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="44d13-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="44d13-197">Response</span></span>

<span data-ttu-id="44d13-198">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44d13-198">The following is an example of the response.</span></span>
><span data-ttu-id="44d13-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44d13-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    },
    {
      "description":"Video Production",
      "displayName":"Video Production",
      "mail":"videoprod@service.contoso.com",
      "mailNickname":"VideoProduction"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
