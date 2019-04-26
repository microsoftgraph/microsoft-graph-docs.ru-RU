---
title: Список групп
description: Список всех групп, доступных в организации, в том числе Групп Office 365.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 8ede194abffe745bee9a23906b965d43de93cec8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561840"
---
# <a name="list-groups"></a><span data-ttu-id="f37e9-103">Список групп</span><span class="sxs-lookup"><span data-stu-id="f37e9-103">List groups</span></span>
<span data-ttu-id="f37e9-104">Список всех групп, доступных в организации, в том числе Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="f37e9-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span>

<span data-ttu-id="f37e9-105">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="f37e9-105">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="f37e9-106">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="f37e9-106">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="f37e9-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию [GET](group-get.md) и укажите их в параметре `$select` запроса OData.</span><span class="sxs-lookup"><span data-stu-id="f37e9-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="f37e9-108">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="f37e9-108">See an [example](group-get.md#request-2).</span></span>

<span data-ttu-id="f37e9-109">Исключением является свойство **hasMembersWithLicenseErrors**.</span><span class="sxs-lookup"><span data-stu-id="f37e9-109">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="f37e9-110">См. [пример](#request-2) использования этого свойства.</span><span class="sxs-lookup"><span data-stu-id="f37e9-110">See an [example](#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f37e9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f37e9-111">Permissions</span></span>
<span data-ttu-id="f37e9-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f37e9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f37e9-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f37e9-114">Permission type</span></span>      | <span data-ttu-id="f37e9-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f37e9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f37e9-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f37e9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f37e9-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37e9-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f37e9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f37e9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f37e9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f37e9-119">Not supported.</span></span>    |
|<span data-ttu-id="f37e9-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f37e9-120">Application</span></span> | <span data-ttu-id="f37e9-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37e9-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f37e9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f37e9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f37e9-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f37e9-123">Optional query parameters</span></span>
<span data-ttu-id="f37e9-124">Чтобы получить только результаты из функции "Группы Office 365" (т. н. единые группы), примените фильтр **groupTypes**:</span><span class="sxs-lookup"><span data-stu-id="f37e9-124">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="f37e9-125">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="f37e9-125">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="f37e9-126">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f37e9-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f37e9-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f37e9-127">Request headers</span></span>
| <span data-ttu-id="f37e9-128">Имя</span><span class="sxs-lookup"><span data-stu-id="f37e9-128">Name</span></span>       | <span data-ttu-id="f37e9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f37e9-129">Type</span></span> | <span data-ttu-id="f37e9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f37e9-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f37e9-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f37e9-131">Authorization</span></span>  | <span data-ttu-id="f37e9-132">string</span><span class="sxs-lookup"><span data-stu-id="f37e9-132">string</span></span>  | <span data-ttu-id="f37e9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f37e9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f37e9-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f37e9-135">Request body</span></span>
<span data-ttu-id="f37e9-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f37e9-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f37e9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f37e9-137">Response</span></span>
<span data-ttu-id="f37e9-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f37e9-138">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="f37e9-139">Отклик включает в себя только свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="f37e9-139">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="f37e9-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f37e9-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="f37e9-141">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="f37e9-141">Request 1</span></span>
<span data-ttu-id="f37e9-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f37e9-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response-1"></a><span data-ttu-id="f37e9-143">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="f37e9-143">Response 1</span></span>
<span data-ttu-id="f37e9-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f37e9-144">The following is an example of the response.</span></span>

><span data-ttu-id="f37e9-145">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f37e9-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f37e9-146">В результате реального вызова возвращаются все свойства по умолчанию для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="f37e9-146">All the default properties are returned for each group in an actual call.</span></span>

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
#### <a name="request-2"></a><span data-ttu-id="f37e9-147">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="f37e9-147">Request 2</span></span>
<span data-ttu-id="f37e9-148">В этом примере используется параметр запроса `$filter` для получения групп, содержащих участников с ошибками в лицензиях из назначения лицензий на основе группы.</span><span class="sxs-lookup"><span data-stu-id="f37e9-148">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="f37e9-149">Кроме того, параметр запроса `$select` используется для получения только свойств **id** и **displayName** в отклике для каждой группы, а не других свойств, заданных по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="f37e9-149">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```

#### <a name="response-2"></a><span data-ttu-id="f37e9-150">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="f37e9-150">Response 2</span></span>
<span data-ttu-id="f37e9-151">Ниже приведен пример отклика, содержащего только запрашиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="f37e9-151">The following is an example of the response which includes only the requested properties.</span></span>

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
  "tocPath": ""
}-->
