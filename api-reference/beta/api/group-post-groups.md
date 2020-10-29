---
title: Создание группы
description: Создание группы Microsoft 365 или группы безопасности.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ef62655e2d31734a466404402ac808c66aace324
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782832"
---
# <a name="create-group"></a><span data-ttu-id="562e9-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="562e9-103">Create group</span></span>

<span data-ttu-id="562e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="562e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="562e9-105">Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="562e9-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="562e9-106">Можно создать одну из следующих групп:</span><span class="sxs-lookup"><span data-stu-id="562e9-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="562e9-107">Группа Microsoft 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="562e9-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="562e9-108">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="562e9-108">Security group</span></span>

<span data-ttu-id="562e9-109">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="562e9-110">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="562e9-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="562e9-111">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="562e9-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="562e9-112">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-112">**Note** : To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="562e9-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="562e9-113">Permissions</span></span>
<span data-ttu-id="562e9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="562e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="562e9-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="562e9-116">Permission type</span></span>      | <span data-ttu-id="562e9-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="562e9-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="562e9-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="562e9-118">Delegated (work or school account)</span></span> | <span data-ttu-id="562e9-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="562e9-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="562e9-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="562e9-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="562e9-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="562e9-121">Not supported.</span></span>    |
|<span data-ttu-id="562e9-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="562e9-122">Application</span></span> | <span data-ttu-id="562e9-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="562e9-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="562e9-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="562e9-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="562e9-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="562e9-125">Request headers</span></span>

| <span data-ttu-id="562e9-126">Имя</span><span class="sxs-lookup"><span data-stu-id="562e9-126">Name</span></span>       | <span data-ttu-id="562e9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="562e9-127">Type</span></span> | <span data-ttu-id="562e9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="562e9-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="562e9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="562e9-129">Authorization</span></span>  | <span data-ttu-id="562e9-130">string</span><span class="sxs-lookup"><span data-stu-id="562e9-130">string</span></span>  | <span data-ttu-id="562e9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="562e9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="562e9-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="562e9-133">Request body</span></span>

