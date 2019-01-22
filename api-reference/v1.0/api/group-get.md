---
title: Вывод группы
description: Получение свойств и связей объекта группы.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 92b9c8de30f0070491d84acf9cfc56225c1a7981
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353092"
---
# <a name="get-group"></a><span data-ttu-id="5669f-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="5669f-103">Get group</span></span>
<span data-ttu-id="5669f-104">Получение свойств и связей объекта группы.</span><span class="sxs-lookup"><span data-stu-id="5669f-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="5669f-105">Это действие по умолчанию возвращает только часть всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="5669f-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="5669f-106">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="5669f-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="5669f-107">См. [пример](#request-2).</span><span class="sxs-lookup"><span data-stu-id="5669f-107">See an [example](#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="5669f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5669f-108">Permissions</span></span>
<span data-ttu-id="5669f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5669f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5669f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5669f-111">Permission type</span></span>      | <span data-ttu-id="5669f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5669f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5669f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5669f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5669f-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5669f-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5669f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5669f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5669f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5669f-116">Not supported.</span></span>    |
|<span data-ttu-id="5669f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5669f-117">Application</span></span> | <span data-ttu-id="5669f-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5669f-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5669f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5669f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5669f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5669f-120">Optional query parameters</span></span>
<span data-ttu-id="5669f-121">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5669f-121">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="5669f-122">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="5669f-122">See an [example](#request-2).</span></span>

<span data-ttu-id="5669f-123">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5669f-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5669f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5669f-124">Request headers</span></span>
| <span data-ttu-id="5669f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="5669f-125">Name</span></span>       | <span data-ttu-id="5669f-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5669f-126">Type</span></span> | <span data-ttu-id="5669f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5669f-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5669f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5669f-128">Authorization</span></span>  | <span data-ttu-id="5669f-129">string</span><span class="sxs-lookup"><span data-stu-id="5669f-129">string</span></span>  | <span data-ttu-id="5669f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5669f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5669f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5669f-132">Request body</span></span>
<span data-ttu-id="5669f-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5669f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5669f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5669f-134">Response</span></span>
<span data-ttu-id="5669f-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5669f-135">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="5669f-136">Он возвращает параметры по умолчанию, если не используется параметр `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="5669f-136">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="5669f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5669f-137">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="5669f-138">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="5669f-138">Request 1</span></span>
<span data-ttu-id="5669f-139">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="5669f-139">The following is an example of the GET request with sample query string values.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="5669f-140">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="5669f-140">Response 1</span></span>
<span data-ttu-id="5669f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5669f-141">The following is an example of the response.</span></span> <span data-ttu-id="5669f-142">Он включает только стандартные свойства.</span><span class="sxs-lookup"><span data-stu-id="5669f-142">It includes only the default properties.</span></span>

><span data-ttu-id="5669f-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5669f-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5669f-144">В реальном вызове возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5669f-144">All the default properties are returned in an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="5669f-145">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="5669f-145">Request 2</span></span>
<span data-ttu-id="5669f-146">В следующем примере используется параметр запрос `$select`, чтобы получить несколько свойств, которые не найдены по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5669f-146">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="5669f-147">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="5669f-147">Response 2</span></span>
<span data-ttu-id="5669f-148">Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5669f-148">The following is an example of the response which includes the requested non-default properties.</span></span>

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
