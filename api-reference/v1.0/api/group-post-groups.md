---
title: Создание группы
description: 'Создание группы согласно инструкциям в тексте запроса. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 418c24dcb3779725cadb41e59c712c870d1bd74a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516993"
---
# <a name="create-group"></a><span data-ttu-id="33875-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="33875-103">Create group</span></span>

<span data-ttu-id="33875-104">Пространство имен: microsoft.graph. Создание группы согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="33875-104">Namespace: microsoft.graph Create a new group as specified in the request body.</span></span> <span data-ttu-id="33875-105">Вы можете создавать группы указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="33875-105">You can create the following types of groups:</span></span>

* <span data-ttu-id="33875-106">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="33875-106">Office 365 group (unified group)</span></span>
* <span data-ttu-id="33875-107">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="33875-107">Security group</span></span>

<span data-ttu-id="33875-108">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="33875-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="33875-109">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="33875-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="33875-110">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="33875-110">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="33875-111">**Примечание.** Несмотря на то, что Microsoft Teams создан на основе групп Office 365, в настоящее время нельзя создать команду через этот API.</span><span class="sxs-lookup"><span data-stu-id="33875-111">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API.</span></span> <span data-ttu-id="33875-112">Вы можете использовать другие API групп для управления командой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="33875-112">You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="33875-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33875-113">Permissions</span></span>
<span data-ttu-id="33875-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33875-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33875-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33875-116">Permission type</span></span>      | <span data-ttu-id="33875-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33875-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33875-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33875-118">Delegated (work or school account)</span></span> | <span data-ttu-id="33875-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33875-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="33875-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33875-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33875-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33875-121">Not supported.</span></span>    |
|<span data-ttu-id="33875-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="33875-122">Application</span></span> | <span data-ttu-id="33875-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33875-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33875-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33875-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="33875-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33875-125">Request headers</span></span>
| <span data-ttu-id="33875-126">Имя</span><span class="sxs-lookup"><span data-stu-id="33875-126">Name</span></span>       | <span data-ttu-id="33875-127">Тип</span><span class="sxs-lookup"><span data-stu-id="33875-127">Type</span></span> | <span data-ttu-id="33875-128">Описание</span><span class="sxs-lookup"><span data-stu-id="33875-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33875-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="33875-129">Authorization</span></span>  | <span data-ttu-id="33875-130">string</span><span class="sxs-lookup"><span data-stu-id="33875-130">string</span></span>  | <span data-ttu-id="33875-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33875-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33875-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33875-133">Content-Type</span></span>  | <span data-ttu-id="33875-134">application/json</span><span class="sxs-lookup"><span data-stu-id="33875-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33875-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33875-135">Request body</span></span>
<span data-ttu-id="33875-136">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="33875-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="33875-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="33875-137">Property</span></span> | <span data-ttu-id="33875-138">Тип</span><span class="sxs-lookup"><span data-stu-id="33875-138">Type</span></span> | <span data-ttu-id="33875-139">Описание</span><span class="sxs-lookup"><span data-stu-id="33875-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33875-140">displayName</span><span class="sxs-lookup"><span data-stu-id="33875-140">displayName</span></span> | <span data-ttu-id="33875-141">string</span><span class="sxs-lookup"><span data-stu-id="33875-141">string</span></span> | <span data-ttu-id="33875-142">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="33875-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="33875-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33875-143">Required.</span></span> |
| <span data-ttu-id="33875-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="33875-144">mailEnabled</span></span> | <span data-ttu-id="33875-145">boolean</span><span class="sxs-lookup"><span data-stu-id="33875-145">boolean</span></span> | <span data-ttu-id="33875-146">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="33875-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="33875-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="33875-147">Required.</span></span> |
| <span data-ttu-id="33875-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="33875-148">mailNickname</span></span> | <span data-ttu-id="33875-149">string</span><span class="sxs-lookup"><span data-stu-id="33875-149">string</span></span> | <span data-ttu-id="33875-150">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="33875-150">The mail alias for the group.</span></span> <span data-ttu-id="33875-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33875-151">Required.</span></span> |
| <span data-ttu-id="33875-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="33875-152">securityEnabled</span></span> | <span data-ttu-id="33875-153">boolean</span><span class="sxs-lookup"><span data-stu-id="33875-153">boolean</span></span> | <span data-ttu-id="33875-154">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="33875-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="33875-155">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="33875-155">Required.</span></span> |
| <span data-ttu-id="33875-156">owners</span><span class="sxs-lookup"><span data-stu-id="33875-156">owners</span></span> | <span data-ttu-id="33875-157">string collection</span><span class="sxs-lookup"><span data-stu-id="33875-157">string collection</span></span> | <span data-ttu-id="33875-158">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="33875-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="33875-159">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="33875-159">Optional.</span></span> |
| <span data-ttu-id="33875-160">members</span><span class="sxs-lookup"><span data-stu-id="33875-160">members</span></span> | <span data-ttu-id="33875-161">string collection</span><span class="sxs-lookup"><span data-stu-id="33875-161">string collection</span></span> | <span data-ttu-id="33875-162">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="33875-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="33875-163">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="33875-163">Optional.</span></span> |

