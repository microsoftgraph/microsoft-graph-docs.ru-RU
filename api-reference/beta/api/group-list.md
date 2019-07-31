---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 11faba0b03b2e82c3086481dab617cd34ffa0d64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953628"
---
# <a name="list-groups"></a><span data-ttu-id="76946-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="76946-103">List groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76946-104">Список всех групп в организации, в том числе групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="76946-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="76946-105">Эта операция по умолчанию возвращает для каждой группы только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="76946-105">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="76946-106">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="76946-106">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="76946-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="76946-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="76946-108">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="76946-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="76946-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76946-109">Permissions</span></span>
<span data-ttu-id="76946-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76946-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76946-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76946-112">Permission type</span></span>      | <span data-ttu-id="76946-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76946-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76946-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76946-114">Delegated (work or school account)</span></span> | <span data-ttu-id="76946-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="76946-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="76946-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76946-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76946-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76946-117">Not supported.</span></span>    |
|<span data-ttu-id="76946-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76946-118">Application</span></span> | <span data-ttu-id="76946-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76946-119">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76946-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76946-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76946-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76946-121">Optional query parameters</span></span>

<span data-ttu-id="76946-122">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="76946-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="76946-123">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="76946-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="76946-124">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="76946-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="76946-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76946-125">Request headers</span></span>
| <span data-ttu-id="76946-126">Имя</span><span class="sxs-lookup"><span data-stu-id="76946-126">Name</span></span>       | <span data-ttu-id="76946-127">Тип</span><span class="sxs-lookup"><span data-stu-id="76946-127">Type</span></span> | <span data-ttu-id="76946-128">Описание</span><span class="sxs-lookup"><span data-stu-id="76946-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="76946-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="76946-129">Authorization</span></span>  | <span data-ttu-id="76946-130">string</span><span class="sxs-lookup"><span data-stu-id="76946-130">string</span></span>  | <span data-ttu-id="76946-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76946-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76946-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76946-133">Request body</span></span>
<span data-ttu-id="76946-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76946-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76946-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="76946-135">Response</span></span>
<span data-ttu-id="76946-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76946-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="76946-137">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="76946-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="76946-138">Пример</span><span class="sxs-lookup"><span data-stu-id="76946-138">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="76946-139">Пример 1. Возвращение списка объектов group</span><span class="sxs-lookup"><span data-stu-id="76946-139">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="76946-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="76946-140">Request</span></span>

<span data-ttu-id="76946-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76946-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76946-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="76946-142">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76946-143">C#</span><span class="sxs-lookup"><span data-stu-id="76946-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76946-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76946-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76946-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76946-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="76946-146">Java</span><span class="sxs-lookup"><span data-stu-id="76946-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="76946-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="76946-147">Response</span></span>

<span data-ttu-id="76946-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="76946-148">The following is an example of the response.</span></span>
><span data-ttu-id="76946-149">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="76946-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="76946-150">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="76946-150">All the default properties are returned for each group in an actual call.</span></span>

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


### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="76946-151">Пример 2. Возвращение отфильтрованного списка объектов group</span><span class="sxs-lookup"><span data-stu-id="76946-151">Example 2: Return a filtered list of group objects</span></span> 

#### <a name="request"></a><span data-ttu-id="76946-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="76946-152">Request</span></span>

<span data-ttu-id="76946-153">В этом примере используется параметр запроса `$filter` для получения групп, содержащих участников с ошибками в лицензиях из назначения лицензий на основе группы.</span><span class="sxs-lookup"><span data-stu-id="76946-153">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="76946-154">Кроме того, параметр запроса `$select` используется для получения только свойств **id** и **displayName** в отклике для каждой группы, а не других свойств, заданных по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="76946-154">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76946-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="76946-155">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76946-156">C#</span><span class="sxs-lookup"><span data-stu-id="76946-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76946-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76946-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76946-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76946-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="76946-159">Java</span><span class="sxs-lookup"><span data-stu-id="76946-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-withlicenseerrors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="76946-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="76946-160">Response</span></span>

<span data-ttu-id="76946-161">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="76946-161">The following is an example of the response which includes only the requested properties.</span></span>

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
