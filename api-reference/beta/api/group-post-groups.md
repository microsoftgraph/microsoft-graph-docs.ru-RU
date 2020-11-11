---
title: Создание группы
description: Создание группы Microsoft 365 или группы безопасности.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 570b3a138e593586d55016f6640c68ddeeb188ce
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953829"
---
# <a name="create-group"></a><span data-ttu-id="7fc39-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="7fc39-103">Create group</span></span>

<span data-ttu-id="7fc39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fc39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fc39-p101">Создайте новую [группу](../resources/group.md) согласно инструкциям в тексте запроса. Можно создать одну из следующих групп.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p101">Create a new [group](../resources/group.md) as specified in the request body. You can create one of the following groups:</span></span>

* <span data-ttu-id="7fc39-107">Группа Microsoft 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="7fc39-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="7fc39-108">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="7fc39-108">Security group</span></span>

<span data-ttu-id="7fc39-p102">Эта операция возвращает по умолчанию только подмножество свойств для каждой группы. Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties). Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите свойства в параметре запроса `$select` OData.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p102">This operation returns by default only a subset of the properties for each group. These default properties are noted in the [Properties](../resources/group.md#properties) section. To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="7fc39-112">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу, а затем добавьте в нее команду. См. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="7fc39-112">**Note** : To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7fc39-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc39-113">Permissions</span></span>
<span data-ttu-id="7fc39-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fc39-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fc39-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc39-116">Permission type</span></span>      | <span data-ttu-id="7fc39-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fc39-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fc39-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fc39-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7fc39-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7fc39-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="7fc39-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fc39-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fc39-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc39-121">Not supported.</span></span>    |
|<span data-ttu-id="7fc39-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="7fc39-122">Application</span></span> | <span data-ttu-id="7fc39-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc39-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fc39-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fc39-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7fc39-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fc39-125">Request headers</span></span>

| <span data-ttu-id="7fc39-126">Имя</span><span class="sxs-lookup"><span data-stu-id="7fc39-126">Name</span></span>       | <span data-ttu-id="7fc39-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7fc39-127">Type</span></span> | <span data-ttu-id="7fc39-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7fc39-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7fc39-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fc39-129">Authorization</span></span>  | <span data-ttu-id="7fc39-130">string</span><span class="sxs-lookup"><span data-stu-id="7fc39-130">string</span></span>  | <span data-ttu-id="7fc39-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fc39-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fc39-133">Request body</span></span>

