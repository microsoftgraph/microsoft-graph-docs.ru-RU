---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 1ec6e4768e979f30cb0cb34de7555e08bf25b41f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324256"
---
# <a name="create-group"></a><span data-ttu-id="7c6e6-104">Создание группы</span><span class="sxs-lookup"><span data-stu-id="7c6e6-104">Create group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c6e6-p102">Используйте этот API, чтобы создать [группу](../resources/group.md) согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="7c6e6-p102">Use this API to create a new [group](../resources/group.md) as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="7c6e6-107">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="7c6e6-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="7c6e6-108">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="7c6e6-108">Dynamic group</span></span>
* <span data-ttu-id="7c6e6-109">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="7c6e6-109">Security group</span></span>

<span data-ttu-id="7c6e6-110">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="7c6e6-111">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="7c6e6-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="7c6e6-112">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="7c6e6-113">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="7c6e6-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="7c6e6-114">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="7c6e6-114">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c6e6-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c6e6-115">Permissions</span></span>
<span data-ttu-id="7c6e6-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c6e6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c6e6-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c6e6-118">Permission type</span></span>      | <span data-ttu-id="7c6e6-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c6e6-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c6e6-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c6e6-120">Delegated (work or school account)</span></span> | <span data-ttu-id="7c6e6-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c6e6-121">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c6e6-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c6e6-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c6e6-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-123">Not supported.</span></span>    |
|<span data-ttu-id="7c6e6-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c6e6-124">Application</span></span> | <span data-ttu-id="7c6e6-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c6e6-125">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c6e6-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c6e6-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7c6e6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c6e6-127">Request headers</span></span>
| <span data-ttu-id="7c6e6-128">Имя</span><span class="sxs-lookup"><span data-stu-id="7c6e6-128">Name</span></span>       | <span data-ttu-id="7c6e6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7c6e6-129">Type</span></span> | <span data-ttu-id="7c6e6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7c6e6-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c6e6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c6e6-131">Authorization</span></span>  | <span data-ttu-id="7c6e6-132">string</span><span class="sxs-lookup"><span data-stu-id="7c6e6-132">string</span></span>  | <span data-ttu-id="7c6e6-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c6e6-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c6e6-135">Request body</span></span>
<span data-ttu-id="7c6e6-136">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-136">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7c6e6-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c6e6-137">Property</span></span> | <span data-ttu-id="7c6e6-138">Тип</span><span class="sxs-lookup"><span data-stu-id="7c6e6-138">Type</span></span> | <span data-ttu-id="7c6e6-139">Описание</span><span class="sxs-lookup"><span data-stu-id="7c6e6-139">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c6e6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7c6e6-140">displayName</span></span> | <span data-ttu-id="7c6e6-141">string</span><span class="sxs-lookup"><span data-stu-id="7c6e6-141">string</span></span> | <span data-ttu-id="7c6e6-142">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-142">The name to display in the address book for the group.</span></span> <span data-ttu-id="7c6e6-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-143">Required.</span></span> |
| <span data-ttu-id="7c6e6-144">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7c6e6-144">mailEnabled</span></span> | <span data-ttu-id="7c6e6-145">boolean</span><span class="sxs-lookup"><span data-stu-id="7c6e6-145">boolean</span></span> | <span data-ttu-id="7c6e6-146">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-146">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="7c6e6-147">При создании группы Office 365 установите значение **true**.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-147">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="7c6e6-148">При создании динамической группы или группы безопасности установите для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-148">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="7c6e6-149">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-149">Required.</span></span> |
| <span data-ttu-id="7c6e6-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7c6e6-150">mailNickname</span></span> | <span data-ttu-id="7c6e6-151">string</span><span class="sxs-lookup"><span data-stu-id="7c6e6-151">string</span></span> | <span data-ttu-id="7c6e6-152">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-152">The mail alias for the group.</span></span> <span data-ttu-id="7c6e6-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-153">Required.</span></span> |
| <span data-ttu-id="7c6e6-154">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7c6e6-154">securityEnabled</span></span> | <span data-ttu-id="7c6e6-155">boolean</span><span class="sxs-lookup"><span data-stu-id="7c6e6-155">boolean</span></span> | <span data-ttu-id="7c6e6-156">Установите значение **true** для защищенных групп.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-156">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="7c6e6-157">При создании динамической группы или группы безопасности установите для этого свойства значение **true**.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-157">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="7c6e6-158">При создании группы Office 365 установите значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-158">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="7c6e6-159">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-159">Required.</span></span> |
| <span data-ttu-id="7c6e6-160">owners</span><span class="sxs-lookup"><span data-stu-id="7c6e6-160">owners</span></span> | <span data-ttu-id="7c6e6-161">string collection</span><span class="sxs-lookup"><span data-stu-id="7c6e6-161">string collection</span></span> | <span data-ttu-id="7c6e6-162">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-162">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="7c6e6-163">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-163">Optional.</span></span> |
| <span data-ttu-id="7c6e6-164">members</span><span class="sxs-lookup"><span data-stu-id="7c6e6-164">members</span></span> | <span data-ttu-id="7c6e6-165">string collection</span><span class="sxs-lookup"><span data-stu-id="7c6e6-165">string collection</span></span> | <span data-ttu-id="7c6e6-166">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-166">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="7c6e6-167">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-167">Optional.</span></span> |

