---
title: Вывод группы
description: Получение свойств и связей объекта group.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a55a019970294039b14e586e791aa1af9fe41cac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517133"
---
# <a name="get-group"></a><span data-ttu-id="8106f-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="8106f-103">Get group</span></span>

<span data-ttu-id="8106f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8106f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8106f-105">Получение свойств и связей объекта group.</span><span class="sxs-lookup"><span data-stu-id="8106f-105">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="8106f-106">Это действие по умолчанию возвращает только часть всех доступных свойств, как указано в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="8106f-106">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="8106f-107">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="8106f-107">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="8106f-108">Свойство **hasMembersWithLicenseErrors** является исключением и не возвращается в запросе `$select`.</span><span class="sxs-lookup"><span data-stu-id="8106f-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="8106f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8106f-109">Permissions</span></span>
<span data-ttu-id="8106f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8106f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8106f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8106f-112">Permission type</span></span>      | <span data-ttu-id="8106f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8106f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8106f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8106f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8106f-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8106f-115">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="8106f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8106f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8106f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8106f-117">Not supported.</span></span>    |
|<span data-ttu-id="8106f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8106f-118">Application</span></span> | <span data-ttu-id="8106f-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8106f-119">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="8106f-120">**Примечание.** В зависимости от функций группы, к которым вы пытаетесь получить доступ, разрешения могут быть ограничены.</span><span class="sxs-lookup"><span data-stu-id="8106f-120">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="8106f-121">Дополнительные сведения см. в разделе [Группы](/graph/known-issues#groups) статьи [Известные проблемы с Microsoft Graph](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="8106f-121">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="8106f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8106f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8106f-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8106f-123">Optional query parameters</span></span>
<span data-ttu-id="8106f-124">Вы можете использовать `$select` для получения свойств определенной группы, включая те, которые не возвращаются по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8106f-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="8106f-125">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8106f-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8106f-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8106f-126">Request headers</span></span>
| <span data-ttu-id="8106f-127">Имя</span><span class="sxs-lookup"><span data-stu-id="8106f-127">Name</span></span>       | <span data-ttu-id="8106f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8106f-128">Type</span></span> | <span data-ttu-id="8106f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8106f-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8106f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8106f-130">Authorization</span></span>  | <span data-ttu-id="8106f-131">string</span><span class="sxs-lookup"><span data-stu-id="8106f-131">string</span></span>  | <span data-ttu-id="8106f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8106f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8106f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8106f-134">Request body</span></span>
<span data-ttu-id="8106f-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8106f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8106f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8106f-136">Response</span></span>
<span data-ttu-id="8106f-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8106f-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="8106f-138">Он возвращает параметры по умолчанию, если не используется параметр `$select` для указания конкретных свойств.</span><span class="sxs-lookup"><span data-stu-id="8106f-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="8106f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8106f-139">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="8106f-140">Пример 1. Возвращение всех свойств по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8106f-140">Example 1: Return all default properties</span></span>

<span data-ttu-id="8106f-141">Возвращение всех свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8106f-141">Return all default properties.</span></span>

#### <a name="request"></a><span data-ttu-id="8106f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8106f-142">Request</span></span> 

<span data-ttu-id="8106f-143">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="8106f-143">The following is an example of a GET request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="8106f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="8106f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```
# <a name="c"></a>[<span data-ttu-id="8106f-145">C#</span><span class="sxs-lookup"><span data-stu-id="8106f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8106f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8106f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8106f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8106f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8106f-148">Java</span><span class="sxs-lookup"><span data-stu-id="8106f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8106f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="8106f-149">Response</span></span>
<span data-ttu-id="8106f-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8106f-150">The following is an example of the response.</span></span> <span data-ttu-id="8106f-151">Он включает только стандартные свойства.</span><span class="sxs-lookup"><span data-stu-id="8106f-151">It includes only the default properties.</span></span>

><span data-ttu-id="8106f-152">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8106f-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8106f-153">В реальном вызове возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8106f-153">All the default properties are returned in an actual call.</span></span>

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


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="8106f-154">Пример 2. Возвращение дополнительных свойств с помощью параметра $select</span><span class="sxs-lookup"><span data-stu-id="8106f-154">Example 2: Return additional properties by using $select</span></span>

<span data-ttu-id="8106f-155">Возвращение дополнительных свойств с помощью параметра `$select`.</span><span class="sxs-lookup"><span data-stu-id="8106f-155">Return additional properties by using `$select`.</span></span>

#### <a name="request"></a><span data-ttu-id="8106f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8106f-156">Request</span></span>

<span data-ttu-id="8106f-157">Ниже приведен пример запроса GET.</span><span class="sxs-lookup"><span data-stu-id="8106f-157">The following is an example of a GET request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8106f-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8106f-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="c"></a>[<span data-ttu-id="8106f-159">C#</span><span class="sxs-lookup"><span data-stu-id="8106f-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8106f-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8106f-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8106f-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8106f-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8106f-162">Java</span><span class="sxs-lookup"><span data-stu-id="8106f-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8106f-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8106f-163">Response</span></span>

<span data-ttu-id="8106f-164">Ниже приведен пример ответа, содержащий запрашиваемые свойства, которые не заданы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8106f-164">The following is an example of the response which includes the requested non-default properties.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
