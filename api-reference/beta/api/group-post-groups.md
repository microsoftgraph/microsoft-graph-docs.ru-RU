---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: de304cc4faaa6e4b64992ba0d7b2af35e8b5900a
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353071"
---
# <a name="create-group"></a><span data-ttu-id="ad8e5-104">Создание группы</span><span class="sxs-lookup"><span data-stu-id="ad8e5-104">Create group</span></span>

> <span data-ttu-id="ad8e5-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad8e5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad8e5-107">Используйте этот API, чтобы создать [группу](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-107">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span> <span data-ttu-id="ad8e5-108">Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="ad8e5-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="ad8e5-109">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="ad8e5-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="ad8e5-110">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="ad8e5-110">Dynamic group</span></span>
* <span data-ttu-id="ad8e5-111">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="ad8e5-111">Security group</span></span>

<span data-ttu-id="ad8e5-112">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-112">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="ad8e5-113">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="ad8e5-113">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="ad8e5-114">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-114">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="ad8e5-115">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="ad8e5-115">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="ad8e5-116">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="ad8e5-116">To create a **team**, first  [create group](../resources/team.md) and then [add a team to it](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad8e5-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad8e5-117">Permissions</span></span>
<span data-ttu-id="ad8e5-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad8e5-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad8e5-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad8e5-120">Permission type</span></span>      | <span data-ttu-id="ad8e5-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad8e5-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad8e5-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad8e5-122">Delegated (work or school account)</span></span> | <span data-ttu-id="ad8e5-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8e5-123">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad8e5-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad8e5-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad8e5-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-125">Not supported.</span></span>    |
|<span data-ttu-id="ad8e5-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad8e5-126">Application</span></span> | <span data-ttu-id="ad8e5-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8e5-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad8e5-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad8e5-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="ad8e5-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad8e5-129">Request headers</span></span>
| <span data-ttu-id="ad8e5-130">Имя</span><span class="sxs-lookup"><span data-stu-id="ad8e5-130">Name</span></span>       | <span data-ttu-id="ad8e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad8e5-131">Type</span></span> | <span data-ttu-id="ad8e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad8e5-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad8e5-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad8e5-133">Authorization</span></span>  | <span data-ttu-id="ad8e5-134">string</span><span class="sxs-lookup"><span data-stu-id="ad8e5-134">string</span></span>  | <span data-ttu-id="ad8e5-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad8e5-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad8e5-137">Request body</span></span>
<span data-ttu-id="ad8e5-138">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-138">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="ad8e5-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad8e5-139">Property</span></span> | <span data-ttu-id="ad8e5-140">Тип</span><span class="sxs-lookup"><span data-stu-id="ad8e5-140">Type</span></span> | <span data-ttu-id="ad8e5-141">Описание</span><span class="sxs-lookup"><span data-stu-id="ad8e5-141">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ad8e5-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ad8e5-142">displayName</span></span> | <span data-ttu-id="ad8e5-143">string</span><span class="sxs-lookup"><span data-stu-id="ad8e5-143">string</span></span> | <span data-ttu-id="ad8e5-144">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-144">The name to display in the address book for the group.</span></span> <span data-ttu-id="ad8e5-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-145">Required.</span></span> |
| <span data-ttu-id="ad8e5-146">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="ad8e5-146">mailEnabled</span></span> | <span data-ttu-id="ad8e5-147">boolean</span><span class="sxs-lookup"><span data-stu-id="ad8e5-147">boolean</span></span> | <span data-ttu-id="ad8e5-148">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-148">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="ad8e5-149">При создании группы Office 365 установите значение **true**.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-149">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="ad8e5-150">При создании динамической группы или группы безопасности установите для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-150">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="ad8e5-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-151">Required.</span></span> |
| <span data-ttu-id="ad8e5-152">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ad8e5-152">mailNickname</span></span> | <span data-ttu-id="ad8e5-153">string</span><span class="sxs-lookup"><span data-stu-id="ad8e5-153">string</span></span> | <span data-ttu-id="ad8e5-154">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-154">The mail alias for the group.</span></span> <span data-ttu-id="ad8e5-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-155">Required.</span></span> |
| <span data-ttu-id="ad8e5-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="ad8e5-156">securityEnabled</span></span> | <span data-ttu-id="ad8e5-157">boolean</span><span class="sxs-lookup"><span data-stu-id="ad8e5-157">boolean</span></span> | <span data-ttu-id="ad8e5-158">Установите значение **true** для защищенных групп.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-158">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="ad8e5-159">При создании динамической группы или группы безопасности установите для этого свойства значение **true**.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-159">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="ad8e5-160">При создании группы Office 365 установите значение **false**.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-160">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="ad8e5-161">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-161">Required.</span></span> |
| <span data-ttu-id="ad8e5-162">owners</span><span class="sxs-lookup"><span data-stu-id="ad8e5-162">owners</span></span> | <span data-ttu-id="ad8e5-163">string collection</span><span class="sxs-lookup"><span data-stu-id="ad8e5-163">string collection</span></span> | <span data-ttu-id="ad8e5-164">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-164">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="ad8e5-165">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-165">Optional.</span></span> |
| <span data-ttu-id="ad8e5-166">members</span><span class="sxs-lookup"><span data-stu-id="ad8e5-166">members</span></span> | <span data-ttu-id="ad8e5-167">string collection</span><span class="sxs-lookup"><span data-stu-id="ad8e5-167">string collection</span></span> | <span data-ttu-id="ad8e5-168">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-168">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="ad8e5-169">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-169">Optional.</span></span> |

<span data-ttu-id="ad8e5-170">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-170">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="ad8e5-171">Тип группы</span><span class="sxs-lookup"><span data-stu-id="ad8e5-171">Type of group</span></span> | <span data-ttu-id="ad8e5-172">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="ad8e5-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="ad8e5-173">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="ad8e5-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="ad8e5-174">"Unified"</span><span class="sxs-lookup"><span data-stu-id="ad8e5-174">"Unified"</span></span> |
| <span data-ttu-id="ad8e5-175">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="ad8e5-175">Dynamic</span></span> | <span data-ttu-id="ad8e5-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="ad8e5-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="ad8e5-177">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="ad8e5-177">Security</span></span> | <span data-ttu-id="ad8e5-178">Не следует устанавливать.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-178">Do not set.</span></span> |

<span data-ttu-id="ad8e5-179">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к событию при его создании.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-179">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

><span data-ttu-id="ad8e5-180">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-180">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="ad8e5-181">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="ad8e5-p115">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="ad8e5-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="ad8e5-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad8e5-184">Response</span></span>
<span data-ttu-id="ad8e5-185">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-185">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="ad8e5-186">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-186">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="ad8e5-187">Пример</span><span class="sxs-lookup"><span data-stu-id="ad8e5-187">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="ad8e5-188">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="ad8e5-188">Request 1</span></span>
<span data-ttu-id="ad8e5-189">Первый пример запроса создает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-189">The following is an example of a request that creates an Office 365 Group.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ad8e5-190">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad8e5-190">Response</span></span>
<span data-ttu-id="ad8e5-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-191">The following is an example of the response.</span></span>
><span data-ttu-id="ad8e5-192">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad8e5-193">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-193">All default properties are returned from the actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="ad8e5-194">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="ad8e5-194">Request 2</span></span>
<span data-ttu-id="ad8e5-195">Второй пример запроса создает группу Office 365 с указанным владельцем.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-195">The second example request creates an Office 365 group with an owner specified.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_with_owner"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a><span data-ttu-id="ad8e5-196">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="ad8e5-196">Response 2</span></span>
<span data-ttu-id="ad8e5-197">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-197">The following is an example of a response to a  event.</span></span> <span data-ttu-id="ad8e5-198">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-198">It includes only default properties.</span></span> <span data-ttu-id="ad8e5-199">Вы можете получить свойство навигации группы **owners**, чтобы проверить информацию о владельце.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-199">You can subsequenty get the **owners** navigation property of the group to verify the details of the owner.</span></span> 
><span data-ttu-id="ad8e5-200">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad8e5-201">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad8e5-201">All default properties are returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group_with_owner"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "502df398-d59c-469d-944f-34a50e60db3f",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-27T22:17:07Z",
     "description": "Group with designated owner",
     "displayName": "Operations group",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "operations2019@contoso.com",
     "mailEnabled": true,
     "mailNickname": "operations2019",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:operations2019@contoso.com"
     ],
     "renewedDateTime": "2018-12-27T22:17:07Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="ad8e5-202">См. также</span><span class="sxs-lookup"><span data-stu-id="ad8e5-202">See also</span></span>

- [<span data-ttu-id="ad8e5-203">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ad8e5-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ad8e5-204">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ad8e5-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ad8e5-205">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ad8e5-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
