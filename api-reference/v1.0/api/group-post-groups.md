---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8bf432d30ba000641654d8c5d457096f5bfcb70e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574868"
---
# <a name="create-group"></a><span data-ttu-id="e7b82-104">Создание группы</span><span class="sxs-lookup"><span data-stu-id="e7b82-104">Create group</span></span>
<span data-ttu-id="e7b82-p102">Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="e7b82-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="e7b82-107">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="e7b82-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="e7b82-108">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="e7b82-108">Dynamic group</span></span>
* <span data-ttu-id="e7b82-109">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="e7b82-109">Security group</span></span>

<span data-ttu-id="e7b82-110">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="e7b82-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="e7b82-111">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="e7b82-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="e7b82-112">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="e7b82-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="e7b82-113">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="e7b82-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="e7b82-p105">**Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7b82-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7b82-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7b82-116">Permissions</span></span>
<span data-ttu-id="e7b82-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7b82-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7b82-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7b82-119">Permission type</span></span>      | <span data-ttu-id="e7b82-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7b82-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7b82-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7b82-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e7b82-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b82-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7b82-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7b82-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7b82-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b82-124">Not supported.</span></span>    |
|<span data-ttu-id="e7b82-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7b82-125">Application</span></span> | <span data-ttu-id="e7b82-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b82-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7b82-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7b82-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="e7b82-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7b82-128">Request headers</span></span>
| <span data-ttu-id="e7b82-129">Имя</span><span class="sxs-lookup"><span data-stu-id="e7b82-129">Name</span></span>       | <span data-ttu-id="e7b82-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7b82-130">Type</span></span> | <span data-ttu-id="e7b82-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7b82-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7b82-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7b82-132">Authorization</span></span>  | <span data-ttu-id="e7b82-133">string</span><span class="sxs-lookup"><span data-stu-id="e7b82-133">string</span></span>  | <span data-ttu-id="e7b82-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7b82-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7b82-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7b82-136">Content-Type</span></span>  | <span data-ttu-id="e7b82-137">application/json</span><span class="sxs-lookup"><span data-stu-id="e7b82-137">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7b82-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7b82-138">Request body</span></span>
<span data-ttu-id="e7b82-139">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="e7b82-139">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="e7b82-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7b82-140">Property</span></span> | <span data-ttu-id="e7b82-141">Тип</span><span class="sxs-lookup"><span data-stu-id="e7b82-141">Type</span></span> | <span data-ttu-id="e7b82-142">Описание</span><span class="sxs-lookup"><span data-stu-id="e7b82-142">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7b82-143">displayName</span><span class="sxs-lookup"><span data-stu-id="e7b82-143">displayName</span></span> | <span data-ttu-id="e7b82-144">string</span><span class="sxs-lookup"><span data-stu-id="e7b82-144">string</span></span> | <span data-ttu-id="e7b82-145">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="e7b82-145">The name to display in the address book for the group.</span></span> <span data-ttu-id="e7b82-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7b82-146">Required.</span></span> |
| <span data-ttu-id="e7b82-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="e7b82-147">mailEnabled</span></span> | <span data-ttu-id="e7b82-148">boolean</span><span class="sxs-lookup"><span data-stu-id="e7b82-148">boolean</span></span> | <span data-ttu-id="e7b82-149">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="e7b82-149">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="e7b82-150">При создании группы Office 365 установите значение **true**.</span><span class="sxs-lookup"><span data-stu-id="e7b82-150">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="e7b82-151">При создании динамической группы или группы безопасности установите для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e7b82-151">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="e7b82-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7b82-152">Required.</span></span> |
| <span data-ttu-id="e7b82-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e7b82-153">mailNickname</span></span> | <span data-ttu-id="e7b82-154">string</span><span class="sxs-lookup"><span data-stu-id="e7b82-154">string</span></span> | <span data-ttu-id="e7b82-155">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="e7b82-155">The mail alias for the group.</span></span> <span data-ttu-id="e7b82-156">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7b82-156">Required.</span></span> |
| <span data-ttu-id="e7b82-157">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="e7b82-157">securityEnabled</span></span> | <span data-ttu-id="e7b82-158">boolean</span><span class="sxs-lookup"><span data-stu-id="e7b82-158">boolean</span></span> | <span data-ttu-id="e7b82-159">Установите значение **true** для защищенных групп.</span><span class="sxs-lookup"><span data-stu-id="e7b82-159">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="e7b82-160">При создании динамической группы или группы безопасности установите для этого свойства значение **true**.</span><span class="sxs-lookup"><span data-stu-id="e7b82-160">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="e7b82-161">Установите значение **false** при создании группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="e7b82-161">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="e7b82-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7b82-162">Required.</span></span> |
| <span data-ttu-id="e7b82-163">owners</span><span class="sxs-lookup"><span data-stu-id="e7b82-163">owners</span></span> | <span data-ttu-id="e7b82-164">string collection</span><span class="sxs-lookup"><span data-stu-id="e7b82-164">string collection</span></span> | <span data-ttu-id="e7b82-165">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="e7b82-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="e7b82-166">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e7b82-166">Optional.</span></span> |
| <span data-ttu-id="e7b82-167">members</span><span class="sxs-lookup"><span data-stu-id="e7b82-167">members</span></span> | <span data-ttu-id="e7b82-168">string collection</span><span class="sxs-lookup"><span data-stu-id="e7b82-168">string collection</span></span> | <span data-ttu-id="e7b82-169">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="e7b82-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="e7b82-170">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e7b82-170">Optional.</span></span> |


