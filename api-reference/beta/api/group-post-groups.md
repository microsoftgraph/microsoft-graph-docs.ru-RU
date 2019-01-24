---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 736c4350cc5c7c57d0b57562676317317f6f74dc
ms.sourcegitcommit: 71368f59d267c8188567529e74486e54cc122804
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29442327"
---
# <a name="create-group"></a><span data-ttu-id="7ef96-104">Создание группы</span><span class="sxs-lookup"><span data-stu-id="7ef96-104">Create group</span></span>

> <span data-ttu-id="7ef96-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ef96-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ef96-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef96-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ef96-p103">Используйте этот API, чтобы создать [группу](../resources/group.md) согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="7ef96-p103">Use this API to create a new [group](../resources/group.md) as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="7ef96-109">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="7ef96-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="7ef96-110">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="7ef96-110">Dynamic group</span></span>
* <span data-ttu-id="7ef96-111">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="7ef96-111">Security group</span></span>

<span data-ttu-id="7ef96-112">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="7ef96-112">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="7ef96-113">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="7ef96-113">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="7ef96-114">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="7ef96-114">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="7ef96-115">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="7ef96-115">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="7ef96-116">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="7ef96-116">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ef96-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef96-117">Permissions</span></span>
<span data-ttu-id="7ef96-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ef96-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ef96-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef96-120">Permission type</span></span>      | <span data-ttu-id="7ef96-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ef96-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ef96-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ef96-122">Delegated (work or school account)</span></span> | <span data-ttu-id="7ef96-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef96-123">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ef96-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ef96-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ef96-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef96-125">Not supported.</span></span>    |
|<span data-ttu-id="7ef96-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ef96-126">Application</span></span> | <span data-ttu-id="7ef96-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef96-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ef96-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ef96-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7ef96-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ef96-129">Request headers</span></span>
| <span data-ttu-id="7ef96-130">Имя</span><span class="sxs-lookup"><span data-stu-id="7ef96-130">Name</span></span>       | <span data-ttu-id="7ef96-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef96-131">Type</span></span> | <span data-ttu-id="7ef96-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef96-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ef96-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ef96-133">Authorization</span></span>  | <span data-ttu-id="7ef96-134">string</span><span class="sxs-lookup"><span data-stu-id="7ef96-134">string</span></span>  | <span data-ttu-id="7ef96-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef96-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ef96-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ef96-137">Request body</span></span>
<span data-ttu-id="7ef96-138">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="7ef96-138">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7ef96-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ef96-139">Property</span></span> | <span data-ttu-id="7ef96-140">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef96-140">Type</span></span> | <span data-ttu-id="7ef96-141">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef96-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ef96-142">displayName</span><span class="sxs-lookup"><span data-stu-id="7ef96-142">displayName</span></span> | <span data-ttu-id="7ef96-143">string</span><span class="sxs-lookup"><span data-stu-id="7ef96-143">string</span></span> | <span data-ttu-id="7ef96-144">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="7ef96-144">The name to display in the address book for the group.</span></span> <span data-ttu-id="7ef96-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef96-145">Required.</span></span> |
| <span data-ttu-id="7ef96-146">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7ef96-146">mailEnabled</span></span> | <span data-ttu-id="7ef96-147">boolean</span><span class="sxs-lookup"><span data-stu-id="7ef96-147">boolean</span></span> | <span data-ttu-id="7ef96-148">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="7ef96-148">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="7ef96-149">При создании группы Office 365 установите значение **true**.</span><span class="sxs-lookup"><span data-stu-id="7ef96-149">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="7ef96-150">При создании динамической группы или группы безопасности установите для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7ef96-150">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="7ef96-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef96-151">Required.</span></span> |
| <span data-ttu-id="7ef96-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7ef96-152">mailNickname</span></span> | <span data-ttu-id="7ef96-153">string</span><span class="sxs-lookup"><span data-stu-id="7ef96-153">string</span></span> | <span data-ttu-id="7ef96-154">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="7ef96-154">The mail alias for the group.</span></span> <span data-ttu-id="7ef96-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef96-155">Required.</span></span> |
| <span data-ttu-id="7ef96-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7ef96-156">securityEnabled</span></span> | <span data-ttu-id="7ef96-157">boolean</span><span class="sxs-lookup"><span data-stu-id="7ef96-157">boolean</span></span> | <span data-ttu-id="7ef96-158">Установите значение **true** для защищенных групп.</span><span class="sxs-lookup"><span data-stu-id="7ef96-158">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="7ef96-159">При создании динамической группы или группы безопасности установите для этого свойства значение **true**.</span><span class="sxs-lookup"><span data-stu-id="7ef96-159">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="7ef96-160">При создании группы Office 365 установите значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7ef96-160">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="7ef96-161">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ef96-161">Required.</span></span> |
| <span data-ttu-id="7ef96-162">owners</span><span class="sxs-lookup"><span data-stu-id="7ef96-162">owners</span></span> | <span data-ttu-id="7ef96-163">string collection</span><span class="sxs-lookup"><span data-stu-id="7ef96-163">string collection</span></span> | <span data-ttu-id="7ef96-164">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="7ef96-164">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="7ef96-165">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7ef96-165">Optional.</span></span> |
| <span data-ttu-id="7ef96-166">members</span><span class="sxs-lookup"><span data-stu-id="7ef96-166">members</span></span> | <span data-ttu-id="7ef96-167">string collection</span><span class="sxs-lookup"><span data-stu-id="7ef96-167">string collection</span></span> | <span data-ttu-id="7ef96-168">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="7ef96-168">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="7ef96-169">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7ef96-169">Optional.</span></span> |

