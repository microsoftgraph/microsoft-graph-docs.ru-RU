---
title: Создание группы
description: Создание группы Office 365 или группы безопасности.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ad934ae8d97d47cef6446def3305d0a6e365597
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418794"
---
# <a name="create-group"></a><span data-ttu-id="ef8be-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="ef8be-103">Create group</span></span>

<span data-ttu-id="ef8be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef8be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef8be-105">Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="ef8be-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="ef8be-106">Можно создать одну из следующих групп:</span><span class="sxs-lookup"><span data-stu-id="ef8be-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="ef8be-107">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="ef8be-107">Office 365 group (unified group)</span></span>
* <span data-ttu-id="ef8be-108">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="ef8be-108">Security group</span></span>

<span data-ttu-id="ef8be-109">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="ef8be-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="ef8be-110">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="ef8be-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="ef8be-111">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="ef8be-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="ef8be-112">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="ef8be-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef8be-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef8be-113">Permissions</span></span>
<span data-ttu-id="ef8be-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef8be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef8be-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef8be-116">Permission type</span></span>      | <span data-ttu-id="ef8be-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef8be-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef8be-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef8be-118">Delegated (work or school account)</span></span> | <span data-ttu-id="ef8be-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ef8be-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="ef8be-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef8be-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef8be-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef8be-121">Not supported.</span></span>    |
|<span data-ttu-id="ef8be-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef8be-122">Application</span></span> | <span data-ttu-id="ef8be-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef8be-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef8be-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef8be-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="ef8be-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef8be-125">Request headers</span></span>

| <span data-ttu-id="ef8be-126">Имя</span><span class="sxs-lookup"><span data-stu-id="ef8be-126">Name</span></span>       | <span data-ttu-id="ef8be-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ef8be-127">Type</span></span> | <span data-ttu-id="ef8be-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ef8be-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ef8be-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef8be-129">Authorization</span></span>  | <span data-ttu-id="ef8be-130">string</span><span class="sxs-lookup"><span data-stu-id="ef8be-130">string</span></span>  | <span data-ttu-id="ef8be-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef8be-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef8be-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef8be-133">Request body</span></span>

<span data-ttu-id="ef8be-134">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="ef8be-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="ef8be-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef8be-135">Property</span></span> | <span data-ttu-id="ef8be-136">Тип</span><span class="sxs-lookup"><span data-stu-id="ef8be-136">Type</span></span> | <span data-ttu-id="ef8be-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ef8be-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ef8be-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ef8be-138">displayName</span></span> | <span data-ttu-id="ef8be-139">string</span><span class="sxs-lookup"><span data-stu-id="ef8be-139">string</span></span> | <span data-ttu-id="ef8be-140">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="ef8be-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="ef8be-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef8be-141">Required.</span></span> |
| <span data-ttu-id="ef8be-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="ef8be-142">mailEnabled</span></span> | <span data-ttu-id="ef8be-143">boolean</span><span class="sxs-lookup"><span data-stu-id="ef8be-143">boolean</span></span> | <span data-ttu-id="ef8be-144">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="ef8be-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="ef8be-145">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ef8be-145">Required.</span></span> |
| <span data-ttu-id="ef8be-146">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ef8be-146">mailNickname</span></span> | <span data-ttu-id="ef8be-147">string</span><span class="sxs-lookup"><span data-stu-id="ef8be-147">string</span></span> | <span data-ttu-id="ef8be-148">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="ef8be-148">The mail alias for the group.</span></span> <span data-ttu-id="ef8be-149">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef8be-149">Required.</span></span> |
| <span data-ttu-id="ef8be-150">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="ef8be-150">securityEnabled</span></span> | <span data-ttu-id="ef8be-151">boolean</span><span class="sxs-lookup"><span data-stu-id="ef8be-151">boolean</span></span> | <span data-ttu-id="ef8be-152">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="ef8be-152">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="ef8be-153">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ef8be-153">Required.</span></span> |
| <span data-ttu-id="ef8be-154">owners</span><span class="sxs-lookup"><span data-stu-id="ef8be-154">owners</span></span> | <span data-ttu-id="ef8be-155">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ef8be-155">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="ef8be-156">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="ef8be-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="ef8be-157">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ef8be-157">Optional.</span></span> |
| <span data-ttu-id="ef8be-158">members</span><span class="sxs-lookup"><span data-stu-id="ef8be-158">members</span></span> | <span data-ttu-id="ef8be-159">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ef8be-159">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="ef8be-160">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="ef8be-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="ef8be-161">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ef8be-161">Optional.</span></span> |

