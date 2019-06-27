---
title: Вывод группы
description: Получение свойств и связей объекта group.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: de58610c8a33e0dee9303a2637d815c2186b95bd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263240"
---
# <a name="get-group"></a><span data-ttu-id="af826-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="af826-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af826-104">Получение свойств и связей объекта [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="af826-104">Get the properties and relationships of a [group](../resources/group.md) object.</span></span> 

<span data-ttu-id="af826-105">Это действие по умолчанию возвращает только подмножество всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="af826-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="af826-106">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="af826-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="af826-107">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="af826-107">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span> <span data-ttu-id="af826-108">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете также получить настраиваемые свойства и данные расширения в экземпляре **group**.</span><span class="sxs-lookup"><span data-stu-id="af826-108">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="af826-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af826-109">Permissions</span></span>
<span data-ttu-id="af826-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af826-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af826-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af826-112">Permission type</span></span>      | <span data-ttu-id="af826-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af826-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af826-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af826-114">Delegated (work or school account)</span></span> | <span data-ttu-id="af826-115">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af826-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="af826-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af826-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af826-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af826-117">Not supported.</span></span>    |
|<span data-ttu-id="af826-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af826-118">Application</span></span> | <span data-ttu-id="af826-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af826-119">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="af826-120">**Примечание.** В зависимости от функций группы, к которым вы пытаетесь получить доступ, разрешения могут быть ограничены.</span><span class="sxs-lookup"><span data-stu-id="af826-120">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="af826-121">Дополнительные сведения см. в разделе [Группы](/graph/known-issues#groups) статьи [Известные проблемы с Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="af826-121">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="af826-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af826-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="af826-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="af826-123">Optional query parameters</span></span>
<span data-ttu-id="af826-124">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af826-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="af826-125">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="af826-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="af826-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af826-126">Request headers</span></span>
| <span data-ttu-id="af826-127">Имя</span><span class="sxs-lookup"><span data-stu-id="af826-127">Name</span></span>       | <span data-ttu-id="af826-128">Тип</span><span class="sxs-lookup"><span data-stu-id="af826-128">Type</span></span> | <span data-ttu-id="af826-129">Описание</span><span class="sxs-lookup"><span data-stu-id="af826-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af826-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="af826-130">Authorization</span></span>  | <span data-ttu-id="af826-131">string</span><span class="sxs-lookup"><span data-stu-id="af826-131">string</span></span>  | <span data-ttu-id="af826-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af826-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af826-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af826-134">Request body</span></span>
<span data-ttu-id="af826-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af826-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af826-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="af826-136">Response</span></span>
<span data-ttu-id="af826-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af826-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="af826-138">Он возвращает параметры по умолчанию, если не используется параметр `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="af826-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="af826-139">Пример</span><span class="sxs-lookup"><span data-stu-id="af826-139">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="af826-140">Пример 1. Возвращение всех свойств по умолчанию</span><span class="sxs-lookup"><span data-stu-id="af826-140">Example 1: Return all default properties</span></span>

#### <a name="request"></a><span data-ttu-id="af826-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="af826-141">Request</span></span>

<span data-ttu-id="af826-142">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="af826-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response"></a><span data-ttu-id="af826-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="af826-143">Response</span></span>
<span data-ttu-id="af826-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="af826-144">The following is an example of the response.</span></span> <span data-ttu-id="af826-145">Он включает только стандартные свойства.</span><span class="sxs-lookup"><span data-stu-id="af826-145">It includes only the default properties.</span></span>

><span data-ttu-id="af826-146">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af826-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="af826-147">В реальном вызове возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af826-147">All the default properties are returned in an actual call.</span></span>
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

#### <a name="sdk-sample-code"></a><span data-ttu-id="af826-148">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="af826-148">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="af826-149">C#</span><span class="sxs-lookup"><span data-stu-id="af826-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af826-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af826-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="af826-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af826-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="af826-152">Пример 2. Возвращение дополнительных свойств с помощью параметра $select</span><span class="sxs-lookup"><span data-stu-id="af826-152">Example 2: Return additional properties by using $select</span></span>

#### <a name="request"></a><span data-ttu-id="af826-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="af826-153">Request</span></span>

<span data-ttu-id="af826-154">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="af826-154">The following is an example of a GET request.</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response"></a><span data-ttu-id="af826-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="af826-155">Response</span></span>

<span data-ttu-id="af826-156">Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="af826-156">The following is an example of the response which includes the requested non-default properties.</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="af826-157">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="af826-157">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="af826-158">C#</span><span class="sxs-lookup"><span data-stu-id="af826-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_non_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af826-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af826-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_non_default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="af826-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af826-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_non_default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="af826-161">См. также</span><span class="sxs-lookup"><span data-stu-id="af826-161">See also</span></span>

- [<span data-ttu-id="af826-162">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="af826-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="af826-163">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="af826-163">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="af826-164">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="af826-164">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
