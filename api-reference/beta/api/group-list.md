---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4e0069df916b3a29759ee164c15aac7dc1fcb2ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419109"
---
# <a name="list-groups"></a><span data-ttu-id="7a245-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="7a245-103">List groups</span></span>

<span data-ttu-id="7a245-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a245-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a245-105">Список всех групп в организации, в том числе групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="7a245-105">List all the groups in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="7a245-106">Эта операция по умолчанию возвращает для каждой группы только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="7a245-106">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="7a245-107">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="7a245-107">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="7a245-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="7a245-108">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="7a245-109">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="7a245-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a245-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a245-110">Permissions</span></span>
<span data-ttu-id="7a245-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a245-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a245-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a245-113">Permission type</span></span>      | <span data-ttu-id="7a245-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a245-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a245-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a245-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7a245-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a245-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7a245-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a245-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a245-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a245-118">Not supported.</span></span>    |
|<span data-ttu-id="7a245-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a245-119">Application</span></span> | <span data-ttu-id="7a245-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a245-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a245-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a245-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a245-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a245-122">Optional query parameters</span></span>

<span data-ttu-id="7a245-123">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="7a245-123">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="7a245-124">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="7a245-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="7a245-125">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7a245-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a245-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a245-126">Request headers</span></span>
| <span data-ttu-id="7a245-127">Имя</span><span class="sxs-lookup"><span data-stu-id="7a245-127">Name</span></span>       | <span data-ttu-id="7a245-128">Тип</span><span class="sxs-lookup"><span data-stu-id="7a245-128">Type</span></span> | <span data-ttu-id="7a245-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7a245-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a245-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a245-130">Authorization</span></span>  | <span data-ttu-id="7a245-131">string</span><span class="sxs-lookup"><span data-stu-id="7a245-131">string</span></span>  | <span data-ttu-id="7a245-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a245-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a245-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a245-134">Request body</span></span>
<span data-ttu-id="7a245-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a245-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a245-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a245-136">Response</span></span>
<span data-ttu-id="7a245-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a245-137">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="7a245-138">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="7a245-138">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="7a245-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7a245-139">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="7a245-140">Пример 1. Возвращение списка объектов group</span><span class="sxs-lookup"><span data-stu-id="7a245-140">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="7a245-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a245-141">Request</span></span>

<span data-ttu-id="7a245-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a245-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a245-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a245-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[<span data-ttu-id="7a245-144">C#</span><span class="sxs-lookup"><span data-stu-id="7a245-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a245-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a245-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a245-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a245-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7a245-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a245-147">Response</span></span>

<span data-ttu-id="7a245-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7a245-148">The following is an example of the response.</span></span>
><span data-ttu-id="7a245-149">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7a245-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7a245-150">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="7a245-150">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups"
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


### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="7a245-151">Пример 2. Возвращение отфильтрованного списка объектов group</span><span class="sxs-lookup"><span data-stu-id="7a245-151">Example 2: Return a filtered list of group objects</span></span> 

#### <a name="request"></a><span data-ttu-id="7a245-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a245-152">Request</span></span>

<span data-ttu-id="7a245-153">В этом примере используется параметр запроса `$filter` для получения групп, содержащих участников с ошибками в лицензиях из назначения лицензий на основе группы.</span><span class="sxs-lookup"><span data-stu-id="7a245-153">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="7a245-154">Кроме того, параметр запроса `$select` используется для получения только свойств **id** и **displayName** в отклике для каждой группы, а не других свойств, заданных по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="7a245-154">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a245-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a245-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```
# <a name="c"></a>[<span data-ttu-id="7a245-156">C#</span><span class="sxs-lookup"><span data-stu-id="7a245-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a245-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a245-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a245-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a245-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7a245-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a245-159">Response</span></span>

<span data-ttu-id="7a245-160">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="7a245-160">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups_withlicenseerrors"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
    "value": [
        {
            "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
            "displayName": "Library Assist"
        },
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "displayName": "Golf Assist"
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