<span data-ttu-id="7fc39-134">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="7fc39-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7fc39-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fc39-135">Property</span></span> | <span data-ttu-id="7fc39-136">Тип</span><span class="sxs-lookup"><span data-stu-id="7fc39-136">Type</span></span> | <span data-ttu-id="7fc39-137">Описание</span><span class="sxs-lookup"><span data-stu-id="7fc39-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7fc39-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7fc39-138">displayName</span></span> | <span data-ttu-id="7fc39-139">строка</span><span class="sxs-lookup"><span data-stu-id="7fc39-139">string</span></span> | <span data-ttu-id="7fc39-p105">Имя, которое следует отобразить в адресной книге для группы. Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p105">The name to display in the address book for the group. Required.</span></span> |
| <span data-ttu-id="7fc39-142">описание</span><span class="sxs-lookup"><span data-stu-id="7fc39-142">description</span></span> | <span data-ttu-id="7fc39-143">строка</span><span class="sxs-lookup"><span data-stu-id="7fc39-143">string</span></span> | <span data-ttu-id="7fc39-p106">Описание для группы. Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p106">A description for the group. Optional.</span></span> |
| <span data-ttu-id="7fc39-146">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="7fc39-146">isAssignableToRole</span></span> | <span data-ttu-id="7fc39-147">Логический</span><span class="sxs-lookup"><span data-stu-id="7fc39-147">Boolean</span></span> | <span data-ttu-id="7fc39-p107">Установите значение **true** , чтобы группе можно было назначить роль Azure AD. Только администратор привилегированных ролей и глобальный администратор может устанавливать значение этого свойства. Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p107">Set to **true** to enable the group to be assigned to an Azure AD role. Only Privileged Role Administrator and Global Administrator can set the value of this property. Optional.</span></span> |
| <span data-ttu-id="7fc39-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7fc39-151">mailEnabled</span></span> | <span data-ttu-id="7fc39-152">логический</span><span class="sxs-lookup"><span data-stu-id="7fc39-152">boolean</span></span> | <span data-ttu-id="7fc39-p108">Установите значение **true** для групп, поддерживающих почту. Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p108">Set to **true** for mail-enabled groups. Required.</span></span> |
| <span data-ttu-id="7fc39-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7fc39-155">mailNickname</span></span> | <span data-ttu-id="7fc39-156">строка</span><span class="sxs-lookup"><span data-stu-id="7fc39-156">string</span></span> | <span data-ttu-id="7fc39-p109">Почтовый псевдоним для группы. Символы, которые нельзя использовать в mailNickName: `@()\[]";:.<>,SPACE`. Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p109">The mail alias for the group. These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`. Required.</span></span> |
| <span data-ttu-id="7fc39-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7fc39-160">securityEnabled</span></span> | <span data-ttu-id="7fc39-161">логический</span><span class="sxs-lookup"><span data-stu-id="7fc39-161">boolean</span></span> | <span data-ttu-id="7fc39-p110">Установите значение **true** для защищенных групп, включая группы Microsoft 365. Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p110">Set to **true** for security-enabled groups, including Microsoft 365 groups. Required.</span></span> |
| <span data-ttu-id="7fc39-164">owners</span><span class="sxs-lookup"><span data-stu-id="7fc39-164">owners</span></span> | <span data-ttu-id="7fc39-165">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7fc39-165">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="7fc39-p111">Это свойство представляет владельцев группы на момент создания. Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p111">This property represents the owners for the group at creation time. Optional.</span></span> |
| <span data-ttu-id="7fc39-168">members</span><span class="sxs-lookup"><span data-stu-id="7fc39-168">members</span></span> | <span data-ttu-id="7fc39-169">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7fc39-169">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="7fc39-p112">Это свойство представляет участников группы на момент создания. Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p112">This property represents the members for the group at creation time. Optional.</span></span> |
|<span data-ttu-id="7fc39-172">visibility</span><span class="sxs-lookup"><span data-stu-id="7fc39-172">visibility</span></span>|<span data-ttu-id="7fc39-173">Строка</span><span class="sxs-lookup"><span data-stu-id="7fc39-173">String</span></span>|<span data-ttu-id="7fc39-p113">Определяет видимость группы Microsoft 365. Возможные значения: `Private`, `Public`, `HiddenMembership` или пустое значение (обрабатывается как `Public`).</span><span class="sxs-lookup"><span data-stu-id="7fc39-p113">Specifies the visibility of a Microsoft 365 group. Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="7fc39-176">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="7fc39-176">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="7fc39-177">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), можно использовать операцию `POST`, чтобы добавить настраиваемые свойства с собственными данными к группе при ее создании.</span><span class="sxs-lookup"><span data-stu-id="7fc39-177">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="7fc39-p114">**Примечание.** Создание группы с помощью разрешения приложения Group.Create без указания владельцев приведет к анонимному созданию группы, которую нельзя изменять. Можно использовать операцию `POST` и добавить владельцев для группы при ее создании, чтобы определить владельцев, имеющих право изменять группу.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p114">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable. You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="7fc39-p115">Создание группы Microsoft 365 программным путем с контекстом только для приложений и без указания владельцев будет анонимным. Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p115">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously. Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7fc39-p116">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="7fc39-p116">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="7fc39-184">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="7fc39-184">groupTypes options</span></span>

<span data-ttu-id="7fc39-185">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="7fc39-185">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="7fc39-186">Тип группы</span><span class="sxs-lookup"><span data-stu-id="7fc39-186">Type of group</span></span> | <span data-ttu-id="7fc39-187">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="7fc39-187">Assigned membership</span></span> | <span data-ttu-id="7fc39-188">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="7fc39-188">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="7fc39-189">Microsoft 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="7fc39-189">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="7fc39-190">Динамический</span><span class="sxs-lookup"><span data-stu-id="7fc39-190">Dynamic</span></span> | <span data-ttu-id="7fc39-191">`[]` ( _null_ )</span><span class="sxs-lookup"><span data-stu-id="7fc39-191">`[]` ( _null_ )</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="7fc39-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc39-192">Response</span></span>

<span data-ttu-id="7fc39-p117">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в тексте отклика. Отклик включает в себя только свойства группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7fc39-p117">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body. The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="7fc39-195">Примеры</span><span class="sxs-lookup"><span data-stu-id="7fc39-195">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="7fc39-196">Пример 1. Создание группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7fc39-196">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="7fc39-197">В следующем примере создается группа Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7fc39-197">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="7fc39-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fc39-198">Request</span></span>

<span data-ttu-id="7fc39-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fc39-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fc39-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fc39-200">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7fc39-201">C#</span><span class="sxs-lookup"><span data-stu-id="7fc39-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fc39-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fc39-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fc39-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fc39-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fc39-204">Java</span><span class="sxs-lookup"><span data-stu-id="7fc39-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7fc39-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc39-205">Response</span></span>

<span data-ttu-id="7fc39-206">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7fc39-206">The following is an example of the response.</span></span>