<span data-ttu-id="7c6e6-168">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-168">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="7c6e6-169">Тип группы</span><span class="sxs-lookup"><span data-stu-id="7c6e6-169">Type of group</span></span> | <span data-ttu-id="7c6e6-170">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="7c6e6-170">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="7c6e6-171">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="7c6e6-171">Office 365 (aka unified group)</span></span>| <span data-ttu-id="7c6e6-172">"Unified"</span><span class="sxs-lookup"><span data-stu-id="7c6e6-172">"Unified"</span></span> |
| <span data-ttu-id="7c6e6-173">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="7c6e6-173">Dynamic</span></span> | <span data-ttu-id="7c6e6-174">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="7c6e6-174">"DynamicMembership"</span></span> |
| <span data-ttu-id="7c6e6-175">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="7c6e6-175">Security</span></span> | <span data-ttu-id="7c6e6-176">Не следует устанавливать.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-176">Do not set.</span></span> |

<span data-ttu-id="7c6e6-177">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-177">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="7c6e6-178">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-178">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="7c6e6-179">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-179">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7c6e6-p114">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="7c6e6-p114">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="7c6e6-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c6e6-182">Response</span></span>
<span data-ttu-id="7c6e6-183">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-183">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="7c6e6-184">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-184">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="7c6e6-185">Пример</span><span class="sxs-lookup"><span data-stu-id="7c6e6-185">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="7c6e6-186">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="7c6e6-186">Request 1</span></span>
<span data-ttu-id="7c6e6-187">Первый пример запроса создает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-187">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response"></a><span data-ttu-id="7c6e6-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c6e6-188">Response</span></span>
<span data-ttu-id="7c6e6-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-189">The following is an example of the response.</span></span>
><span data-ttu-id="7c6e6-190">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-190">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7c6e6-191">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-191">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="7c6e6-192">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="7c6e6-192">Request 2</span></span>
<span data-ttu-id="7c6e6-193">Второй пример запроса создает группу Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-193">The second example request creates an Office 365 group with an owner and members specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="7c6e6-194">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="7c6e6-194">Response 2</span></span>
<span data-ttu-id="7c6e6-195">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-195">The following is an example of a successful response.</span></span> <span data-ttu-id="7c6e6-196">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-196">It includes only default properties.</span></span> <span data-ttu-id="7c6e6-197">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-197">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="7c6e6-198">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-198">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7c6e6-199">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7c6e6-199">All the default properties are returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7c6e6-200">См. также</span><span class="sxs-lookup"><span data-stu-id="7c6e6-200">See also</span></span>

- [<span data-ttu-id="7c6e6-201">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7c6e6-201">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7c6e6-202">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7c6e6-202">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7c6e6-203">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7c6e6-203">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
