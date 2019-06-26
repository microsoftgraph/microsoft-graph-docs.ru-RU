---
title: Вывод группы
description: Получение свойств и связей объекта group.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 3d3ac3542593ef25bd309a2277903794b5a69fbd
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236491"
---
# <a name="get-group"></a><span data-ttu-id="dd7a1-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="dd7a1-103">Get group</span></span>

<span data-ttu-id="dd7a1-104">Получение свойств и связей объекта группы.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="dd7a1-105">Это действие по умолчанию возвращает только часть всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="dd7a1-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="dd7a1-106">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="dd7a1-107">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-107">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd7a1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd7a1-108">Permissions</span></span>
<span data-ttu-id="dd7a1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd7a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd7a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd7a1-111">Permission type</span></span>      | <span data-ttu-id="dd7a1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd7a1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd7a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd7a1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dd7a1-114">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd7a1-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="dd7a1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd7a1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd7a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-116">Not supported.</span></span>    |
|<span data-ttu-id="dd7a1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd7a1-117">Application</span></span> | <span data-ttu-id="dd7a1-118">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd7a1-118">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="dd7a1-119">**Примечание.** В зависимости от функций группы, к которым вы пытаетесь получить доступ, разрешения могут быть ограничены.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-119">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="dd7a1-120">Дополнительные сведения см. в разделе [Группы](/graph/known-issues#groups) статьи [Известные проблемы с Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="dd7a1-120">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="dd7a1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd7a1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd7a1-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd7a1-122">Optional query parameters</span></span>
<span data-ttu-id="dd7a1-123">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="dd7a1-124">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dd7a1-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd7a1-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd7a1-125">Request headers</span></span>
| <span data-ttu-id="dd7a1-126">Имя</span><span class="sxs-lookup"><span data-stu-id="dd7a1-126">Name</span></span>       | <span data-ttu-id="dd7a1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="dd7a1-127">Type</span></span> | <span data-ttu-id="dd7a1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dd7a1-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dd7a1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd7a1-129">Authorization</span></span>  | <span data-ttu-id="dd7a1-130">string</span><span class="sxs-lookup"><span data-stu-id="dd7a1-130">string</span></span>  | <span data-ttu-id="dd7a1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd7a1-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd7a1-133">Request body</span></span>
<span data-ttu-id="dd7a1-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd7a1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd7a1-135">Response</span></span>
<span data-ttu-id="dd7a1-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-136">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="dd7a1-137">Он возвращает параметры по умолчанию, если не используется параметр `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-137">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="dd7a1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="dd7a1-138">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="dd7a1-139">Пример 1. Возвращение всех свойств по умолчанию</span><span class="sxs-lookup"><span data-stu-id="dd7a1-139">Example 1: Return all default properties</span></span>

<span data-ttu-id="dd7a1-140">Возвращение всех свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-140">Return all default properties.</span></span>

#### <a name="request"></a><span data-ttu-id="dd7a1-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7a1-141">Request</span></span> 

<span data-ttu-id="dd7a1-142">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response"></a><span data-ttu-id="dd7a1-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7a1-143">Response</span></span>
<span data-ttu-id="dd7a1-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-144">The following is an example of the response.</span></span> <span data-ttu-id="dd7a1-145">Он включает только стандартные свойства.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-145">It includes only the default properties.</span></span>

><span data-ttu-id="dd7a1-146">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dd7a1-147">В реальном вызове возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-147">All the default properties are returned in an actual call.</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="dd7a1-148">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="dd7a1-148">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="dd7a1-149">C#</span><span class="sxs-lookup"><span data-stu-id="dd7a1-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd7a1-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd7a1-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="dd7a1-151">Пример 2. Возвращение дополнительных свойств с помощью параметра $select</span><span class="sxs-lookup"><span data-stu-id="dd7a1-151">Example 2: Return additional properties by using $select</span></span>

<span data-ttu-id="dd7a1-152">Возвращение дополнительных свойств с помощью параметра `$select`.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-152">Return additional properties by using `$select`.</span></span>

#### <a name="request"></a><span data-ttu-id="dd7a1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd7a1-153">Request</span></span>

<span data-ttu-id="dd7a1-154">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-154">The following is an example of a GET request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response"></a><span data-ttu-id="dd7a1-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd7a1-155">Response</span></span>

<span data-ttu-id="dd7a1-156">Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dd7a1-156">The following is an example of the response which includes the requested non-default properties.</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="dd7a1-157">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="dd7a1-157">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="dd7a1-158">C#</span><span class="sxs-lookup"><span data-stu-id="dd7a1-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_non_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd7a1-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd7a1-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_non_default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
