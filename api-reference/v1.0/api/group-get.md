---
title: Вывод группы
description: Получение свойств и связей объекта group.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 4954ee99b52d3d932421651d17e6b7a8b906f3bf
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641339"
---
# <a name="get-group"></a><span data-ttu-id="f7eec-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="f7eec-103">Get group</span></span>
<span data-ttu-id="f7eec-104">Получение свойств и связей объекта группы.</span><span class="sxs-lookup"><span data-stu-id="f7eec-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="f7eec-105">Это действие по умолчанию возвращает только часть всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="f7eec-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="f7eec-106">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="f7eec-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="f7eec-107">См. [пример](#request-2) для `$select`.</span><span class="sxs-lookup"><span data-stu-id="f7eec-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="f7eec-108">Исключением является свойство **hasMembersWithLicenseErrors**.</span><span class="sxs-lookup"><span data-stu-id="f7eec-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="f7eec-109">См. [пример](group-list.md#request-2) использования этого свойства.</span><span class="sxs-lookup"><span data-stu-id="f7eec-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7eec-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7eec-110">Permissions</span></span>
<span data-ttu-id="f7eec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7eec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7eec-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7eec-113">Permission type</span></span>      | <span data-ttu-id="f7eec-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7eec-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7eec-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7eec-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f7eec-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7eec-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7eec-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7eec-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7eec-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7eec-118">Not supported.</span></span>    |
|<span data-ttu-id="f7eec-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7eec-119">Application</span></span> | <span data-ttu-id="f7eec-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7eec-120">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7eec-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7eec-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7eec-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f7eec-122">Optional query parameters</span></span>
<span data-ttu-id="f7eec-123">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7eec-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="f7eec-124">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="f7eec-124">See an [example](#request-2) below.</span></span>

<span data-ttu-id="f7eec-125">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f7eec-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7eec-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7eec-126">Request headers</span></span>
| <span data-ttu-id="f7eec-127">Имя</span><span class="sxs-lookup"><span data-stu-id="f7eec-127">Name</span></span>       | <span data-ttu-id="f7eec-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f7eec-128">Type</span></span> | <span data-ttu-id="f7eec-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f7eec-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f7eec-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7eec-130">Authorization</span></span>  | <span data-ttu-id="f7eec-131">string</span><span class="sxs-lookup"><span data-stu-id="f7eec-131">string</span></span>  | <span data-ttu-id="f7eec-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7eec-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7eec-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7eec-134">Request body</span></span>
<span data-ttu-id="f7eec-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7eec-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7eec-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7eec-136">Response</span></span>
<span data-ttu-id="f7eec-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7eec-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="f7eec-138">Он возвращает параметры по умолчанию, если не используется параметр `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="f7eec-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="f7eec-139">Пример</span><span class="sxs-lookup"><span data-stu-id="f7eec-139">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="f7eec-140">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="f7eec-140">Request 1</span></span>
<span data-ttu-id="f7eec-141">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="f7eec-141">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="f7eec-142">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="f7eec-142">Response 1</span></span>
<span data-ttu-id="f7eec-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f7eec-143">The following is an example of the response.</span></span> <span data-ttu-id="f7eec-144">Он включает только стандартные свойства.</span><span class="sxs-lookup"><span data-stu-id="f7eec-144">It includes only the default properties.</span></span>

><span data-ttu-id="f7eec-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f7eec-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f7eec-146">В реальном вызове возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7eec-146">All the default properties are returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-22T00:51:37Z",
    "creationOptions": [],
    "description": "Self help community for library",
    "displayName": "Library Assist",
    "groupTypes": [
        "Unified"
    ],
    "mail": "library2@contoso.com",
    "mailEnabled": true,
    "mailNickname": "library",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "smtp:library7423@contoso.com",
        "SMTP:library2@contoso.com"
    ],
    "renewedDateTime": "2018-12-22T00:51:37Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a><span data-ttu-id="f7eec-147">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="f7eec-147">Request 2</span></span>
<span data-ttu-id="f7eec-148">В следующем примере используется параметр запрос `$select`, чтобы получить несколько свойств, которые не найдены по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7eec-148">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="f7eec-149">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="f7eec-149">Response 2</span></span>
<span data-ttu-id="f7eec-150">Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f7eec-150">The following is an example of the response which includes the requested non-default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_non_default"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
