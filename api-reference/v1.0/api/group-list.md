---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5081c5013c1bf7c1a1bfbcff58afe5a83aa67bc9
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726577"
---
# <a name="list-groups"></a><span data-ttu-id="af8bc-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="af8bc-103">List groups</span></span>
<span data-ttu-id="af8bc-104">Список всех групп, доступных в организации, в том числе Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="af8bc-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="af8bc-105">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="af8bc-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="af8bc-106">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="af8bc-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="af8bc-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию [GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="af8bc-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="af8bc-108">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="af8bc-108">See an [example](group-get.md#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="af8bc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af8bc-109">Permissions</span></span>
<span data-ttu-id="af8bc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af8bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af8bc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af8bc-112">Permission type</span></span>      | <span data-ttu-id="af8bc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af8bc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af8bc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af8bc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="af8bc-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af8bc-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="af8bc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af8bc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af8bc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af8bc-117">Not supported.</span></span>    |
|<span data-ttu-id="af8bc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af8bc-118">Application</span></span> | <span data-ttu-id="af8bc-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af8bc-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af8bc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af8bc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af8bc-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="af8bc-121">Optional query parameters</span></span>
<span data-ttu-id="af8bc-122">Чтобы показать список только Групп Office 365 (т. н. единых групп), примените фильтр для **groupTypes**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="af8bc-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="af8bc-123">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="af8bc-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="af8bc-124">Дополнительную информацию о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="af8bc-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="af8bc-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af8bc-125">Request headers</span></span>
| <span data-ttu-id="af8bc-126">Имя</span><span class="sxs-lookup"><span data-stu-id="af8bc-126">Name</span></span>       | <span data-ttu-id="af8bc-127">Тип</span><span class="sxs-lookup"><span data-stu-id="af8bc-127">Type</span></span> | <span data-ttu-id="af8bc-128">Описание</span><span class="sxs-lookup"><span data-stu-id="af8bc-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af8bc-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="af8bc-129">Authorization</span></span>  | <span data-ttu-id="af8bc-130">string</span><span class="sxs-lookup"><span data-stu-id="af8bc-130">string</span></span>  | <span data-ttu-id="af8bc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af8bc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af8bc-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af8bc-133">Request body</span></span>
<span data-ttu-id="af8bc-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af8bc-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af8bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="af8bc-135">Response</span></span>
<span data-ttu-id="af8bc-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af8bc-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="af8bc-137">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="af8bc-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="af8bc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="af8bc-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="af8bc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="af8bc-139">Request</span></span>
<span data-ttu-id="af8bc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af8bc-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="af8bc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="af8bc-141">Response</span></span>
<span data-ttu-id="af8bc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af8bc-142">The following is an example of the response.</span></span>

><span data-ttu-id="af8bc-143">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af8bc-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="af8bc-144">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="af8bc-144">All the default properties are returned for each group in an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
