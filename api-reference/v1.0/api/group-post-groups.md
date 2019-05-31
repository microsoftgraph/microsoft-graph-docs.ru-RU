---
title: Создание группы
description: 'Создание группы согласно инструкциям в тексте запроса. '
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 0a525ffffe62685e863572c0e81c808b2c6e8a02
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537123"
---
# <a name="create-group"></a><span data-ttu-id="d3d45-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="d3d45-103">Create group</span></span>
<span data-ttu-id="d3d45-104">Создание группы согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d3d45-104">Create a new channel in a Microsoft Team, as specified in the request body.</span></span> <span data-ttu-id="d3d45-105">Вы можете создавать группы указанных ниже типов.</span><span class="sxs-lookup"><span data-stu-id="d3d45-105">You can use the New-DistributionGroup cmdlet to create the following types of groups:</span></span>

* <span data-ttu-id="d3d45-106">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="d3d45-106">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="d3d45-107">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="d3d45-107">Security group</span></span>

<span data-ttu-id="d3d45-108">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="d3d45-108">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="d3d45-109">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="d3d45-109">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="d3d45-110">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="d3d45-110">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="d3d45-111">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="d3d45-111">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="d3d45-p104">**Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d3d45-p104">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3d45-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3d45-114">Permissions</span></span>
<span data-ttu-id="d3d45-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3d45-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3d45-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3d45-117">Permission type</span></span>      | <span data-ttu-id="d3d45-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3d45-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3d45-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3d45-119">Delegated (work or school account)</span></span> | <span data-ttu-id="d3d45-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d45-120">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3d45-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3d45-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3d45-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3d45-122">Not supported.</span></span>    |
|<span data-ttu-id="d3d45-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3d45-123">Application</span></span> | <span data-ttu-id="d3d45-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d45-124">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3d45-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3d45-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="d3d45-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3d45-126">Request headers</span></span>
| <span data-ttu-id="d3d45-127">Имя</span><span class="sxs-lookup"><span data-stu-id="d3d45-127">Name</span></span>       | <span data-ttu-id="d3d45-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d3d45-128">Type</span></span> | <span data-ttu-id="d3d45-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d45-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d3d45-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3d45-130">Authorization</span></span>  | <span data-ttu-id="d3d45-131">string</span><span class="sxs-lookup"><span data-stu-id="d3d45-131">string</span></span>  | <span data-ttu-id="d3d45-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3d45-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3d45-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3d45-134">Content-Type</span></span>  | <span data-ttu-id="d3d45-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d3d45-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3d45-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3d45-136">Request body</span></span>
<span data-ttu-id="d3d45-137">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="d3d45-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="d3d45-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3d45-138">Property</span></span> | <span data-ttu-id="d3d45-139">Тип</span><span class="sxs-lookup"><span data-stu-id="d3d45-139">Type</span></span> | <span data-ttu-id="d3d45-140">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d45-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d3d45-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d3d45-141">displayName</span></span> | <span data-ttu-id="d3d45-142">string</span><span class="sxs-lookup"><span data-stu-id="d3d45-142">string</span></span> | <span data-ttu-id="d3d45-143">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="d3d45-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="d3d45-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3d45-144">Required.</span></span> |
| <span data-ttu-id="d3d45-145">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="d3d45-145">mailEnabled</span></span> | <span data-ttu-id="d3d45-146">boolean</span><span class="sxs-lookup"><span data-stu-id="d3d45-146">boolean</span></span> | <span data-ttu-id="d3d45-147">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="d3d45-147">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="d3d45-148">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3d45-148">Required.</span></span> |
| <span data-ttu-id="d3d45-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d3d45-149">mailNickname</span></span> | <span data-ttu-id="d3d45-150">string</span><span class="sxs-lookup"><span data-stu-id="d3d45-150">string</span></span> | <span data-ttu-id="d3d45-151">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="d3d45-151">The mail alias for the group.</span></span> <span data-ttu-id="d3d45-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3d45-152">Required.</span></span> |
| <span data-ttu-id="d3d45-153">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="d3d45-153">securityEnabled</span></span> | <span data-ttu-id="d3d45-154">boolean</span><span class="sxs-lookup"><span data-stu-id="d3d45-154">boolean</span></span> | <span data-ttu-id="d3d45-155">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="d3d45-155">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="d3d45-156">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d3d45-156">Required.</span></span> |
| <span data-ttu-id="d3d45-157">owners</span><span class="sxs-lookup"><span data-stu-id="d3d45-157">owners</span></span> | <span data-ttu-id="d3d45-158">string collection</span><span class="sxs-lookup"><span data-stu-id="d3d45-158">string collection</span></span> | <span data-ttu-id="d3d45-159">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="d3d45-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="d3d45-160">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d3d45-160">Optional.</span></span> |
| <span data-ttu-id="d3d45-161">members</span><span class="sxs-lookup"><span data-stu-id="d3d45-161">members</span></span> | <span data-ttu-id="d3d45-162">string collection</span><span class="sxs-lookup"><span data-stu-id="d3d45-162">string collection</span></span> | <span data-ttu-id="d3d45-163">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="d3d45-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="d3d45-164">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d3d45-164">Optional.</span></span> |

