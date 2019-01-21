---
title: Вывод группы
description: Получение свойств и связей объекта группы.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 51a3f6a8b135c7a898381180c9da2ad22a4d9527
ms.sourcegitcommit: 02a3ae7f3070d38d949158808545003e85ae8fe7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2019
ms.locfileid: "28726591"
---
# <a name="get-group"></a><span data-ttu-id="af0b7-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="af0b7-103">Get group</span></span>

> <span data-ttu-id="af0b7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af0b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af0b7-105">Использование этих API в рабочих приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af0b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af0b7-106">Получение свойств и связей объекта [группы](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="af0b7-106">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="af0b7-107">Это действие по умолчанию возвращает только подмножество всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="af0b7-107">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="af0b7-108">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="af0b7-108">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="af0b7-109">См. [пример](#request-2) для `$select`.</span><span class="sxs-lookup"><span data-stu-id="af0b7-109">See an [example](#request-2) of the `$select` header in use.</span></span> <span data-ttu-id="af0b7-110">Исключением является свойство **hasMembersWithLicenseErrors**.</span><span class="sxs-lookup"><span data-stu-id="af0b7-110">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="af0b7-111">См. [пример](group-list.md#request-2) использования этого свойства.</span><span class="sxs-lookup"><span data-stu-id="af0b7-111">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="af0b7-112">Так как ресурс **группы** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете также получить настраиваемые свойства и данные расширения в экземпляре **группы**.</span><span class="sxs-lookup"><span data-stu-id="af0b7-112">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="af0b7-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af0b7-113">Permissions</span></span>
<span data-ttu-id="af0b7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af0b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af0b7-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af0b7-116">Permission type</span></span>      | <span data-ttu-id="af0b7-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af0b7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af0b7-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af0b7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="af0b7-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af0b7-119">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="af0b7-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af0b7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af0b7-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af0b7-121">Not supported.</span></span>    |
|<span data-ttu-id="af0b7-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af0b7-122">Application</span></span> | <span data-ttu-id="af0b7-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af0b7-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af0b7-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af0b7-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="af0b7-125">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="af0b7-125">Optional query parameters</span></span>
<span data-ttu-id="af0b7-126">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af0b7-126">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="af0b7-127">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="af0b7-127">See an [example](#request-2).</span></span>

<span data-ttu-id="af0b7-128">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="af0b7-128">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="af0b7-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af0b7-129">Request headers</span></span>
| <span data-ttu-id="af0b7-130">Имя</span><span class="sxs-lookup"><span data-stu-id="af0b7-130">Name</span></span>       | <span data-ttu-id="af0b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af0b7-131">Type</span></span> | <span data-ttu-id="af0b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af0b7-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af0b7-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="af0b7-133">Authorization</span></span>  | <span data-ttu-id="af0b7-134">string</span><span class="sxs-lookup"><span data-stu-id="af0b7-134">string</span></span>  | <span data-ttu-id="af0b7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af0b7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af0b7-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af0b7-137">Request body</span></span>
<span data-ttu-id="af0b7-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af0b7-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af0b7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="af0b7-139">Response</span></span>
<span data-ttu-id="af0b7-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af0b7-140">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af0b7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="af0b7-141">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="af0b7-142">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="af0b7-142">Request 1</span></span>
<span data-ttu-id="af0b7-143">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="af0b7-143">The following is an example of the GET request with sample query string values.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="af0b7-144">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="af0b7-144">Response 1</span></span>
<span data-ttu-id="af0b7-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="af0b7-145">The following is an example of the response.</span></span> <span data-ttu-id="af0b7-146">Он включает только стандартные свойства.</span><span class="sxs-lookup"><span data-stu-id="af0b7-146">It includes only the default properties.</span></span>

><span data-ttu-id="af0b7-147">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af0b7-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="af0b7-148">В реальном вызове возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af0b7-148">All the default properties are returned in an actual call.</span></span>
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
}
```

#### <a name="request-2"></a><span data-ttu-id="af0b7-149">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="af0b7-149">Request 2</span></span>
<span data-ttu-id="af0b7-150">В следующем примере используется параметр запрос `$select`, чтобы получить несколько свойств, которые не найдены по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af0b7-150">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="af0b7-151">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="af0b7-151">Response 2</span></span>
<span data-ttu-id="af0b7-152">Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af0b7-152">The following is an example of the response which includes the requested non-default properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

## <a name="see-also"></a><span data-ttu-id="af0b7-153">См. также</span><span class="sxs-lookup"><span data-stu-id="af0b7-153">See also</span></span>

- [<span data-ttu-id="af0b7-154">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="af0b7-154">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="af0b7-155">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="af0b7-155">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="af0b7-156">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="af0b7-156">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
