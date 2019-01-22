---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 393381bfe5f21c4d4196251a4055fc65e0771e5c
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726605"
---
# <a name="list-groups"></a><span data-ttu-id="13f1a-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="13f1a-103">List groups</span></span>

> <span data-ttu-id="13f1a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13f1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13f1a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13f1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13f1a-106">Список всех групп, доступных в организации, в том числе Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="13f1a-106">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="13f1a-107">Эта операция по умолчанию возвращает для каждой группы только подмножество наиболее часто используемых свойств.</span><span class="sxs-lookup"><span data-stu-id="13f1a-107">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="13f1a-108">Эти свойства _по умолчанию_ указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="13f1a-108">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="13f1a-109">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию [GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="13f1a-109">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="13f1a-110">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="13f1a-110">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="13f1a-111">Исключением является свойство **hasMembersWithLicenseErrors**.</span><span class="sxs-lookup"><span data-stu-id="13f1a-111">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="13f1a-112">См. [пример](#request-2) использования этого свойства.</span><span class="sxs-lookup"><span data-stu-id="13f1a-112">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="13f1a-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13f1a-113">Permissions</span></span>
<span data-ttu-id="13f1a-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13f1a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13f1a-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13f1a-116">Permission type</span></span>      | <span data-ttu-id="13f1a-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13f1a-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13f1a-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13f1a-118">Delegated (work or school account)</span></span> | <span data-ttu-id="13f1a-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f1a-119">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="13f1a-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13f1a-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13f1a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13f1a-121">Not supported.</span></span>    |
|<span data-ttu-id="13f1a-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13f1a-122">Application</span></span> | <span data-ttu-id="13f1a-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f1a-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13f1a-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13f1a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13f1a-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="13f1a-125">Optional query parameters</span></span>

<span data-ttu-id="13f1a-126">Чтобы показать список только Групп Office 365 (т. н. единых групп), примените фильтр для **groupTypes**: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13f1a-126">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="13f1a-127">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="13f1a-127">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="13f1a-128">Дополнительную информацию о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="13f1a-128">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="13f1a-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13f1a-129">Request headers</span></span>
| <span data-ttu-id="13f1a-130">Имя</span><span class="sxs-lookup"><span data-stu-id="13f1a-130">Name</span></span>       | <span data-ttu-id="13f1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13f1a-131">Type</span></span> | <span data-ttu-id="13f1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13f1a-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="13f1a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="13f1a-133">Authorization</span></span>  | <span data-ttu-id="13f1a-134">string</span><span class="sxs-lookup"><span data-stu-id="13f1a-134">string</span></span>  | <span data-ttu-id="13f1a-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13f1a-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13f1a-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13f1a-137">Request body</span></span>
<span data-ttu-id="13f1a-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13f1a-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13f1a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="13f1a-139">Response</span></span>
<span data-ttu-id="13f1a-140">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13f1a-140">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="13f1a-141">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="13f1a-141">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="13f1a-142">Пример</span><span class="sxs-lookup"><span data-stu-id="13f1a-142">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="13f1a-143">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="13f1a-143">Request 1</span></span>
<span data-ttu-id="13f1a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13f1a-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response-1"></a><span data-ttu-id="13f1a-145">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="13f1a-145">Response 1</span></span>
<span data-ttu-id="13f1a-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13f1a-146">The following is an example of the response.</span></span>
><span data-ttu-id="13f1a-147">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="13f1a-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13f1a-148">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="13f1a-148">All the default properties are returned for each group in an actual call.</span></span>

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

#### <a name="request-2"></a><span data-ttu-id="13f1a-149">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="13f1a-149">Request 2</span></span>
<span data-ttu-id="13f1a-150">В этом примере используется параметр запроса `$filter` для получения групп, содержащих участников с ошибками в лицензиях из назначения лицензий на основе группы.</span><span class="sxs-lookup"><span data-stu-id="13f1a-150">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="13f1a-151">Кроме того, параметр запроса `$select` используется для получения только свойств **id** и **displayName** в отклике для каждой группы, а не других свойств, заданных по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="13f1a-151">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="13f1a-152">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="13f1a-152">Response 2</span></span>
<span data-ttu-id="13f1a-153">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="13f1a-153">The following is an example of the response which includes only the requested properties.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
