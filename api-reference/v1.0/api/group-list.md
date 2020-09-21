---
title: Список групп
description: Список всех групп, доступных в организации, в том числе групп Microsoft 365.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4dd291610e6c25a916a76a72768a5dd456171b2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057558"
---
# <a name="list-groups"></a><span data-ttu-id="a73d7-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="a73d7-103">List groups</span></span>

<span data-ttu-id="a73d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a73d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a73d7-105">Список всех групп в организации, в том числе групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a73d7-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="a73d7-106">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="a73d7-106">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="a73d7-107">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="a73d7-107">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="a73d7-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию [GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="a73d7-108">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="a73d7-109">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="a73d7-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="a73d7-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a73d7-110">Permissions</span></span>
<span data-ttu-id="a73d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a73d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a73d7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a73d7-113">Permission type</span></span>      | <span data-ttu-id="a73d7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a73d7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a73d7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a73d7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a73d7-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a73d7-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a73d7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a73d7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a73d7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a73d7-118">Not supported.</span></span>    |
|<span data-ttu-id="a73d7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a73d7-119">Application</span></span> | <span data-ttu-id="a73d7-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a73d7-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a73d7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a73d7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a73d7-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a73d7-122">Optional query parameters</span></span>
<span data-ttu-id="a73d7-123">Чтобы показать список только групп Microsoft 365 (т. н. единых групп), примените фильтр для **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="a73d7-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="a73d7-124">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="a73d7-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="a73d7-125">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a73d7-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a73d7-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a73d7-126">Request headers</span></span>
| <span data-ttu-id="a73d7-127">Имя</span><span class="sxs-lookup"><span data-stu-id="a73d7-127">Name</span></span>       | <span data-ttu-id="a73d7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a73d7-128">Type</span></span> | <span data-ttu-id="a73d7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a73d7-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a73d7-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a73d7-130">Authorization</span></span>  | <span data-ttu-id="a73d7-131">string</span><span class="sxs-lookup"><span data-stu-id="a73d7-131">string</span></span>  | <span data-ttu-id="a73d7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a73d7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a73d7-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a73d7-134">Request body</span></span>
<span data-ttu-id="a73d7-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a73d7-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a73d7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a73d7-136">Response</span></span>
<span data-ttu-id="a73d7-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a73d7-137">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="a73d7-138">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="a73d7-138">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="a73d7-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a73d7-139">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="a73d7-140">Пример 1. Возвращение списка объектов group</span><span class="sxs-lookup"><span data-stu-id="a73d7-140">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="a73d7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a73d7-141">Request</span></span>

<span data-ttu-id="a73d7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a73d7-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a73d7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a73d7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups
```
# <a name="c"></a>[<span data-ttu-id="a73d7-144">C#</span><span class="sxs-lookup"><span data-stu-id="a73d7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a73d7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a73d7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a73d7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a73d7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a73d7-147">Java</span><span class="sxs-lookup"><span data-stu-id="a73d7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a73d7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a73d7-148">Response</span></span>

<span data-ttu-id="a73d7-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a73d7-149">The following is an example of the response.</span></span>

><span data-ttu-id="a73d7-150">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a73d7-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a73d7-151">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="a73d7-151">All the default properties are returned for each group in an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-12-22T02:21:05Z",
            "creationOptions": [],
            "description": "Self help community for golf",
            "displayName": "Golf Assist",
            "groupTypes": [
                "Unified"
            ],
            "mail": "golfassist@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golfassist",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golfassist@contoso.onmicrosoft.com",
                "SMTP:golfassist@contoso.com"
            ],
            "renewedDateTime": "2018-12-22T02:21:05Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": "Public",
            "onPremisesProvisioningErrors": []
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "creationOptions": [],
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```


### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="a73d7-152">Пример 2. Возвращение отфильтрованного списка объектов group</span><span class="sxs-lookup"><span data-stu-id="a73d7-152">Example 2: Return a filtered list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="a73d7-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a73d7-153">Request</span></span>

<span data-ttu-id="a73d7-154">В этом примере используется параметр запроса `$filter` для получения групп, содержащих участников с ошибками в лицензиях из назначения лицензий на основе группы.</span><span class="sxs-lookup"><span data-stu-id="a73d7-154">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="a73d7-155">Кроме того, параметр запроса `$select` используется для получения только свойств **id** и **displayName** в отклике для каждой группы, а не других свойств, заданных по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="a73d7-155">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="a73d7-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="a73d7-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```
# <a name="c"></a>[<span data-ttu-id="a73d7-157">C#</span><span class="sxs-lookup"><span data-stu-id="a73d7-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a73d7-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a73d7-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a73d7-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a73d7-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a73d7-160">Java</span><span class="sxs-lookup"><span data-stu-id="a73d7-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-withlicenseerrors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a73d7-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a73d7-161">Response</span></span>

<span data-ttu-id="a73d7-162">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="a73d7-162">The following is an example of the response which includes only the requested properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
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
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