<span data-ttu-id="562e9-134">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="562e9-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="562e9-135">Property</span></span> | <span data-ttu-id="562e9-136">Тип</span><span class="sxs-lookup"><span data-stu-id="562e9-136">Type</span></span> | <span data-ttu-id="562e9-137">Описание</span><span class="sxs-lookup"><span data-stu-id="562e9-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="562e9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="562e9-138">displayName</span></span> | <span data-ttu-id="562e9-139">string</span><span class="sxs-lookup"><span data-stu-id="562e9-139">string</span></span> | <span data-ttu-id="562e9-140">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="562e9-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="562e9-141">Required.</span></span> |
| <span data-ttu-id="562e9-142">description</span><span class="sxs-lookup"><span data-stu-id="562e9-142">description</span></span> | <span data-ttu-id="562e9-143">строка</span><span class="sxs-lookup"><span data-stu-id="562e9-143">string</span></span> | <span data-ttu-id="562e9-144">Описание группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-144">A description for the group.</span></span> <span data-ttu-id="562e9-145">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="562e9-145">Optional.</span></span> |
| <span data-ttu-id="562e9-146">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="562e9-146">isAssignableToRole</span></span> | <span data-ttu-id="562e9-147">Логическое</span><span class="sxs-lookup"><span data-stu-id="562e9-147">Boolean</span></span> | <span data-ttu-id="562e9-148">Значение **true** , чтобы группу можно было назначить роли Azure AD.</span><span class="sxs-lookup"><span data-stu-id="562e9-148">Set to **true** to enable the group to be assigned to an Azure AD role.</span></span> <span data-ttu-id="562e9-149">Только администратор привилегированных ролей и глобальный администратор может настроить значение этого свойства.</span><span class="sxs-lookup"><span data-stu-id="562e9-149">Only Privileged Role Administrator and Global Administrator can set the value of this property.</span></span> <span data-ttu-id="562e9-150">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="562e9-150">Optional.</span></span> |
| <span data-ttu-id="562e9-151">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="562e9-151">mailEnabled</span></span> | <span data-ttu-id="562e9-152">boolean</span><span class="sxs-lookup"><span data-stu-id="562e9-152">boolean</span></span> | <span data-ttu-id="562e9-153">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="562e9-153">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="562e9-154">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="562e9-154">Required.</span></span> |
| <span data-ttu-id="562e9-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="562e9-155">mailNickname</span></span> | <span data-ttu-id="562e9-156">string</span><span class="sxs-lookup"><span data-stu-id="562e9-156">string</span></span> | <span data-ttu-id="562e9-157">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-157">The mail alias for the group.</span></span> <span data-ttu-id="562e9-158">Такие символы нельзя использовать в mailNickName: `@()\[]";:.<>,SPACE`.</span><span class="sxs-lookup"><span data-stu-id="562e9-158">These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`.</span></span> <span data-ttu-id="562e9-159">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="562e9-159">Required.</span></span> |
| <span data-ttu-id="562e9-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="562e9-160">securityEnabled</span></span> | <span data-ttu-id="562e9-161">boolean</span><span class="sxs-lookup"><span data-stu-id="562e9-161">boolean</span></span> | <span data-ttu-id="562e9-162">Значение **true** для групп безопасности, включая группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="562e9-162">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="562e9-163">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="562e9-163">Required.</span></span> |
| <span data-ttu-id="562e9-164">owners</span><span class="sxs-lookup"><span data-stu-id="562e9-164">owners</span></span> | <span data-ttu-id="562e9-165">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="562e9-165">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="562e9-166">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="562e9-166">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="562e9-167">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="562e9-167">Optional.</span></span> |
| <span data-ttu-id="562e9-168">members</span><span class="sxs-lookup"><span data-stu-id="562e9-168">members</span></span> | <span data-ttu-id="562e9-169">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="562e9-169">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="562e9-170">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="562e9-170">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="562e9-171">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="562e9-171">Optional.</span></span> |
|<span data-ttu-id="562e9-172">visibility</span><span class="sxs-lookup"><span data-stu-id="562e9-172">visibility</span></span>|<span data-ttu-id="562e9-173">String</span><span class="sxs-lookup"><span data-stu-id="562e9-173">String</span></span>|<span data-ttu-id="562e9-174">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="562e9-174">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="562e9-175">Возможные значения: `Private`, `Public`, `HiddenMembership` или пустое значение (обрабатывается как `Public`).</span><span class="sxs-lookup"><span data-stu-id="562e9-175">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="562e9-176">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="562e9-176">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="562e9-177">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к группе при ее создании.</span><span class="sxs-lookup"><span data-stu-id="562e9-177">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="562e9-178">**Примечание:** создание группы с помощью разрешения приложения Group.Create без указания владельцев анонимно создает группу, которая не будет изменяться.</span><span class="sxs-lookup"><span data-stu-id="562e9-178">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="562e9-179">Вы можете использовать операцию `POST` и добавить владельцев в группу при ее создании, чтобы указать владельцев, которые могут изменять группу.</span><span class="sxs-lookup"><span data-stu-id="562e9-179">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="562e9-180">Создание группы Microsoft 365 программным путем с контекстом только для приложений, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="562e9-180">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="562e9-181">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="562e9-181">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="562e9-182">При необходимости укажите другие записываемые свойства для своей группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-182">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="562e9-183">Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="562e9-183">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="562e9-184">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="562e9-184">groupTypes options</span></span>

<span data-ttu-id="562e9-185">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="562e9-185">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="562e9-186">Тип группы</span><span class="sxs-lookup"><span data-stu-id="562e9-186">Type of group</span></span> | <span data-ttu-id="562e9-187">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="562e9-187">Assigned membership</span></span> | <span data-ttu-id="562e9-188">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="562e9-188">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="562e9-189">Microsoft 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="562e9-189">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="562e9-190">Динамический</span><span class="sxs-lookup"><span data-stu-id="562e9-190">Dynamic</span></span> | <span data-ttu-id="562e9-191">`[]` ( _null_ )</span><span class="sxs-lookup"><span data-stu-id="562e9-191">`[]` ( _null_ )</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="562e9-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="562e9-192">Response</span></span>

<span data-ttu-id="562e9-193">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="562e9-193">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="562e9-194">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="562e9-194">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="562e9-195">Примеры</span><span class="sxs-lookup"><span data-stu-id="562e9-195">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="562e9-196">Пример 1. Создание группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="562e9-196">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="562e9-197">В следующем примере создается группа Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="562e9-197">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="562e9-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="562e9-198">Request</span></span>

<span data-ttu-id="562e9-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="562e9-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="562e9-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="562e9-200">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="562e9-201">C#</span><span class="sxs-lookup"><span data-stu-id="562e9-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="562e9-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="562e9-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="562e9-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="562e9-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="562e9-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="562e9-204">Response</span></span>

<span data-ttu-id="562e9-205">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="562e9-205">The following is an example of the response.</span></span>

><span data-ttu-id="562e9-206">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="562e9-206">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="562e9-207">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="562e9-207">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-a-microsoft-365-group-with-an-owner-and-members"></a><span data-ttu-id="562e9-208">Пример 2. Создание группы Microsoft 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="562e9-208">Example 2: Create a Microsoft 365 group with an owner and members</span></span>

<span data-ttu-id="562e9-209">В следующем примере создается группа Microsoft 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="562e9-209">The following example creates a Microsoft 365 group with an owner and members specified.</span></span> <span data-ttu-id="562e9-210">Обратите внимание на то, что в рамках создания группы можно добавить не более 20 отношений, например владельцев и участников.</span><span class="sxs-lookup"><span data-stu-id="562e9-210">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="562e9-211">Позже вы можете добавить дополнительных участников с помощью API [добавления участников](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) или пакетной обработки JSON.</span><span class="sxs-lookup"><span data-stu-id="562e9-211">You can subsequently add more members by using the [add member](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="562e9-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="562e9-212">Request</span></span>

<span data-ttu-id="562e9-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="562e9-213">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="562e9-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="562e9-214">Response</span></span> 

<span data-ttu-id="562e9-215">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="562e9-215">The following is an example of a successful response.</span></span> <span data-ttu-id="562e9-216">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="562e9-216">It includes only default properties.</span></span> <span data-ttu-id="562e9-217">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="562e9-217">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="562e9-218">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="562e9-218">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="562e9-219">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="562e9-219">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="562e9-220">Пример 3. Создание группы, которую можно назначить роли Azure AD</span><span class="sxs-lookup"><span data-stu-id="562e9-220">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="562e9-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="562e9-221">Request</span></span>

<span data-ttu-id="562e9-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="562e9-222">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="562e9-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="562e9-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="562e9-224">C#</span><span class="sxs-lookup"><span data-stu-id="562e9-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="562e9-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="562e9-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="562e9-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="562e9-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="562e9-227">**Примечание.** Свойства **visibility** и **groupTypes** необязательны для создания, но заполняются автоматически этими значениями.</span><span class="sxs-lookup"><span data-stu-id="562e9-227">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="562e9-228">Группа, свойству **isAssignableToRole** которой присвоено значение `true`, не может относиться к типу с динамическим членством.</span><span class="sxs-lookup"><span data-stu-id="562e9-228">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type.</span></span> <span data-ttu-id="562e9-229">Дополнительные сведения см. в статье [Использование группы для управления назначениями ролей Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).</span><span class="sxs-lookup"><span data-stu-id="562e9-229">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="562e9-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="562e9-230">Response</span></span>

<span data-ttu-id="562e9-231">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="562e9-231">The following is an example of the response.</span></span> <span data-ttu-id="562e9-232">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="562e9-232">It includes only default properties.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="562e9-233">См. также</span><span class="sxs-lookup"><span data-stu-id="562e9-233">See also</span></span>

- [<span data-ttu-id="562e9-234">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="562e9-234">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="562e9-235">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="562e9-235">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="562e9-236">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="562e9-236">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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