> <span data-ttu-id="ef8be-162">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="ef8be-162">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="ef8be-163">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к группе при ее создании.</span><span class="sxs-lookup"><span data-stu-id="ef8be-163">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="ef8be-164">**Примечание:** создание группы с помощью разрешения приложения Group.Create без указания владельцев анонимно создает группу, которая не будет изменяться.</span><span class="sxs-lookup"><span data-stu-id="ef8be-164">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="ef8be-165">Вы можете использовать операцию `POST` и добавить владельцев в группу при ее создании, чтобы указать владельцев, которые могут изменять группу.</span><span class="sxs-lookup"><span data-stu-id="ef8be-165">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="ef8be-166">Создание группы Office 365 программным путем с контекстом только для приложений, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="ef8be-166">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="ef8be-167">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="ef8be-167">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="ef8be-168">При необходимости укажите другие записываемые свойства для своей группы.</span><span class="sxs-lookup"><span data-stu-id="ef8be-168">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="ef8be-169">Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="ef8be-169">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="ef8be-170">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="ef8be-170">groupTypes options</span></span>

<span data-ttu-id="ef8be-171">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="ef8be-171">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="ef8be-172">Тип группы</span><span class="sxs-lookup"><span data-stu-id="ef8be-172">Type of group</span></span> | <span data-ttu-id="ef8be-173">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="ef8be-173">Assigned membership</span></span> | <span data-ttu-id="ef8be-174">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="ef8be-174">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="ef8be-175">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="ef8be-175">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="ef8be-176">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="ef8be-176">Dynamic</span></span> | <span data-ttu-id="ef8be-177">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="ef8be-177">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="ef8be-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef8be-178">Response</span></span>

<span data-ttu-id="ef8be-179">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef8be-179">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="ef8be-180">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="ef8be-180">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="ef8be-181">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef8be-181">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="ef8be-182">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="ef8be-182">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="ef8be-183">В приведенном ниже примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="ef8be-183">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="ef8be-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef8be-184">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ef8be-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef8be-185">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ef8be-186">C#</span><span class="sxs-lookup"><span data-stu-id="ef8be-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef8be-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef8be-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef8be-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef8be-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef8be-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef8be-189">Response</span></span>

<span data-ttu-id="ef8be-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef8be-190">The following is an example of the response.</span></span>

><span data-ttu-id="ef8be-191">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef8be-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ef8be-192">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef8be-192">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="ef8be-193">Пример 2. Создание группы Office 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="ef8be-193">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="ef8be-194">В следующем примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="ef8be-194">The following example creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="ef8be-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef8be-195">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ef8be-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef8be-196">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ef8be-197">C#</span><span class="sxs-lookup"><span data-stu-id="ef8be-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef8be-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef8be-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef8be-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef8be-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef8be-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef8be-200">Response</span></span> 

<span data-ttu-id="ef8be-201">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="ef8be-201">The following is an example of a successful response.</span></span> <span data-ttu-id="ef8be-202">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef8be-202">It includes only default properties.</span></span> <span data-ttu-id="ef8be-203">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="ef8be-203">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="ef8be-204">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef8be-204">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ef8be-205">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef8be-205">All the default properties are returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ef8be-206">См. также</span><span class="sxs-lookup"><span data-stu-id="ef8be-206">See also</span></span>

- [<span data-ttu-id="ef8be-207">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ef8be-207">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ef8be-208">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ef8be-208">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ef8be-209">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ef8be-209">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
