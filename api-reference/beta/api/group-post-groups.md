---
title: Создание группы
description: Создание группы Microsoft 365 или группы безопасности.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9099f0b6cbf3c0daabda9fbb67635f74a64ac19d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990804"
---
# <a name="create-group"></a><span data-ttu-id="9ce42-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="9ce42-103">Create group</span></span>

<span data-ttu-id="9ce42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ce42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ce42-105">Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="9ce42-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="9ce42-106">Можно создать одну из следующих групп:</span><span class="sxs-lookup"><span data-stu-id="9ce42-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="9ce42-107">Группа Microsoft 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="9ce42-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="9ce42-108">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="9ce42-108">Security group</span></span>

<span data-ttu-id="9ce42-109">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="9ce42-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="9ce42-110">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="9ce42-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="9ce42-111">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="9ce42-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="9ce42-112">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="9ce42-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ce42-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce42-113">Permissions</span></span>
<span data-ttu-id="9ce42-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ce42-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ce42-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ce42-116">Permission type</span></span>      | <span data-ttu-id="9ce42-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ce42-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ce42-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ce42-118">Delegated (work or school account)</span></span> | <span data-ttu-id="9ce42-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ce42-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="9ce42-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ce42-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ce42-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ce42-121">Not supported.</span></span>    |
|<span data-ttu-id="9ce42-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ce42-122">Application</span></span> | <span data-ttu-id="9ce42-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ce42-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ce42-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ce42-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="9ce42-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ce42-125">Request headers</span></span>

| <span data-ttu-id="9ce42-126">Имя</span><span class="sxs-lookup"><span data-stu-id="9ce42-126">Name</span></span>       | <span data-ttu-id="9ce42-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce42-127">Type</span></span> | <span data-ttu-id="9ce42-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce42-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ce42-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ce42-129">Authorization</span></span>  | <span data-ttu-id="9ce42-130">string</span><span class="sxs-lookup"><span data-stu-id="9ce42-130">string</span></span>  | <span data-ttu-id="9ce42-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce42-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ce42-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ce42-133">Request body</span></span>

