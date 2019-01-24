---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: bc83ccc3c32dbde12b93c1d22eb7640e4e72fcb8
ms.sourcegitcommit: 71368f59d267c8188567529e74486e54cc122804
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29442320"
---
# <a name="create-group"></a><span data-ttu-id="3fff4-104">Создание группы</span><span class="sxs-lookup"><span data-stu-id="3fff4-104">Create group</span></span>
<span data-ttu-id="3fff4-p102">Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="3fff4-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="3fff4-107">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="3fff4-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="3fff4-108">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="3fff4-108">Dynamic group</span></span>
* <span data-ttu-id="3fff4-109">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="3fff4-109">Security group</span></span>

<span data-ttu-id="3fff4-110">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="3fff4-110">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="3fff4-111">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="3fff4-111">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="3fff4-112">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните операцию GET и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="3fff4-112">To get properties that are _not_ returned by default, do a GET operation and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="3fff4-113">См. [пример](group-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="3fff4-113">See an [example](group-get.md#request-2).</span></span>

> <span data-ttu-id="3fff4-p105">**Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3fff4-p105">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fff4-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fff4-116">Permissions</span></span>
<span data-ttu-id="3fff4-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fff4-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fff4-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fff4-119">Permission type</span></span>      | <span data-ttu-id="3fff4-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fff4-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fff4-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fff4-121">Delegated (work or school account)</span></span> | <span data-ttu-id="3fff4-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fff4-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3fff4-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fff4-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fff4-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fff4-124">Not supported.</span></span>    |
|<span data-ttu-id="3fff4-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fff4-125">Application</span></span> | <span data-ttu-id="3fff4-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fff4-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fff4-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fff4-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="3fff4-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fff4-128">Request headers</span></span>
| <span data-ttu-id="3fff4-129">Имя</span><span class="sxs-lookup"><span data-stu-id="3fff4-129">Name</span></span>       | <span data-ttu-id="3fff4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3fff4-130">Type</span></span> | <span data-ttu-id="3fff4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3fff4-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3fff4-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fff4-132">Authorization</span></span>  | <span data-ttu-id="3fff4-133">string</span><span class="sxs-lookup"><span data-stu-id="3fff4-133">string</span></span>  | <span data-ttu-id="3fff4-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fff4-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fff4-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fff4-136">Request body</span></span>
<span data-ttu-id="3fff4-137">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="3fff4-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="3fff4-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fff4-138">Property</span></span> | <span data-ttu-id="3fff4-139">Тип</span><span class="sxs-lookup"><span data-stu-id="3fff4-139">Type</span></span> | <span data-ttu-id="3fff4-140">Описание</span><span class="sxs-lookup"><span data-stu-id="3fff4-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3fff4-141">displayName</span><span class="sxs-lookup"><span data-stu-id="3fff4-141">displayName</span></span> | <span data-ttu-id="3fff4-142">string</span><span class="sxs-lookup"><span data-stu-id="3fff4-142">string</span></span> | <span data-ttu-id="3fff4-143">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="3fff4-143">The name to display in the address book for the group.</span></span> <span data-ttu-id="3fff4-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fff4-144">Required.</span></span> |
| <span data-ttu-id="3fff4-145">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="3fff4-145">mailEnabled</span></span> | <span data-ttu-id="3fff4-146">boolean</span><span class="sxs-lookup"><span data-stu-id="3fff4-146">boolean</span></span> | <span data-ttu-id="3fff4-147">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="3fff4-147">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="3fff4-148">При создании группы Office 365 установите значение **true**.</span><span class="sxs-lookup"><span data-stu-id="3fff4-148">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="3fff4-149">При создании динамической группы или группы безопасности установите для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="3fff4-149">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="3fff4-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fff4-150">Required.</span></span> |
| <span data-ttu-id="3fff4-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3fff4-151">mailNickname</span></span> | <span data-ttu-id="3fff4-152">string</span><span class="sxs-lookup"><span data-stu-id="3fff4-152">string</span></span> | <span data-ttu-id="3fff4-153">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="3fff4-153">The mail alias for the group.</span></span> <span data-ttu-id="3fff4-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fff4-154">Required.</span></span> |
| <span data-ttu-id="3fff4-155">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="3fff4-155">securityEnabled</span></span> | <span data-ttu-id="3fff4-156">boolean</span><span class="sxs-lookup"><span data-stu-id="3fff4-156">boolean</span></span> | <span data-ttu-id="3fff4-157">Установите значение **true** для защищенных групп.</span><span class="sxs-lookup"><span data-stu-id="3fff4-157">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="3fff4-158">При создании динамической группы или группы безопасности установите для этого свойства значение **true**.</span><span class="sxs-lookup"><span data-stu-id="3fff4-158">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="3fff4-159">Установите значение **false** при создании группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="3fff4-159">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="3fff4-160">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fff4-160">Required.</span></span> |
| <span data-ttu-id="3fff4-161">owners</span><span class="sxs-lookup"><span data-stu-id="3fff4-161">owners</span></span> | <span data-ttu-id="3fff4-162">string collection</span><span class="sxs-lookup"><span data-stu-id="3fff4-162">string collection</span></span> | <span data-ttu-id="3fff4-163">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="3fff4-163">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="3fff4-164">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3fff4-164">Optional.</span></span> |
| <span data-ttu-id="3fff4-165">members</span><span class="sxs-lookup"><span data-stu-id="3fff4-165">members</span></span> | <span data-ttu-id="3fff4-166">string collection</span><span class="sxs-lookup"><span data-stu-id="3fff4-166">string collection</span></span> | <span data-ttu-id="3fff4-167">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="3fff4-167">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="3fff4-168">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3fff4-168">Optional.</span></span> |


<span data-ttu-id="3fff4-169">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="3fff4-169">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="3fff4-170">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="3fff4-170">groupTypes options</span></span>

| <span data-ttu-id="3fff4-171">Тип группы</span><span class="sxs-lookup"><span data-stu-id="3fff4-171">Type of group</span></span> | <span data-ttu-id="3fff4-172">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="3fff4-172">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="3fff4-173">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="3fff4-173">Office 365 (aka unified group)</span></span>| <span data-ttu-id="3fff4-174">"Unified"</span><span class="sxs-lookup"><span data-stu-id="3fff4-174">"Unified"</span></span> |
| <span data-ttu-id="3fff4-175">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="3fff4-175">Dynamic</span></span> | <span data-ttu-id="3fff4-176">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="3fff4-176">"DynamicMembership"</span></span> |
| <span data-ttu-id="3fff4-177">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="3fff4-177">Security</span></span> | <span data-ttu-id="3fff4-178">Не задавайте.</span><span class="sxs-lookup"><span data-stu-id="3fff4-178">Do not set.</span></span> |


><span data-ttu-id="3fff4-179">**Примечание.** Создание группы Office 365 программным путем без пользовательского контекста, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="3fff4-179">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="3fff4-180">Это может привести к тому, что связанный с ней сайт SharePoint Online, не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="3fff4-180">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="3fff4-p115">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="3fff4-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="3fff4-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fff4-183">Response</span></span>
<span data-ttu-id="3fff4-184">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3fff4-184">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="3fff4-185">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="3fff4-185">The response includes only the default properties of the group.</span></span>

## <a name="example"></a><span data-ttu-id="3fff4-186">Пример</span><span class="sxs-lookup"><span data-stu-id="3fff4-186">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="3fff4-187">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="3fff4-187">Request 1</span></span>
<span data-ttu-id="3fff4-188">Первый пример запроса создает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="3fff4-188">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="3fff4-189">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="3fff4-189">Response 1</span></span>
<span data-ttu-id="3fff4-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3fff4-190">The following is an example of the response.</span></span>
><span data-ttu-id="3fff4-191">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3fff4-191">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3fff4-192">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3fff4-192">All the default properties are returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="3fff4-193">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="3fff4-193">Request 2</span></span>
<span data-ttu-id="3fff4-194">Второй пример запроса создает группу Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="3fff4-194">The second example request creates an Office 365 group with an owner specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="3fff4-195">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="3fff4-195">Response 2</span></span>
<span data-ttu-id="3fff4-196">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="3fff4-196">The following is an example of a successful response.</span></span> <span data-ttu-id="3fff4-197">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3fff4-197">It includes only default properties.</span></span> <span data-ttu-id="3fff4-198">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="3fff4-198">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 
><span data-ttu-id="3fff4-199">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3fff4-199">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3fff4-200">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3fff4-200">All the default properties are returned from an actual call.</span></span>
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
