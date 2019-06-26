---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 26743ec0be606bc76466c6fa680824d4d2f8914a
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236484"
---
# <a name="list-groups"></a><span data-ttu-id="976b3-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="976b3-103">List groups</span></span>
<span data-ttu-id="976b3-104">Список всех групп в организации, в том числе групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="976b3-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="976b3-105">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="976b3-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="976b3-106">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="976b3-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="976b3-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию [GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="976b3-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="976b3-108">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="976b3-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="976b3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="976b3-109">Permissions</span></span>
<span data-ttu-id="976b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="976b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="976b3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="976b3-112">Permission type</span></span>      | <span data-ttu-id="976b3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="976b3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="976b3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="976b3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="976b3-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="976b3-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="976b3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="976b3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="976b3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="976b3-117">Not supported.</span></span>    |
|<span data-ttu-id="976b3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="976b3-118">Application</span></span> | <span data-ttu-id="976b3-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="976b3-119">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="976b3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="976b3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="976b3-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="976b3-121">Optional query parameters</span></span>
<span data-ttu-id="976b3-122">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="976b3-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="976b3-123">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="976b3-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="976b3-124">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="976b3-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="976b3-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="976b3-125">Request headers</span></span>
| <span data-ttu-id="976b3-126">Имя</span><span class="sxs-lookup"><span data-stu-id="976b3-126">Name</span></span>       | <span data-ttu-id="976b3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="976b3-127">Type</span></span> | <span data-ttu-id="976b3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="976b3-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="976b3-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="976b3-129">Authorization</span></span>  | <span data-ttu-id="976b3-130">string</span><span class="sxs-lookup"><span data-stu-id="976b3-130">string</span></span>  | <span data-ttu-id="976b3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="976b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="976b3-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="976b3-133">Request body</span></span>
<span data-ttu-id="976b3-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="976b3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="976b3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="976b3-135">Response</span></span>
<span data-ttu-id="976b3-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="976b3-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="976b3-137">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="976b3-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="976b3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="976b3-138">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="976b3-139">Пример 1. Возвращение списка объектов group</span><span class="sxs-lookup"><span data-stu-id="976b3-139">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="976b3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="976b3-140">Request</span></span>

<span data-ttu-id="976b3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="976b3-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="976b3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="976b3-142">Response</span></span>

<span data-ttu-id="976b3-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="976b3-143">The following is an example of the response.</span></span>

><span data-ttu-id="976b3-144">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="976b3-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="976b3-145">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="976b3-145">All the default properties are returned for each group in an actual call.</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="976b3-146">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="976b3-146">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="976b3-147">C#</span><span class="sxs-lookup"><span data-stu-id="976b3-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="976b3-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="976b3-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="976b3-149">Пример 2. Возвращение отфильтрованного списка объектов group</span><span class="sxs-lookup"><span data-stu-id="976b3-149">Example 2: Return a filtered list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="976b3-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="976b3-150">Request</span></span>

<span data-ttu-id="976b3-151">В этом примере используется параметр запроса `$filter` для получения групп, содержащих участников с ошибками в лицензиях из назначения лицензий на основе группы.</span><span class="sxs-lookup"><span data-stu-id="976b3-151">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="976b3-152">Кроме того, параметр запроса `$select` используется для получения только свойств **id** и **displayName** в отклике для каждой группы, а не других свойств, заданных по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="976b3-152">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response"></a><span data-ttu-id="976b3-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="976b3-153">Response</span></span>

<span data-ttu-id="976b3-154">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="976b3-154">The following is an example of the response which includes only the requested properties.</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="976b3-155">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="976b3-155">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="976b3-156">C#</span><span class="sxs-lookup"><span data-stu-id="976b3-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="976b3-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="976b3-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