<span data-ttu-id="9ce42-134">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="9ce42-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="9ce42-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ce42-135">Property</span></span> | <span data-ttu-id="9ce42-136">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce42-136">Type</span></span> | <span data-ttu-id="9ce42-137">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce42-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ce42-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9ce42-138">displayName</span></span> | <span data-ttu-id="9ce42-139">string</span><span class="sxs-lookup"><span data-stu-id="9ce42-139">string</span></span> | <span data-ttu-id="9ce42-140">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="9ce42-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="9ce42-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce42-141">Required.</span></span> |
| <span data-ttu-id="9ce42-142">description</span><span class="sxs-lookup"><span data-stu-id="9ce42-142">description</span></span> | <span data-ttu-id="9ce42-143">строка</span><span class="sxs-lookup"><span data-stu-id="9ce42-143">string</span></span> | <span data-ttu-id="9ce42-144">Описание группы.</span><span class="sxs-lookup"><span data-stu-id="9ce42-144">A description for the group.</span></span> <span data-ttu-id="9ce42-145">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ce42-145">Optional.</span></span> |
| <span data-ttu-id="9ce42-146">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="9ce42-146">isAssignableToRole</span></span> | <span data-ttu-id="9ce42-147">Логическое</span><span class="sxs-lookup"><span data-stu-id="9ce42-147">Boolean</span></span> | <span data-ttu-id="9ce42-148">Значение **true**, чтобы группу можно было назначить роли Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9ce42-148">Set to **true** to enable the group to be assigned to an Azure AD role.</span></span> <span data-ttu-id="9ce42-149">Только администратор привилегированных ролей и глобальный администратор может настроить значение этого свойства.</span><span class="sxs-lookup"><span data-stu-id="9ce42-149">Only Privileged Role Administrator and Global Administrator can set the value of this property.</span></span> <span data-ttu-id="9ce42-150">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ce42-150">Optional.</span></span> |
| <span data-ttu-id="9ce42-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="9ce42-151">mailEnabled</span></span> | <span data-ttu-id="9ce42-152">boolean</span><span class="sxs-lookup"><span data-stu-id="9ce42-152">boolean</span></span> | <span data-ttu-id="9ce42-153">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="9ce42-153">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="9ce42-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9ce42-154">Required.</span></span> |
| <span data-ttu-id="9ce42-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9ce42-155">mailNickname</span></span> | <span data-ttu-id="9ce42-156">string</span><span class="sxs-lookup"><span data-stu-id="9ce42-156">string</span></span> | <span data-ttu-id="9ce42-157">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="9ce42-157">The mail alias for the group.</span></span> <span data-ttu-id="9ce42-158">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce42-158">Required.</span></span> |
| <span data-ttu-id="9ce42-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="9ce42-159">securityEnabled</span></span> | <span data-ttu-id="9ce42-160">boolean</span><span class="sxs-lookup"><span data-stu-id="9ce42-160">boolean</span></span> | <span data-ttu-id="9ce42-161">Значение **true** для групп безопасности, включая группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ce42-161">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="9ce42-162">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ce42-162">Required.</span></span> |
| <span data-ttu-id="9ce42-163">owners</span><span class="sxs-lookup"><span data-stu-id="9ce42-163">owners</span></span> | <span data-ttu-id="9ce42-164">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9ce42-164">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="9ce42-165">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="9ce42-165">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="9ce42-166">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9ce42-166">Optional.</span></span> |
| <span data-ttu-id="9ce42-167">members</span><span class="sxs-lookup"><span data-stu-id="9ce42-167">members</span></span> | <span data-ttu-id="9ce42-168">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9ce42-168">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="9ce42-169">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="9ce42-169">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="9ce42-170">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ce42-170">Optional.</span></span> |
|<span data-ttu-id="9ce42-171">visibility</span><span class="sxs-lookup"><span data-stu-id="9ce42-171">visibility</span></span>|<span data-ttu-id="9ce42-172">String</span><span class="sxs-lookup"><span data-stu-id="9ce42-172">String</span></span>|<span data-ttu-id="9ce42-173">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ce42-173">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="9ce42-174">Возможные значения: `Private`, `Public`, `HiddenMembership` или пустое значение (обрабатывается как `Public`).</span><span class="sxs-lookup"><span data-stu-id="9ce42-174">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="9ce42-175">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="9ce42-175">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="9ce42-176">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к группе при ее создании.</span><span class="sxs-lookup"><span data-stu-id="9ce42-176">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="9ce42-177">**Примечание:** создание группы с помощью разрешения приложения Group.Create без указания владельцев анонимно создает группу, которая не будет изменяться.</span><span class="sxs-lookup"><span data-stu-id="9ce42-177">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="9ce42-178">Вы можете использовать операцию `POST` и добавить владельцев в группу при ее создании, чтобы указать владельцев, которые могут изменять группу.</span><span class="sxs-lookup"><span data-stu-id="9ce42-178">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="9ce42-179">Создание группы Microsoft 365 программным путем с контекстом только для приложений, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="9ce42-179">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="9ce42-180">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="9ce42-180">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="9ce42-181">При необходимости укажите другие записываемые свойства для своей группы.</span><span class="sxs-lookup"><span data-stu-id="9ce42-181">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="9ce42-182">Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="9ce42-182">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="9ce42-183">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="9ce42-183">groupTypes options</span></span>

<span data-ttu-id="9ce42-184">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9ce42-184">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="9ce42-185">Тип группы</span><span class="sxs-lookup"><span data-stu-id="9ce42-185">Type of group</span></span> | <span data-ttu-id="9ce42-186">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="9ce42-186">Assigned membership</span></span> | <span data-ttu-id="9ce42-187">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="9ce42-187">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="9ce42-188">Microsoft 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="9ce42-188">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="9ce42-189">Динамический</span><span class="sxs-lookup"><span data-stu-id="9ce42-189">Dynamic</span></span> | <span data-ttu-id="9ce42-190">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="9ce42-190">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="9ce42-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce42-191">Response</span></span>