<span data-ttu-id="7ef96-170">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="7ef96-170">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="7ef96-171">Тип группы</span><span class="sxs-lookup"><span data-stu-id="7ef96-171">Type of group</span></span> | <span data-ttu-id="7ef96-172">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="7ef96-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="7ef96-173">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="7ef96-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="7ef96-174">"Unified"</span><span class="sxs-lookup"><span data-stu-id="7ef96-174">"Unified"</span></span> |
| <span data-ttu-id="7ef96-175">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="7ef96-175">Dynamic</span></span> | <span data-ttu-id="7ef96-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="7ef96-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="7ef96-177">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="7ef96-177">Security</span></span> | <span data-ttu-id="7ef96-178">Не следует устанавливать.</span><span class="sxs-lookup"><span data-stu-id="7ef96-178">Do not set.</span></span> |

<span data-ttu-id="7ef96-179">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="7ef96-179">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="7ef96-180">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="7ef96-180">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="7ef96-181">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="7ef96-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7ef96-p115">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="7ef96-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="7ef96-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ef96-184">Response</span></span>
<span data-ttu-id="7ef96-185">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ef96-185">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="7ef96-186">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="7ef96-186">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="7ef96-187">Пример</span><span class="sxs-lookup"><span data-stu-id="7ef96-187">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="7ef96-188">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="7ef96-188">Request 1</span></span>
<span data-ttu-id="7ef96-189">Первый пример запроса создает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="7ef96-189">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
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

#### <a name="response"></a><span data-ttu-id="7ef96-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ef96-190">Response</span></span>
<span data-ttu-id="7ef96-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ef96-191">The following is an example of the response.</span></span>
><span data-ttu-id="7ef96-192">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7ef96-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ef96-193">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ef96-193">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="7ef96-194">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="7ef96-194">Request 2</span></span>
<span data-ttu-id="7ef96-195">Второй пример запроса создает группу Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="7ef96-195">The second example request creates an Office 365 group with an owner specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
```http
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

#### <a name="response-2"></a><span data-ttu-id="7ef96-196">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="7ef96-196">Response 2</span></span>
<span data-ttu-id="7ef96-197">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="7ef96-197">The following is an example of a successful response.</span></span> <span data-ttu-id="7ef96-198">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ef96-198">It includes only default properties.</span></span> <span data-ttu-id="7ef96-199">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="7ef96-199">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="7ef96-200">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7ef96-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ef96-201">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ef96-201">All the default properties are returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7ef96-202">См. также</span><span class="sxs-lookup"><span data-stu-id="7ef96-202">See also</span></span>

- [<span data-ttu-id="7ef96-203">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7ef96-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7ef96-204">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7ef96-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7ef96-205">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7ef96-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
