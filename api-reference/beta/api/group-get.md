---
title: Вывод группы
description: Получение свойств и связей объекта group.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 9ac99ad0e31a355ea81c47a313d3440c985753a1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593167"
---
# <a name="get-group"></a><span data-ttu-id="3cb22-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="3cb22-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb22-104">Получение свойств и связей объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="3cb22-104">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

<span data-ttu-id="3cb22-105">Это действие по умолчанию возвращает только подмножество всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="3cb22-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="3cb22-106">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="3cb22-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="3cb22-107">См. [пример](#request-2) для `$select`.</span><span class="sxs-lookup"><span data-stu-id="3cb22-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="3cb22-108">Исключением является свойство **hasMembersWithLicenseErrors**.</span><span class="sxs-lookup"><span data-stu-id="3cb22-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="3cb22-109">См. [пример](group-list.md#request-2) использования этого свойства.</span><span class="sxs-lookup"><span data-stu-id="3cb22-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="3cb22-110">Так как ресурс **группы** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете также получить настраиваемые свойства и данные расширения в экземпляре **группы**.</span><span class="sxs-lookup"><span data-stu-id="3cb22-110">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb22-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb22-111">Permissions</span></span>
<span data-ttu-id="3cb22-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cb22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cb22-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb22-114">Permission type</span></span>      | <span data-ttu-id="3cb22-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cb22-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cb22-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cb22-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3cb22-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb22-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3cb22-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cb22-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cb22-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb22-119">Not supported.</span></span>    |
|<span data-ttu-id="3cb22-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cb22-120">Application</span></span> | <span data-ttu-id="3cb22-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb22-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cb22-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cb22-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3cb22-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3cb22-123">Optional query parameters</span></span>
<span data-ttu-id="3cb22-124">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3cb22-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="3cb22-125">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="3cb22-125">See an [example](#request-2) below.</span></span>

<span data-ttu-id="3cb22-126">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3cb22-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cb22-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cb22-127">Request headers</span></span>
| <span data-ttu-id="3cb22-128">Имя</span><span class="sxs-lookup"><span data-stu-id="3cb22-128">Name</span></span>       | <span data-ttu-id="3cb22-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb22-129">Type</span></span> | <span data-ttu-id="3cb22-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb22-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3cb22-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cb22-131">Authorization</span></span>  | <span data-ttu-id="3cb22-132">string</span><span class="sxs-lookup"><span data-stu-id="3cb22-132">string</span></span>  | <span data-ttu-id="3cb22-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cb22-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cb22-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cb22-135">Request body</span></span>
<span data-ttu-id="3cb22-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cb22-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb22-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cb22-137">Response</span></span>
<span data-ttu-id="3cb22-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cb22-138">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="3cb22-139">Он возвращает параметры по умолчанию, если не используется параметр `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="3cb22-139">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="3cb22-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3cb22-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="3cb22-141">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="3cb22-141">Request 1</span></span>
<span data-ttu-id="3cb22-142">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="3cb22-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="3cb22-143">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="3cb22-143">Response 1</span></span>
<span data-ttu-id="3cb22-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3cb22-144">The following is an example of the response.</span></span> <span data-ttu-id="3cb22-145">Он включает только стандартные свойства.</span><span class="sxs-lookup"><span data-stu-id="3cb22-145">It includes only the default properties.</span></span>

><span data-ttu-id="3cb22-146">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3cb22-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3cb22-147">В реальном вызове возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3cb22-147">All the default properties are returned in an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3cb22-148">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="3cb22-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3cb22-149">C#</span><span class="sxs-lookup"><span data-stu-id="3cb22-149">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cb22-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cb22-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="3cb22-151">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="3cb22-151">Request 2</span></span>
<span data-ttu-id="3cb22-152">В следующем примере используется параметр запрос `$select`, чтобы получить несколько свойств, которые не найдены по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3cb22-152">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="3cb22-153">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="3cb22-153">Response 2</span></span>
<span data-ttu-id="3cb22-154">Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3cb22-154">The following is an example of the response which includes the requested non-default properties.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3cb22-155">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="3cb22-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3cb22-156">C#</span><span class="sxs-lookup"><span data-stu-id="3cb22-156">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_non_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cb22-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cb22-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_non_default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="3cb22-158">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="3cb22-158">See also</span></span>

- [<span data-ttu-id="3cb22-159">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="3cb22-159">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3cb22-160">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="3cb22-160">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3cb22-161">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="3cb22-161">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