<span data-ttu-id="9ce42-192">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce42-192">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="9ce42-193">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="9ce42-193">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="9ce42-194">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ce42-194">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="9ce42-195">Пример 1. Создание группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9ce42-195">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="9ce42-196">В следующем примере создается группа Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ce42-196">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="9ce42-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce42-197">Request</span></span>

<span data-ttu-id="9ce42-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ce42-198">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ce42-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ce42-199">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9ce42-200">C#</span><span class="sxs-lookup"><span data-stu-id="9ce42-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ce42-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ce42-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ce42-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ce42-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ce42-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce42-203">Response</span></span>

<span data-ttu-id="9ce42-204">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce42-204">The following is an example of the response.</span></span>

><span data-ttu-id="9ce42-205">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ce42-205">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ce42-206">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9ce42-206">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-a-microsoft-365-group-with-an-owner-and-members"></a><span data-ttu-id="9ce42-207">Пример 2. Создание группы Microsoft 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="9ce42-207">Example 2: Create a Microsoft 365 group with an owner and members</span></span>

<span data-ttu-id="9ce42-208">В следующем примере создается группа Microsoft 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="9ce42-208">The following example creates a Microsoft 365 group with an owner and members specified.</span></span> <span data-ttu-id="9ce42-209">Обратите внимание на то, что в рамках создания группы можно добавить не более 20 отношений, например владельцев и участников.</span><span class="sxs-lookup"><span data-stu-id="9ce42-209">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="9ce42-210">Позже вы можете добавить дополнительных участников с помощью API [добавления участников](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) или пакетной обработки JSON.</span><span class="sxs-lookup"><span data-stu-id="9ce42-210">You can subsequently add more members by using the [add member](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="9ce42-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce42-211">Request</span></span>

<span data-ttu-id="9ce42-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ce42-212">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ce42-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ce42-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9ce42-214">C#</span><span class="sxs-lookup"><span data-stu-id="9ce42-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ce42-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ce42-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ce42-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ce42-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ce42-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce42-217">Response</span></span> 

<span data-ttu-id="9ce42-218">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce42-218">The following is an example of a successful response.</span></span> <span data-ttu-id="9ce42-219">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9ce42-219">It includes only default properties.</span></span> <span data-ttu-id="9ce42-220">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="9ce42-220">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="9ce42-221">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ce42-221">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ce42-222">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9ce42-222">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="9ce42-223">Пример 3. Создание группы, которую можно назначить роли Azure AD</span><span class="sxs-lookup"><span data-stu-id="9ce42-223">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="9ce42-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ce42-224">Request</span></span>

<span data-ttu-id="9ce42-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ce42-225">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ce42-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ce42-226">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9ce42-227">C#</span><span class="sxs-lookup"><span data-stu-id="9ce42-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ce42-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ce42-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ce42-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ce42-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="9ce42-230">**Примечание.** Свойства **visibility** и **groupTypes** необязательны для создания, но заполняются автоматически этими значениями.</span><span class="sxs-lookup"><span data-stu-id="9ce42-230">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="9ce42-231">Группа, свойству **isAssignableToRole** которой присвоено значение `true`, не может относиться к типу с динамическим членством.</span><span class="sxs-lookup"><span data-stu-id="9ce42-231">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type.</span></span> <span data-ttu-id="9ce42-232">Дополнительные сведения см. в статье [Использование группы для управления назначениями ролей Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).</span><span class="sxs-lookup"><span data-stu-id="9ce42-232">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="9ce42-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ce42-233">Response</span></span>

<span data-ttu-id="9ce42-234">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ce42-234">The following is an example of the response.</span></span> <span data-ttu-id="9ce42-235">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9ce42-235">It includes only default properties.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9ce42-236">См. также</span><span class="sxs-lookup"><span data-stu-id="9ce42-236">See also</span></span>

- [<span data-ttu-id="9ce42-237">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9ce42-237">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9ce42-238">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9ce42-238">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9ce42-239">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9ce42-239">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


