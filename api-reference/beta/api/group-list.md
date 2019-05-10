---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a4149954da3bacf7b0a327112b297d7a693f6035
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592878"
---
# <a name="list-groups"></a><span data-ttu-id="0a868-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="0a868-103">List groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a868-104">Список всех групп, доступных в организации, в том числе Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="0a868-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="0a868-105">Эта операция по умолчанию возвращает для каждой группы только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="0a868-105">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="0a868-106">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="0a868-106">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="0a868-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию [GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="0a868-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="0a868-108">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="0a868-108">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="0a868-109">Исключением является свойство **hasMembersWithLicenseErrors**.</span><span class="sxs-lookup"><span data-stu-id="0a868-109">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="0a868-110">См. [пример](#request-2) использования этого свойства.</span><span class="sxs-lookup"><span data-stu-id="0a868-110">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a868-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a868-111">Permissions</span></span>
<span data-ttu-id="0a868-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a868-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a868-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a868-114">Permission type</span></span>      | <span data-ttu-id="0a868-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a868-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a868-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a868-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0a868-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a868-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a868-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a868-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a868-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a868-119">Not supported.</span></span>    |
|<span data-ttu-id="0a868-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a868-120">Application</span></span> | <span data-ttu-id="0a868-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a868-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a868-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a868-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a868-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a868-123">Optional query parameters</span></span>

<span data-ttu-id="0a868-124">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="0a868-124">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="0a868-125">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="0a868-125">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="0a868-126">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0a868-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a868-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a868-127">Request headers</span></span>
| <span data-ttu-id="0a868-128">Имя</span><span class="sxs-lookup"><span data-stu-id="0a868-128">Name</span></span>       | <span data-ttu-id="0a868-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0a868-129">Type</span></span> | <span data-ttu-id="0a868-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0a868-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0a868-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a868-131">Authorization</span></span>  | <span data-ttu-id="0a868-132">string</span><span class="sxs-lookup"><span data-stu-id="0a868-132">string</span></span>  | <span data-ttu-id="0a868-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a868-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a868-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a868-135">Request body</span></span>
<span data-ttu-id="0a868-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a868-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a868-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a868-137">Response</span></span>
<span data-ttu-id="0a868-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a868-138">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="0a868-139">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="0a868-139">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="0a868-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0a868-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="0a868-141">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="0a868-141">Request 1</span></span>
<span data-ttu-id="0a868-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a868-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response-1"></a><span data-ttu-id="0a868-143">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="0a868-143">Response 1</span></span>
<span data-ttu-id="0a868-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a868-144">The following is an example of the response.</span></span>
><span data-ttu-id="0a868-145">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a868-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0a868-146">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="0a868-146">All the default properties are returned for each group in an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a868-147">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="0a868-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a868-148">C#</span><span class="sxs-lookup"><span data-stu-id="0a868-148">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a868-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a868-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="0a868-150">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="0a868-150">Request 2</span></span>
<span data-ttu-id="0a868-151">В этом примере используется параметр запроса `$filter` для получения групп, содержащих участников с ошибками в лицензиях из назначения лицензий на основе группы.</span><span class="sxs-lookup"><span data-stu-id="0a868-151">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="0a868-152">Кроме того, параметр запроса `$select` используется для получения только свойств **id** и **displayName** в отклике для каждой группы, а не других свойств, заданных по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="0a868-152">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="0a868-153">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="0a868-153">Response 2</span></span>
<span data-ttu-id="0a868-154">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="0a868-154">The following is an example of the response which includes only the requested properties.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0a868-155">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="0a868-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0a868-156">C#</span><span class="sxs-lookup"><span data-stu-id="0a868-156">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a868-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a868-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groups_withlicenseerrors-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