> <span data-ttu-id="33875-164">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="33875-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="33875-165">При необходимости укажите другие записываемые свойства для своей группы.</span><span class="sxs-lookup"><span data-stu-id="33875-165">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="33875-166">Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="33875-166">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="33875-167">**Примечание.** Создание группы с помощью разрешения приложения Group.Create без указания владельцев анонимно создает группу, которая не будет изменяться.</span><span class="sxs-lookup"><span data-stu-id="33875-167">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="33875-168">Вы можете использовать операцию `POST` и добавить владельцев в группу при ее создании, чтобы указать владельцев, которые могут изменять группу.</span><span class="sxs-lookup"><span data-stu-id="33875-168">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="33875-169">Создание группы Office 365 программным путем с контекстом только для приложений, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="33875-169">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="33875-170">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="33875-170">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  


### <a name="grouptypes-options"></a><span data-ttu-id="33875-171">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="33875-171">groupTypes options</span></span>

<span data-ttu-id="33875-172">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="33875-172">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="33875-173">Тип группы</span><span class="sxs-lookup"><span data-stu-id="33875-173">Type of group</span></span> | <span data-ttu-id="33875-174">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="33875-174">Assigned membership</span></span> | <span data-ttu-id="33875-175">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="33875-175">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="33875-176">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="33875-176">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="33875-177">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="33875-177">Dynamic</span></span> | <span data-ttu-id="33875-178">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="33875-178">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="33875-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="33875-179">Response</span></span>
<span data-ttu-id="33875-180">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="33875-180">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="33875-181">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="33875-181">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="33875-182">Примеры</span><span class="sxs-lookup"><span data-stu-id="33875-182">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="33875-183">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="33875-183">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="33875-184">В приведенном ниже примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="33875-184">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="33875-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="33875-185">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="33875-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="33875-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="33875-187">C#</span><span class="sxs-lookup"><span data-stu-id="33875-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33875-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33875-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33875-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33875-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33875-190">Java</span><span class="sxs-lookup"><span data-stu-id="33875-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33875-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="33875-191">Response</span></span>

<span data-ttu-id="33875-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33875-192">The following is an example of the response.</span></span>

><span data-ttu-id="33875-193">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="33875-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="33875-194">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33875-194">All the default properties are returned from an actual call.</span></span>
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
      "mail": "library7423@contoso.com",
      "mailEnabled": true,
      "mailNickname": "library",
      "onPremisesLastSyncDateTime": null,
      "onPremisesSecurityIdentifier": null,
      "onPremisesSyncEnabled": null,
      "preferredDataLocation": "CAN",
      "proxyAddresses": [
          "SMTP:library7423@contoso.com"
      ],
      "renewedDateTime": "2018-12-22T00:51:37Z",
      "resourceBehaviorOptions": [],
      "resourceProvisioningOptions": [],
      "securityEnabled": false,
      "visibility": "Public",
      "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="33875-195">Пример 2. Создание группы с владельцами и участниками</span><span class="sxs-lookup"><span data-stu-id="33875-195">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="33875-196">В приведенном ниже примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="33875-196">The following example creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="33875-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="33875-197">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="33875-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="33875-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups
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
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="33875-199">C#</span><span class="sxs-lookup"><span data-stu-id="33875-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33875-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33875-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33875-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33875-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33875-202">Java</span><span class="sxs-lookup"><span data-stu-id="33875-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33875-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="33875-203">Response</span></span>

<span data-ttu-id="33875-204">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="33875-204">The following is an example of a successful response.</span></span> <span data-ttu-id="33875-205">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33875-205">It includes only default properties.</span></span> <span data-ttu-id="33875-206">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="33875-206">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="33875-207">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="33875-207">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="33875-208">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33875-208">All the default properties are returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