<span data-ttu-id="e7b82-171">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="e7b82-171">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="e7b82-172">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="e7b82-172">groupTypes options</span></span>

| <span data-ttu-id="e7b82-173">Тип группы</span><span class="sxs-lookup"><span data-stu-id="e7b82-173">Type of group</span></span> | <span data-ttu-id="e7b82-174">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="e7b82-174">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="e7b82-175">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="e7b82-175">Office 365 (aka unified group)</span></span>| <span data-ttu-id="e7b82-176">"Unified"</span><span class="sxs-lookup"><span data-stu-id="e7b82-176">"Unified"</span></span> |
| <span data-ttu-id="e7b82-177">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="e7b82-177">Dynamic</span></span> | <span data-ttu-id="e7b82-178">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="e7b82-178">"DynamicMembership"</span></span> |
| <span data-ttu-id="e7b82-179">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="e7b82-179">Security</span></span> | <span data-ttu-id="e7b82-180">Не задавайте.</span><span class="sxs-lookup"><span data-stu-id="e7b82-180">Do not set.</span></span> |


><span data-ttu-id="e7b82-181">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="e7b82-181">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="e7b82-182">Это может привести к тому, что связанный с ней сайт SharePoint Online, не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="e7b82-182">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="e7b82-p115">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="e7b82-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="e7b82-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7b82-185">Response</span></span>
<span data-ttu-id="e7b82-186">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7b82-186">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e7b82-187">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="e7b82-187">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="e7b82-188">Пример</span><span class="sxs-lookup"><span data-stu-id="e7b82-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e7b82-189">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="e7b82-189">Request 1</span></span>
<span data-ttu-id="e7b82-190">Первый пример запроса создает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="e7b82-190">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
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

#### <a name="response-1"></a><span data-ttu-id="e7b82-191">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="e7b82-191">Response 1</span></span>
<span data-ttu-id="e7b82-192">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e7b82-192">The following is an example of the response.</span></span>
><span data-ttu-id="e7b82-193">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e7b82-193">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7b82-194">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e7b82-194">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
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

#### <a name="request-2"></a><span data-ttu-id="e7b82-195">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="e7b82-195">Request 2</span></span>
<span data-ttu-id="e7b82-196">Второй пример запроса создает группу Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="e7b82-196">The second example request creates an Office 365 group with an owner and members specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
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

#### <a name="response-2"></a><span data-ttu-id="e7b82-197">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="e7b82-197">Response 2</span></span>
<span data-ttu-id="e7b82-198">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="e7b82-198">The following is an example of a successful response.</span></span> <span data-ttu-id="e7b82-199">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e7b82-199">It includes only default properties.</span></span> <span data-ttu-id="e7b82-200">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="e7b82-200">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="e7b82-201">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e7b82-201">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7b82-202">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e7b82-202">All the default properties are returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
```http
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
  "tocPath": ""
}-->