> <span data-ttu-id="d3d45-165">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="d3d45-165">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="d3d45-166">При необходимости укажите другие записываемые свойства для своей группы.</span><span class="sxs-lookup"><span data-stu-id="d3d45-166">Specify other writable properties as necessary for your group. For more information, see the properties of the group resource.</span></span> <span data-ttu-id="d3d45-167">Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="d3d45-167">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="d3d45-168">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="d3d45-168">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="d3d45-169">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="d3d45-169">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

### <a name="grouptypes-options"></a><span data-ttu-id="d3d45-170">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="d3d45-170">groupTypes options</span></span>

<span data-ttu-id="d3d45-171">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="d3d45-171">Use the **groupTypes** property to control the type of group and its membership, as shown below:</span></span>

| <span data-ttu-id="d3d45-172">Тип группы</span><span class="sxs-lookup"><span data-stu-id="d3d45-172">Type of group</span></span> | <span data-ttu-id="d3d45-173">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="d3d45-173">Assigned membership</span></span> | <span data-ttu-id="d3d45-174">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="d3d45-174">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="d3d45-175">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="d3d45-175">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="d3d45-176">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="d3d45-176">Dynamic</span></span> | <span data-ttu-id="d3d45-177">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="d3d45-177">Null</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="d3d45-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3d45-178">Response</span></span>
<span data-ttu-id="d3d45-179">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d3d45-179">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="d3d45-180">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="d3d45-180">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="d3d45-181">Примеры</span><span class="sxs-lookup"><span data-stu-id="d3d45-181">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="d3d45-182">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="d3d45-182">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="d3d45-183">В приведенном ниже примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="d3d45-183">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="d3d45-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3d45-184">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d3d45-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3d45-185">Response</span></span>

<span data-ttu-id="d3d45-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3d45-186">The following is an example of the response.</span></span>

><span data-ttu-id="d3d45-187">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3d45-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d3d45-188">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d3d45-188">All the default properties are returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3d45-189">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3d45-189">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3d45-190">C#</span><span class="sxs-lookup"><span data-stu-id="d3d45-190">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3d45-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3d45-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="d3d45-192">Пример 2. Создание группы с владельцами и участниками</span><span class="sxs-lookup"><span data-stu-id="d3d45-192">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="d3d45-193">В приведенном ниже примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="d3d45-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>

#### <a name="request"></a><span data-ttu-id="d3d45-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3d45-194">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="d3d45-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3d45-195">Response</span></span>

<span data-ttu-id="d3d45-196">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="d3d45-196">The following is an example of a successful response.</span></span> <span data-ttu-id="d3d45-197">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d3d45-197">It includes only default properties.</span></span> <span data-ttu-id="d3d45-198">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="d3d45-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="d3d45-199">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3d45-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d3d45-200">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d3d45-200">All the default properties are returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d3d45-201">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d3d45-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d3d45-202">C#</span><span class="sxs-lookup"><span data-stu-id="d3d45-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3d45-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3d45-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_prepopulated_group-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-post-groups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
