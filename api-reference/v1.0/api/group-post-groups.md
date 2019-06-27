---
title: Создание группы
description: 'Создание группы согласно инструкциям в тексте запроса. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: ff8d4c28e4b2fed0858650d704dca34feb8eb79a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277786"
---
# <a name="create-group"></a><span data-ttu-id="18231-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="18231-103">Create group</span></span>
<span data-ttu-id="18231-104">Создание группы согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="18231-104">Create a new channel in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="18231-105">Вы можете создавать группы указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="18231-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="18231-106">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="18231-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="18231-107">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="18231-107">Security group</span></span>

<span data-ttu-id="18231-108">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="18231-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="18231-109">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="18231-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="18231-110">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="18231-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="18231-p103">**Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="18231-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="18231-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18231-113">Permissions</span></span>
<span data-ttu-id="18231-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18231-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18231-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18231-116">Permission type</span></span>      | <span data-ttu-id="18231-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18231-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18231-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18231-118">Delegated (work or school account)</span></span> | <span data-ttu-id="18231-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18231-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="18231-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18231-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18231-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18231-121">Not supported.</span></span>    |
|<span data-ttu-id="18231-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18231-122">Application</span></span> | <span data-ttu-id="18231-123">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18231-123">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18231-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18231-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="18231-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18231-125">Request headers</span></span>
| <span data-ttu-id="18231-126">Имя</span><span class="sxs-lookup"><span data-stu-id="18231-126">Name</span></span>       | <span data-ttu-id="18231-127">Тип</span><span class="sxs-lookup"><span data-stu-id="18231-127">Type</span></span> | <span data-ttu-id="18231-128">Описание</span><span class="sxs-lookup"><span data-stu-id="18231-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18231-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="18231-129">Authorization</span></span>  | <span data-ttu-id="18231-130">string</span><span class="sxs-lookup"><span data-stu-id="18231-130">string</span></span>  | <span data-ttu-id="18231-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18231-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18231-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18231-133">Content-Type</span></span>  | <span data-ttu-id="18231-134">application/json</span><span class="sxs-lookup"><span data-stu-id="18231-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18231-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18231-135">Request body</span></span>
<span data-ttu-id="18231-136">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="18231-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="18231-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="18231-137">Property</span></span> | <span data-ttu-id="18231-138">Тип</span><span class="sxs-lookup"><span data-stu-id="18231-138">Type</span></span> | <span data-ttu-id="18231-139">Описание</span><span class="sxs-lookup"><span data-stu-id="18231-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18231-140">displayName</span><span class="sxs-lookup"><span data-stu-id="18231-140">displayName</span></span> | <span data-ttu-id="18231-141">string</span><span class="sxs-lookup"><span data-stu-id="18231-141">string</span></span> | <span data-ttu-id="18231-142">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="18231-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="18231-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18231-143">Required.</span></span> |
| <span data-ttu-id="18231-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="18231-144">mailEnabled</span></span> | <span data-ttu-id="18231-145">boolean</span><span class="sxs-lookup"><span data-stu-id="18231-145">boolean</span></span> | <span data-ttu-id="18231-146">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="18231-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="18231-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="18231-147">Required.</span></span> |
| <span data-ttu-id="18231-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="18231-148">mailNickname</span></span> | <span data-ttu-id="18231-149">string</span><span class="sxs-lookup"><span data-stu-id="18231-149">string</span></span> | <span data-ttu-id="18231-150">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="18231-150">The mail alias for the group.</span></span> <span data-ttu-id="18231-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18231-151">Required.</span></span> |
| <span data-ttu-id="18231-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="18231-152">securityEnabled</span></span> | <span data-ttu-id="18231-153">boolean</span><span class="sxs-lookup"><span data-stu-id="18231-153">boolean</span></span> | <span data-ttu-id="18231-154">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="18231-154">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="18231-155">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="18231-155">Required.</span></span> |
| <span data-ttu-id="18231-156">owners</span><span class="sxs-lookup"><span data-stu-id="18231-156">owners</span></span> | <span data-ttu-id="18231-157">string collection</span><span class="sxs-lookup"><span data-stu-id="18231-157">string collection</span></span> | <span data-ttu-id="18231-158">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="18231-158">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="18231-159">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="18231-159">Optional.</span></span> |
| <span data-ttu-id="18231-160">members</span><span class="sxs-lookup"><span data-stu-id="18231-160">members</span></span> | <span data-ttu-id="18231-161">string collection</span><span class="sxs-lookup"><span data-stu-id="18231-161">string collection</span></span> | <span data-ttu-id="18231-162">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="18231-162">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="18231-163">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="18231-163">Optional.</span></span> |

> <span data-ttu-id="18231-164">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="18231-164">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="18231-165">При необходимости укажите другие записываемые свойства для своей группы.</span><span class="sxs-lookup"><span data-stu-id="18231-165">Specify other writable properties as necessary for your group. For more information, see the properties of the group resource.</span></span> <span data-ttu-id="18231-166">Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="18231-166">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="18231-167">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="18231-167">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="18231-168">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="18231-168">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="18231-169">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="18231-169">groupTypes options</span></span>

<span data-ttu-id="18231-170">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="18231-170">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="18231-171">Тип группы</span><span class="sxs-lookup"><span data-stu-id="18231-171">Type of group</span></span> | <span data-ttu-id="18231-172">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="18231-172">Assigned membership</span></span> | <span data-ttu-id="18231-173">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="18231-173">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="18231-174">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="18231-174">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="18231-175">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="18231-175">Dynamic</span></span> | <span data-ttu-id="18231-176">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="18231-176">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="18231-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="18231-177">Response</span></span>
<span data-ttu-id="18231-178">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18231-178">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="18231-179">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="18231-179">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="18231-180">Примеры</span><span class="sxs-lookup"><span data-stu-id="18231-180">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="18231-181">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="18231-181">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="18231-182">В приведенном ниже примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="18231-182">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="18231-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="18231-183">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="18231-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="18231-184">Response</span></span>

<span data-ttu-id="18231-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18231-185">The following is an example of the response.</span></span>

><span data-ttu-id="18231-186">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="18231-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18231-187">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="18231-187">All the default properties are returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="18231-188">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="18231-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18231-189">C#</span><span class="sxs-lookup"><span data-stu-id="18231-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18231-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18231-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="18231-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18231-191">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="18231-192">Пример 2. Создание группы с владельцами и участниками</span><span class="sxs-lookup"><span data-stu-id="18231-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="18231-193">В приведенном ниже примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="18231-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="18231-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="18231-194">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="18231-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="18231-195">Response</span></span>

<span data-ttu-id="18231-196">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="18231-196">The following is an example of a successful response.</span></span> <span data-ttu-id="18231-197">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="18231-197">It includes only default properties.</span></span> <span data-ttu-id="18231-198">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="18231-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="18231-199">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="18231-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18231-200">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="18231-200">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="18231-201">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="18231-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18231-202">C#</span><span class="sxs-lookup"><span data-stu-id="18231-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18231-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18231-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="18231-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18231-204">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
