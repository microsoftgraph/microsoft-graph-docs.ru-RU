---
title: Создание группы
description: Создание группы Office 365 или группы безопасности.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: e33a1fbfe4ff3c48fe80e71e9a066f8d59e31208
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812539"
---
# <a name="create-group"></a><span data-ttu-id="4a942-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="4a942-103">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a942-104">Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="4a942-104">Create a new [channel](../resources/group.md) in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="4a942-105">Можно создать одну из следующих групп:</span><span class="sxs-lookup"><span data-stu-id="4a942-105">You can choose one of the following options:</span></span>

* <span data-ttu-id="4a942-106">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="4a942-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="4a942-107">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="4a942-107">Security group</span></span>

<span data-ttu-id="4a942-108">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="4a942-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="4a942-109">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="4a942-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="4a942-110">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="4a942-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="4a942-111">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="4a942-111">See an [example](group-get.md#request-2).</span></span>

><span data-ttu-id="4a942-112">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="4a942-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a942-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a942-113">Permissions</span></span>
<span data-ttu-id="4a942-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a942-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a942-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a942-116">Permission type</span></span>      | <span data-ttu-id="4a942-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a942-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a942-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a942-118">Delegated (work or school account)</span></span> | <span data-ttu-id="4a942-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a942-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="4a942-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a942-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a942-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a942-121">Not supported.</span></span>    |
|<span data-ttu-id="4a942-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a942-122">Application</span></span> | <span data-ttu-id="4a942-123">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a942-123">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a942-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a942-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="4a942-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a942-125">Request headers</span></span>

| <span data-ttu-id="4a942-126">Имя</span><span class="sxs-lookup"><span data-stu-id="4a942-126">Name</span></span>       | <span data-ttu-id="4a942-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4a942-127">Type</span></span> | <span data-ttu-id="4a942-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4a942-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a942-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a942-129">Authorization</span></span>  | <span data-ttu-id="4a942-130">string</span><span class="sxs-lookup"><span data-stu-id="4a942-130">string</span></span>  | <span data-ttu-id="4a942-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a942-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a942-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a942-133">Request body</span></span>

<span data-ttu-id="4a942-134">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="4a942-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="4a942-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a942-135">Property</span></span> | <span data-ttu-id="4a942-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4a942-136">Type</span></span> | <span data-ttu-id="4a942-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4a942-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4a942-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4a942-138">displayName</span></span> | <span data-ttu-id="4a942-139">string</span><span class="sxs-lookup"><span data-stu-id="4a942-139">string</span></span> | <span data-ttu-id="4a942-140">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="4a942-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="4a942-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a942-141">Required.</span></span> |
| <span data-ttu-id="4a942-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4a942-142">mailEnabled</span></span> | <span data-ttu-id="4a942-143">boolean</span><span class="sxs-lookup"><span data-stu-id="4a942-143">boolean</span></span> | <span data-ttu-id="4a942-144">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="4a942-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="4a942-145">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4a942-145">Required.</span></span> |
| <span data-ttu-id="4a942-146">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4a942-146">mailNickname</span></span> | <span data-ttu-id="4a942-147">string</span><span class="sxs-lookup"><span data-stu-id="4a942-147">string</span></span> | <span data-ttu-id="4a942-148">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="4a942-148">The mail alias for the group.</span></span> <span data-ttu-id="4a942-149">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a942-149">Required.</span></span> |
| <span data-ttu-id="4a942-150">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4a942-150">securityEnabled</span></span> | <span data-ttu-id="4a942-151">boolean</span><span class="sxs-lookup"><span data-stu-id="4a942-151">boolean</span></span> | <span data-ttu-id="4a942-152">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a942-152">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="4a942-153">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4a942-153">Required.</span></span> |
| <span data-ttu-id="4a942-154">owners</span><span class="sxs-lookup"><span data-stu-id="4a942-154">owners</span></span> | <span data-ttu-id="4a942-155">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4a942-155">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="4a942-156">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="4a942-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="4a942-157">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a942-157">Optional.</span></span> |
| <span data-ttu-id="4a942-158">members</span><span class="sxs-lookup"><span data-stu-id="4a942-158">members</span></span> | <span data-ttu-id="4a942-159">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4a942-159">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="4a942-160">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="4a942-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="4a942-161">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a942-161">Optional.</span></span> |

> <span data-ttu-id="4a942-162">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="4a942-162">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="4a942-163">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="4a942-163">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="4a942-164">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="4a942-164">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="4a942-165">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="4a942-165">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="4a942-p113">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="4a942-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="4a942-168">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="4a942-168">groupTypes options</span></span>

<span data-ttu-id="4a942-169">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="4a942-169">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="4a942-170">Тип группы</span><span class="sxs-lookup"><span data-stu-id="4a942-170">Type of group</span></span> | <span data-ttu-id="4a942-171">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="4a942-171">Assigned membership</span></span> | <span data-ttu-id="4a942-172">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="4a942-172">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="4a942-173">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="4a942-173">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="4a942-174">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="4a942-174">Dynamic</span></span> | <span data-ttu-id="4a942-175">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="4a942-175">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="4a942-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a942-176">Response</span></span>

<span data-ttu-id="4a942-177">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4a942-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="4a942-178">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="4a942-178">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="4a942-179">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a942-179">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="4a942-180">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="4a942-180">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="4a942-181">В следующем примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a942-181">The first example request creates an Office 365 Group.</span></span>

#### <a name="request"></a><span data-ttu-id="4a942-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a942-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4a942-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a942-183">Response</span></span>

<span data-ttu-id="4a942-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a942-184">The following is an example of the response.</span></span>

><span data-ttu-id="4a942-185">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a942-185">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a942-186">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a942-186">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a942-187">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4a942-187">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a942-188">C#</span><span class="sxs-lookup"><span data-stu-id="4a942-188">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a942-189">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a942-189">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="4a942-190">Пример 2. Создание группы Office 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="4a942-190">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="4a942-191">В следующем примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="4a942-191">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="4a942-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a942-192">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="4a942-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a942-193">Response</span></span> 

<span data-ttu-id="4a942-194">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="4a942-194">The following is an example of a successful response.</span></span> <span data-ttu-id="4a942-195">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a942-195">It includes only default properties.</span></span> <span data-ttu-id="4a942-196">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="4a942-196">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="4a942-197">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a942-197">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a942-198">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a942-198">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4a942-199">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4a942-199">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4a942-200">C#</span><span class="sxs-lookup"><span data-stu-id="4a942-200">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a942-201">Javascript</span><span class="sxs-lookup"><span data-stu-id="4a942-201">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="4a942-202">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="4a942-202">See also</span></span>

- [<span data-ttu-id="4a942-203">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4a942-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4a942-204">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4a942-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4a942-205">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4a942-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
