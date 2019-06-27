---
title: Создание группы
description: Создание группы Office 365 или группы безопасности.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 918e1b40ff45b92b44d3e18970f232cd318a2865
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262946"
---
# <a name="create-group"></a><span data-ttu-id="f38a3-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="f38a3-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f38a3-104">Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="f38a3-104">Create a new [channel](../resources/group.md) in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="f38a3-105">Можно создать одну из следующих групп:</span><span class="sxs-lookup"><span data-stu-id="f38a3-105">You can choose one of the following options:</span></span>

* <span data-ttu-id="f38a3-106">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="f38a3-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="f38a3-107">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="f38a3-107">Security group</span></span>

<span data-ttu-id="f38a3-108">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="f38a3-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="f38a3-109">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="f38a3-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="f38a3-110">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="f38a3-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="f38a3-111">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="f38a3-111">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f38a3-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f38a3-112">Permissions</span></span>
<span data-ttu-id="f38a3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f38a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f38a3-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f38a3-115">Permission type</span></span>      | <span data-ttu-id="f38a3-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f38a3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f38a3-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f38a3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f38a3-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f38a3-118">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="f38a3-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f38a3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f38a3-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f38a3-120">Not supported.</span></span>    |
|<span data-ttu-id="f38a3-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f38a3-121">Application</span></span> | <span data-ttu-id="f38a3-122">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f38a3-122">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f38a3-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f38a3-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="f38a3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f38a3-124">Request headers</span></span>

| <span data-ttu-id="f38a3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f38a3-125">Name</span></span>       | <span data-ttu-id="f38a3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="f38a3-126">Type</span></span> | <span data-ttu-id="f38a3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="f38a3-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f38a3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f38a3-128">Authorization</span></span>  | <span data-ttu-id="f38a3-129">string</span><span class="sxs-lookup"><span data-stu-id="f38a3-129">string</span></span>  | <span data-ttu-id="f38a3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f38a3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f38a3-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f38a3-132">Request body</span></span>

<span data-ttu-id="f38a3-133">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="f38a3-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="f38a3-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="f38a3-134">Property</span></span> | <span data-ttu-id="f38a3-135">Тип</span><span class="sxs-lookup"><span data-stu-id="f38a3-135">Type</span></span> | <span data-ttu-id="f38a3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f38a3-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f38a3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f38a3-137">displayName</span></span> | <span data-ttu-id="f38a3-138">string</span><span class="sxs-lookup"><span data-stu-id="f38a3-138">string</span></span> | <span data-ttu-id="f38a3-139">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="f38a3-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="f38a3-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f38a3-140">Required.</span></span> |
| <span data-ttu-id="f38a3-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="f38a3-141">mailEnabled</span></span> | <span data-ttu-id="f38a3-142">boolean</span><span class="sxs-lookup"><span data-stu-id="f38a3-142">boolean</span></span> | <span data-ttu-id="f38a3-143">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="f38a3-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="f38a3-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f38a3-144">Required.</span></span> |
| <span data-ttu-id="f38a3-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f38a3-145">mailNickname</span></span> | <span data-ttu-id="f38a3-146">string</span><span class="sxs-lookup"><span data-stu-id="f38a3-146">string</span></span> | <span data-ttu-id="f38a3-147">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="f38a3-147">The mail alias for the group.</span></span> <span data-ttu-id="f38a3-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f38a3-148">Required.</span></span> |
| <span data-ttu-id="f38a3-149">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="f38a3-149">securityEnabled</span></span> | <span data-ttu-id="f38a3-150">boolean</span><span class="sxs-lookup"><span data-stu-id="f38a3-150">boolean</span></span> | <span data-ttu-id="f38a3-151">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="f38a3-151">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="f38a3-152">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f38a3-152">Required.</span></span> |
| <span data-ttu-id="f38a3-153">owners</span><span class="sxs-lookup"><span data-stu-id="f38a3-153">owners</span></span> | <span data-ttu-id="f38a3-154">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="f38a3-154">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="f38a3-155">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="f38a3-155">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="f38a3-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f38a3-156">Optional.</span></span> |
| <span data-ttu-id="f38a3-157">members</span><span class="sxs-lookup"><span data-stu-id="f38a3-157">members</span></span> | <span data-ttu-id="f38a3-158">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="f38a3-158">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="f38a3-159">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="f38a3-159">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="f38a3-160">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f38a3-160">Optional.</span></span> |

> <span data-ttu-id="f38a3-161">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="f38a3-161">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="f38a3-162">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="f38a3-162">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="f38a3-163">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="f38a3-163">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="f38a3-164">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="f38a3-164">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="f38a3-p112">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="f38a3-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="f38a3-167">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="f38a3-167">groupTypes options</span></span>

<span data-ttu-id="f38a3-168">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="f38a3-168">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="f38a3-169">Тип группы</span><span class="sxs-lookup"><span data-stu-id="f38a3-169">Type of group</span></span> | <span data-ttu-id="f38a3-170">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="f38a3-170">Assigned membership</span></span> | <span data-ttu-id="f38a3-171">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="f38a3-171">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="f38a3-172">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="f38a3-172">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="f38a3-173">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="f38a3-173">Dynamic</span></span> | <span data-ttu-id="f38a3-174">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="f38a3-174">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="f38a3-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="f38a3-175">Response</span></span>

<span data-ttu-id="f38a3-176">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f38a3-176">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="f38a3-177">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="f38a3-177">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="f38a3-178">Примеры</span><span class="sxs-lookup"><span data-stu-id="f38a3-178">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="f38a3-179">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="f38a3-179">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="f38a3-180">В следующем примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="f38a3-180">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="f38a3-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="f38a3-181">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f38a3-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="f38a3-182">Response</span></span>

<span data-ttu-id="f38a3-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f38a3-183">The following is an example of the response.</span></span>

><span data-ttu-id="f38a3-184">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f38a3-184">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f38a3-185">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f38a3-185">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f38a3-186">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f38a3-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f38a3-187">C#</span><span class="sxs-lookup"><span data-stu-id="f38a3-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f38a3-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f38a3-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f38a3-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f38a3-189">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="f38a3-190">Пример 2. Создание группы Office 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="f38a3-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="f38a3-191">В следующем примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="f38a3-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="f38a3-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="f38a3-192">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f38a3-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="f38a3-193">Response</span></span> 

<span data-ttu-id="f38a3-194">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="f38a3-194">The following is an example of a successful response.</span></span> <span data-ttu-id="f38a3-195">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f38a3-195">It includes only default properties.</span></span> <span data-ttu-id="f38a3-196">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="f38a3-196">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="f38a3-197">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f38a3-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f38a3-198">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f38a3-198">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f38a3-199">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f38a3-199">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f38a3-200">C#</span><span class="sxs-lookup"><span data-stu-id="f38a3-200">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f38a3-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f38a3-201">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f38a3-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f38a3-202">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="f38a3-203">См. также</span><span class="sxs-lookup"><span data-stu-id="f38a3-203">See also</span></span>

- [<span data-ttu-id="f38a3-204">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="f38a3-204">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f38a3-205">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f38a3-205">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f38a3-206">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f38a3-206">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
