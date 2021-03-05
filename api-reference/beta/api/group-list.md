---
title: Список групп
description: Список всех групп, доступных в организации, в том числе групп Microsoft 365.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b2f6170ce88c7f6c570f3bc0774898d0aa6bd256
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471050"
---
# <a name="list-groups"></a><span data-ttu-id="55278-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="55278-103">List groups</span></span>

<span data-ttu-id="55278-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55278-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55278-105">Список всех групп в организации, в том числе групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55278-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="55278-106">Эта операция по умолчанию возвращает для каждой группы только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="55278-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="55278-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="55278-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="55278-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="55278-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="55278-109">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="55278-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="55278-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55278-110">Permissions</span></span>

<span data-ttu-id="55278-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55278-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55278-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55278-113">Permission type</span></span> | <span data-ttu-id="55278-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55278-114">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="55278-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55278-115">Delegated (work or school account)</span></span> | <span data-ttu-id="55278-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55278-116">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="55278-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55278-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55278-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55278-118">Not supported.</span></span> |
| <span data-ttu-id="55278-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55278-119">Application</span></span> | <span data-ttu-id="55278-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55278-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55278-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55278-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55278-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55278-122">Optional query parameters</span></span>

<span data-ttu-id="55278-123">Чтобы показать список только групп Microsoft 365 (т. н. единых групп), примените фильтр для **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="55278-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="55278-124">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="55278-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```
<span data-ttu-id="55278-125">Вы также можете использовать параметры запроса `$count` и `$search`, чтобы ограничить ответ.</span><span class="sxs-lookup"><span data-stu-id="55278-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="55278-126">Параметр запроса `$search` поддерживает разметку только в полях **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="55278-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="55278-127">По умолчанию в других полях используется действие `$filter`.</span><span class="sxs-lookup"><span data-stu-id="55278-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="55278-128">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="55278-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="55278-129">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="55278-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="55278-130">Дополнительные сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="55278-130">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="55278-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55278-131">Request headers</span></span>

| <span data-ttu-id="55278-132">Имя</span><span class="sxs-lookup"><span data-stu-id="55278-132">Name</span></span> | <span data-ttu-id="55278-133">Описание</span><span class="sxs-lookup"><span data-stu-id="55278-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="55278-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55278-134">Authorization</span></span>  | <span data-ttu-id="55278-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55278-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55278-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="55278-137">ConsistencyLevel</span></span> | <span data-ttu-id="55278-138">необязательный.</span><span class="sxs-lookup"><span data-stu-id="55278-138">eventual.</span></span> <span data-ttu-id="55278-139">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="55278-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="55278-140">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="55278-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55278-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55278-141">Request body</span></span>

<span data-ttu-id="55278-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55278-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55278-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-143">Response</span></span>

<span data-ttu-id="55278-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55278-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="55278-145">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="55278-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="55278-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="55278-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="55278-147">Пример 1. Получение списка групп</span><span class="sxs-lookup"><span data-stu-id="55278-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="55278-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="55278-148">Request</span></span>

<span data-ttu-id="55278-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55278-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55278-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="55278-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="55278-151">C#</span><span class="sxs-lookup"><span data-stu-id="55278-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55278-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55278-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55278-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55278-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55278-154">Java</span><span class="sxs-lookup"><span data-stu-id="55278-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="55278-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-155">Response</span></span>

<span data-ttu-id="55278-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55278-156">The following is an example of the response.</span></span>
><span data-ttu-id="55278-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="55278-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55278-158">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="55278-158">All the default properties are returned for each group in an actual call.</span></span>

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
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-12-22T02:21:05Z",
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "expirationDateTime": null,
            "groupTypes": [
                "Unified"
            ],
            "isAssignableToRole": null,
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "membershipRule": null,
            "membershipRuleProcessingState": null,
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "preferredLanguage": null,
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "theme": null,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "expirationDateTime": null,
            "groupTypes": [],
            "isAssignableToRole": null,
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "membershipRule": null,
            "membershipRuleProcessingState": null,
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "preferredLanguage": null,
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "theme": null,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}
```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="55278-159">Пример 2. Получение отфильтрованного списка групп, включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="55278-159">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="55278-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="55278-160">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55278-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-161">Response</span></span>

<span data-ttu-id="55278-162">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="55278-162">The following is an example of the response which includes only the requested properties.</span></span>

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

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="55278-163">Пример 3. Получение только количества групп</span><span class="sxs-lookup"><span data-stu-id="55278-163">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="55278-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="55278-164">Request</span></span>

<span data-ttu-id="55278-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55278-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55278-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-166">Response</span></span>

<span data-ttu-id="55278-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55278-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="55278-168">893</span><span class="sxs-lookup"><span data-stu-id="55278-168">893</span></span>


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="55278-169">Пример 4. Использование параметров $filter и $top для получения группы с отображаемым именем, которое начинается с "а", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="55278-169">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="55278-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="55278-170">Request</span></span>

<span data-ttu-id="55278-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55278-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55278-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-172">Response</span></span>

<span data-ttu-id="55278-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55278-173">The following is an example of the response.</span></span>
><span data-ttu-id="55278-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55278-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="55278-176">Пример 5. Использование параметра $search для получения групп с отображаемыми именами, содержащими буквы "Video", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="55278-176">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="55278-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="55278-177">Request</span></span>

<span data-ttu-id="55278-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55278-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55278-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-179">Response</span></span>

<span data-ttu-id="55278-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55278-180">The following is an example of the response.</span></span>
><span data-ttu-id="55278-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55278-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="55278-183">Пример 6. Использование параметра $search для получения групп с отображаемыми именами, содержащими буквы "Video", или описания, содержащего буквы "prod", включая количество возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="55278-183">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="55278-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="55278-184">Request</span></span>

<span data-ttu-id="55278-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55278-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="55278-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-186">Response</span></span>

<span data-ttu-id="55278-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55278-187">The following is an example of the response.</span></span>
><span data-ttu-id="55278-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55278-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-7-list-dynamic-groups-filtered-by-enabled-membershipruleprocessingstate"></a><span data-ttu-id="55278-190">Пример 7. Перечисление динамических групп, отфильтрованных по включенному свойству membershipRuleProcessingState</span><span class="sxs-lookup"><span data-stu-id="55278-190">Example 7: List dynamic groups, filtered by enabled membershipRuleProcessingState</span></span>

#### <a name="request"></a><span data-ttu-id="55278-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="55278-191">Request</span></span>

<span data-ttu-id="55278-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55278-192">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="55278-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="55278-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_enabled_dynamic_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$select=id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus&$filter=membershipRuleProcessingState eq 'On'
```
# <a name="c"></a>[<span data-ttu-id="55278-194">C#</span><span class="sxs-lookup"><span data-stu-id="55278-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-enabled-dynamic-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55278-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55278-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-enabled-dynamic-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55278-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55278-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-enabled-dynamic-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55278-197">Java</span><span class="sxs-lookup"><span data-stu-id="55278-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-enabled-dynamic-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55278-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="55278-198">Response</span></span>

<span data-ttu-id="55278-199">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="55278-199">The following is an example of the response.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus)",
  "value":[
    {
      "id": "1cdf9c18-a7dc-46b1-b47f-094d5656376d",
      "membershipRule": "user.accountEnabled -eq false",
      "membershipRuleProcessingState": "On",
      "membershipRuleProcessingStatus": {
          "status" : "Succeeded",
          "lastMembershipUpdated"  : "2020-09-14T00:00:00Z",
          "errorMessage" : null
        }
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


