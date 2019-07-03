---
title: Создание группы
description: Создание группы Office 365 или группы безопасности.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: cee571584f37feece435892caef0b0c648d13184
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440283"
---
# <a name="create-group"></a><span data-ttu-id="031ac-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="031ac-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="031ac-104">Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="031ac-104">Create a new [channel](../resources/group.md) in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="031ac-105">Можно создать одну из следующих групп:</span><span class="sxs-lookup"><span data-stu-id="031ac-105">You can choose one of the following options:</span></span>

* <span data-ttu-id="031ac-106">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="031ac-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="031ac-107">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="031ac-107">Security group</span></span>

<span data-ttu-id="031ac-108">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="031ac-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="031ac-109">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="031ac-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="031ac-110">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="031ac-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="031ac-111">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="031ac-111">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="031ac-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="031ac-112">Permissions</span></span>
<span data-ttu-id="031ac-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="031ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="031ac-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="031ac-115">Permission type</span></span>      | <span data-ttu-id="031ac-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="031ac-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="031ac-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="031ac-117">Delegated (work or school account)</span></span> | <span data-ttu-id="031ac-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="031ac-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="031ac-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="031ac-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="031ac-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="031ac-120">Not supported.</span></span>    |
|<span data-ttu-id="031ac-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="031ac-121">Application</span></span> | <span data-ttu-id="031ac-122">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="031ac-122">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="031ac-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="031ac-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="031ac-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="031ac-124">Request headers</span></span>

| <span data-ttu-id="031ac-125">Имя</span><span class="sxs-lookup"><span data-stu-id="031ac-125">Name</span></span>       | <span data-ttu-id="031ac-126">Тип</span><span class="sxs-lookup"><span data-stu-id="031ac-126">Type</span></span> | <span data-ttu-id="031ac-127">Описание</span><span class="sxs-lookup"><span data-stu-id="031ac-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="031ac-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="031ac-128">Authorization</span></span>  | <span data-ttu-id="031ac-129">string</span><span class="sxs-lookup"><span data-stu-id="031ac-129">string</span></span>  | <span data-ttu-id="031ac-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="031ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="031ac-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="031ac-132">Request body</span></span>

<span data-ttu-id="031ac-133">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="031ac-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="031ac-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="031ac-134">Property</span></span> | <span data-ttu-id="031ac-135">Тип</span><span class="sxs-lookup"><span data-stu-id="031ac-135">Type</span></span> | <span data-ttu-id="031ac-136">Описание</span><span class="sxs-lookup"><span data-stu-id="031ac-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="031ac-137">displayName</span><span class="sxs-lookup"><span data-stu-id="031ac-137">displayName</span></span> | <span data-ttu-id="031ac-138">string</span><span class="sxs-lookup"><span data-stu-id="031ac-138">string</span></span> | <span data-ttu-id="031ac-139">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="031ac-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="031ac-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="031ac-140">Required.</span></span> |
| <span data-ttu-id="031ac-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="031ac-141">mailEnabled</span></span> | <span data-ttu-id="031ac-142">boolean</span><span class="sxs-lookup"><span data-stu-id="031ac-142">boolean</span></span> | <span data-ttu-id="031ac-143">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="031ac-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="031ac-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="031ac-144">Required.</span></span> |
| <span data-ttu-id="031ac-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="031ac-145">mailNickname</span></span> | <span data-ttu-id="031ac-146">string</span><span class="sxs-lookup"><span data-stu-id="031ac-146">string</span></span> | <span data-ttu-id="031ac-147">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="031ac-147">The mail alias for the group.</span></span> <span data-ttu-id="031ac-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="031ac-148">Required.</span></span> |
| <span data-ttu-id="031ac-149">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="031ac-149">securityEnabled</span></span> | <span data-ttu-id="031ac-150">boolean</span><span class="sxs-lookup"><span data-stu-id="031ac-150">boolean</span></span> | <span data-ttu-id="031ac-151">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="031ac-151">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="031ac-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="031ac-152">Required.</span></span> |
| <span data-ttu-id="031ac-153">owners</span><span class="sxs-lookup"><span data-stu-id="031ac-153">owners</span></span> | <span data-ttu-id="031ac-154">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="031ac-154">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="031ac-155">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="031ac-155">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="031ac-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="031ac-156">Optional.</span></span> |
| <span data-ttu-id="031ac-157">members</span><span class="sxs-lookup"><span data-stu-id="031ac-157">members</span></span> | <span data-ttu-id="031ac-158">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="031ac-158">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="031ac-159">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="031ac-159">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="031ac-160">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="031ac-160">Optional.</span></span> |

> <span data-ttu-id="031ac-161">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="031ac-161">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="031ac-162">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="031ac-162">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="031ac-163">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="031ac-163">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="031ac-164">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="031ac-164">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="031ac-p112">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="031ac-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="031ac-167">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="031ac-167">groupTypes options</span></span>

<span data-ttu-id="031ac-168">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="031ac-168">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="031ac-169">Тип группы</span><span class="sxs-lookup"><span data-stu-id="031ac-169">Type of group</span></span> | <span data-ttu-id="031ac-170">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="031ac-170">Assigned membership</span></span> | <span data-ttu-id="031ac-171">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="031ac-171">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="031ac-172">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="031ac-172">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="031ac-173">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="031ac-173">Dynamic</span></span> | <span data-ttu-id="031ac-174">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="031ac-174">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="031ac-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="031ac-175">Response</span></span>

<span data-ttu-id="031ac-176">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="031ac-176">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="031ac-177">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="031ac-177">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="031ac-178">Примеры</span><span class="sxs-lookup"><span data-stu-id="031ac-178">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="031ac-179">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="031ac-179">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="031ac-180">В следующем примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="031ac-180">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="031ac-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="031ac-181">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="031ac-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="031ac-182">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="031ac-183">C#</span><span class="sxs-lookup"><span data-stu-id="031ac-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="031ac-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="031ac-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="031ac-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="031ac-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="031ac-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="031ac-186">Response</span></span>

<span data-ttu-id="031ac-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="031ac-187">The following is an example of the response.</span></span>

><span data-ttu-id="031ac-188">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="031ac-188">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="031ac-189">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="031ac-189">All the default properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
``` http
HTTP/1.1 201 Created
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
         "SMTP:golfassist@contoso.onmicrosoft.com"
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

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="031ac-190">Пример 2. Создание группы Office 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="031ac-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="031ac-191">В следующем примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="031ac-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="031ac-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="031ac-192">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="031ac-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="031ac-193">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="031ac-194">C#</span><span class="sxs-lookup"><span data-stu-id="031ac-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="031ac-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="031ac-195">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="031ac-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="031ac-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="031ac-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="031ac-197">Response</span></span> 

<span data-ttu-id="031ac-198">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="031ac-198">The following is an example of a successful response.</span></span> <span data-ttu-id="031ac-199">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="031ac-199">It includes only default properties.</span></span> <span data-ttu-id="031ac-200">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="031ac-200">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="031ac-201">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="031ac-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="031ac-202">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="031ac-202">All the default properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "502df398-d59c-469d-944f-34a50e60db3f",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-27T22:17:07Z",
    "creationOptions": [],
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "groupTypes": [
        "Unified"
    ],
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "SMTP:operations2019@contoso.com"
    ],
    "renewedDateTime": "2018-12-27T22:17:07Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="031ac-203">См. также</span><span class="sxs-lookup"><span data-stu-id="031ac-203">See also</span></span>

- [<span data-ttu-id="031ac-204">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="031ac-204">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="031ac-205">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="031ac-205">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="031ac-206">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="031ac-206">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