><span data-ttu-id="7fc39-207">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7fc39-207">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7fc39-208">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7fc39-208">All the default properties are returned from an actual call.</span></span>

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
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
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
   "isAssignableToRole": null,
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
   "securityIdentifier": "S-1-12-1-1753967289-1089268234-832641959-555555555",
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-a-microsoft-365-group-with-an-owner-and-members"></a><span data-ttu-id="7fc39-209">Пример 2. Создание группы Microsoft 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="7fc39-209">Example 2: Create a Microsoft 365 group with an owner and members</span></span>

<span data-ttu-id="7fc39-210">В следующем примере создается группа Microsoft 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="7fc39-210">The following example creates a Microsoft 365 group with an owner and members specified.</span></span> <span data-ttu-id="7fc39-211">Обратите внимание на то, что в рамках создания группы можно добавить не более 20 отношений, например владельцев и участников.</span><span class="sxs-lookup"><span data-stu-id="7fc39-211">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="7fc39-212">Позже вы можете добавить дополнительных участников с помощью API [добавления участников](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) или пакетной обработки JSON.</span><span class="sxs-lookup"><span data-stu-id="7fc39-212">You can subsequently add more members by using the [add member](/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="7fc39-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fc39-213">Request</span></span>

<span data-ttu-id="7fc39-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fc39-214">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
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

#### <a name="response"></a><span data-ttu-id="7fc39-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc39-215">Response</span></span> 

<span data-ttu-id="7fc39-216">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="7fc39-216">The following is an example of a successful response.</span></span> <span data-ttu-id="7fc39-217">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7fc39-217">It includes only default properties.</span></span> <span data-ttu-id="7fc39-218">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="7fc39-218">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="7fc39-219">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7fc39-219">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7fc39-220">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7fc39-220">All the default properties are returned from an actual call.</span></span>

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
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "expirationDateTime": null,
    "groupTypes": [
        "Unified"
    ],
    "isAssignableToRole": null,
    "mail": "operations2019@contoso.com",
    "mailEnabled": true,
    "mailNickname": "operations2019",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
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
    "securityIdentifier": "S-1-12-1-1905728287-1207447622-870010782-555555555",
    "theme": null,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="7fc39-221">Пример 3. Создание группы, которую можно назначить роли Azure AD</span><span class="sxs-lookup"><span data-stu-id="7fc39-221">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="7fc39-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fc39-222">Request</span></span>

<span data-ttu-id="7fc39-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fc39-223">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7fc39-224">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fc39-224">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group assignable to a role",
  "displayName": "Role assignable group",
  "groupTypes": [
    "Unified"
  ],
  "isAssignableToRole": true,
  "mailEnabled": true,
  "securityEnabled": true,
  "mailNickname": "contosohelpdeskadministrators",
  "visibility" : "Private"
}
```
# <a name="c"></a>[<span data-ttu-id="7fc39-225">C#</span><span class="sxs-lookup"><span data-stu-id="7fc39-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fc39-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fc39-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fc39-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fc39-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fc39-228">Java</span><span class="sxs-lookup"><span data-stu-id="7fc39-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="7fc39-229">**Примечание.** Свойства **visibility** и **groupTypes** необязательны для создания, но заполняются автоматически этими значениями.</span><span class="sxs-lookup"><span data-stu-id="7fc39-229">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="7fc39-230">Группа, свойству **isAssignableToRole** которой присвоено значение `true`, не может относиться к типу с динамическим членством.</span><span class="sxs-lookup"><span data-stu-id="7fc39-230">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type.</span></span> <span data-ttu-id="7fc39-231">Дополнительные сведения см. в статье [Использование группы для управления назначениями ролей Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).</span><span class="sxs-lookup"><span data-stu-id="7fc39-231">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="7fc39-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc39-232">Response</span></span>

<span data-ttu-id="7fc39-233">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7fc39-233">The following is an example of the response.</span></span> <span data-ttu-id="7fc39-234">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7fc39-234">It includes only default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_role_enabled_group"
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
  "description": "Group assignable to a role",
  "displayName": "Role assignable group",
  "expirationDateTime": null,
  "groupTypes": [
    "Unified"
  ],
  "isAssignableToRole": true,
  "mail": "operations2019@contoso.com",
  "mailEnabled": true,
  "mailNickname": "contosohelpdeskadministrators",
  "membershipRule": null,
  "membershipRuleProcessingState": null,
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
  "securityEnabled": true,
  "securityIdentifier": "S-1-12-1-1905728287-1207447622-870010782-555555555",
  "theme": null,
  "visibility": "Private",
  "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a><span data-ttu-id="7fc39-235">См. также</span><span class="sxs-lookup"><span data-stu-id="7fc39-235">See also</span></span>

- [<span data-ttu-id="7fc39-236">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7fc39-236">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7fc39-237">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7fc39-237">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7fc39-238">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7fc39-238">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


