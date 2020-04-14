---
title: Создание группы
description: Создание группы Office 365 или группы безопасности.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e4fc80fc664404a0d17d535282e0d791b7e96cbb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396615"
---
# <a name="create-group"></a><span data-ttu-id="3c4f8-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="3c4f8-103">Create group</span></span>

<span data-ttu-id="3c4f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c4f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c4f8-105">Создание [группы](../resources/group.md) согласно инструкциям в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-105">Create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="3c4f8-106">Можно создать одну из следующих групп:</span><span class="sxs-lookup"><span data-stu-id="3c4f8-106">You can create one of the following groups:</span></span>

* <span data-ttu-id="3c4f8-107">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-107">Office 365 group (unified group)</span></span>
* <span data-ttu-id="3c4f8-108">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="3c4f8-108">Security group</span></span>

<span data-ttu-id="3c4f8-109">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="3c4f8-110">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="3c4f8-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="3c4f8-111">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

><span data-ttu-id="3c4f8-112">**Примечание.** Чтобы создать [команду](../resources/team.md), сначала создайте группу и добавьте команду в нее, см. раздел [Создание команды](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="3c4f8-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c4f8-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c4f8-113">Permissions</span></span>
<span data-ttu-id="3c4f8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c4f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c4f8-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c4f8-116">Permission type</span></span>      | <span data-ttu-id="3c4f8-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c4f8-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-118">Delegated (work or school account)</span></span> | <span data-ttu-id="3c4f8-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c4f8-119">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="3c4f8-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c4f8-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-121">Not supported.</span></span>    |
|<span data-ttu-id="3c4f8-122">Приложение</span><span class="sxs-lookup"><span data-stu-id="3c4f8-122">Application</span></span> | <span data-ttu-id="3c4f8-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c4f8-123">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c4f8-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c4f8-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="3c4f8-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c4f8-125">Request headers</span></span>

| <span data-ttu-id="3c4f8-126">Имя</span><span class="sxs-lookup"><span data-stu-id="3c4f8-126">Name</span></span>       | <span data-ttu-id="3c4f8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3c4f8-127">Type</span></span> | <span data-ttu-id="3c4f8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3c4f8-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c4f8-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c4f8-129">Authorization</span></span>  | <span data-ttu-id="3c4f8-130">string</span><span class="sxs-lookup"><span data-stu-id="3c4f8-130">string</span></span>  | <span data-ttu-id="3c4f8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c4f8-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c4f8-133">Request body</span></span>

<span data-ttu-id="3c4f8-134">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="3c4f8-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c4f8-135">Property</span></span> | <span data-ttu-id="3c4f8-136">Тип</span><span class="sxs-lookup"><span data-stu-id="3c4f8-136">Type</span></span> | <span data-ttu-id="3c4f8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3c4f8-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c4f8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3c4f8-138">displayName</span></span> | <span data-ttu-id="3c4f8-139">string</span><span class="sxs-lookup"><span data-stu-id="3c4f8-139">string</span></span> | <span data-ttu-id="3c4f8-140">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="3c4f8-141">Максимальная длина: 256 символов.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-141">Maximum length: 256 characters.</span></span> <span data-ttu-id="3c4f8-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-142">Required.</span></span> |
| <span data-ttu-id="3c4f8-143">description</span><span class="sxs-lookup"><span data-stu-id="3c4f8-143">description</span></span> | <span data-ttu-id="3c4f8-144">строка</span><span class="sxs-lookup"><span data-stu-id="3c4f8-144">string</span></span> | <span data-ttu-id="3c4f8-145">Описание группы.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-145">A description for the group.</span></span> <span data-ttu-id="3c4f8-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-146">Optional.</span></span> |
| <span data-ttu-id="3c4f8-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="3c4f8-147">mailEnabled</span></span> | <span data-ttu-id="3c4f8-148">boolean</span><span class="sxs-lookup"><span data-stu-id="3c4f8-148">boolean</span></span> | <span data-ttu-id="3c4f8-149">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-149">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="3c4f8-150">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-150">Required.</span></span> |
| <span data-ttu-id="3c4f8-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3c4f8-151">mailNickname</span></span> | <span data-ttu-id="3c4f8-152">string</span><span class="sxs-lookup"><span data-stu-id="3c4f8-152">string</span></span> | <span data-ttu-id="3c4f8-153">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-153">The mail alias for the group.</span></span> <span data-ttu-id="3c4f8-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-154">Required.</span></span> |
| <span data-ttu-id="3c4f8-155">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="3c4f8-155">securityEnabled</span></span> | <span data-ttu-id="3c4f8-156">boolean</span><span class="sxs-lookup"><span data-stu-id="3c4f8-156">boolean</span></span> | <span data-ttu-id="3c4f8-157">Значение **true** для защищенных групп, включая группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-157">Set to **true** for security-enabled groups, including Office 365 groups.</span></span> <span data-ttu-id="3c4f8-158">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-158">Required.</span></span> |
| <span data-ttu-id="3c4f8-159">owners</span><span class="sxs-lookup"><span data-stu-id="3c4f8-159">owners</span></span> | <span data-ttu-id="3c4f8-160">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-160">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="3c4f8-161">Это свойство представляет владельцев группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-161">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="3c4f8-162">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-162">Optional.</span></span> |
| <span data-ttu-id="3c4f8-163">members</span><span class="sxs-lookup"><span data-stu-id="3c4f8-163">members</span></span> | <span data-ttu-id="3c4f8-164">Коллекция [directoryObject](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-164">[directoryObject](../resources/directoryobject.md) collection</span></span> | <span data-ttu-id="3c4f8-165">Это свойство представляет участников группы на момент создания.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-165">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="3c4f8-166">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-166">Optional.</span></span> |
|<span data-ttu-id="3c4f8-167">visibility</span><span class="sxs-lookup"><span data-stu-id="3c4f8-167">visibility</span></span>|<span data-ttu-id="3c4f8-168">String</span><span class="sxs-lookup"><span data-stu-id="3c4f8-168">String</span></span>|<span data-ttu-id="3c4f8-169">Определяет видимость группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-169">Specifies the visibility of an Office 365 group.</span></span> <span data-ttu-id="3c4f8-170">Возможные значения: `Private`, `Public`, `HiddenMembership` или пустое значение (обрабатывается как `Public`).</span><span class="sxs-lookup"><span data-stu-id="3c4f8-170">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="3c4f8-171">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-171">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="3c4f8-172">Так как ресурс **group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `POST` можно добавлять настраиваемые свойства с собственными данными к группе при ее создании.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-172">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="3c4f8-173">**Примечание:** создание группы с помощью разрешения приложения Group.Create без указания владельцев анонимно создает группу, которая не будет изменяться.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-173">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="3c4f8-174">Вы можете использовать операцию `POST` и добавить владельцев в группу при ее создании, чтобы указать владельцев, которые могут изменять группу.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-174">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="3c4f8-175">Создание группы Office 365 программным путем с контекстом только для приложений, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-175">Creating an Office 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="3c4f8-176">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="3c4f8-177">При необходимости укажите другие записываемые свойства для своей группы.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-177">Specify other writable properties as necessary for your group.</span></span> <span data-ttu-id="3c4f8-178">Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="3c4f8-178">For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="3c4f8-179">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="3c4f8-179">groupTypes options</span></span>

<span data-ttu-id="3c4f8-180">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-180">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="3c4f8-181">Тип группы</span><span class="sxs-lookup"><span data-stu-id="3c4f8-181">Type of group</span></span> | <span data-ttu-id="3c4f8-182">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="3c4f8-182">Assigned membership</span></span> | <span data-ttu-id="3c4f8-183">Динамическое участие</span><span class="sxs-lookup"><span data-stu-id="3c4f8-183">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="3c4f8-184">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-184">Office 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="3c4f8-185">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="3c4f8-185">Dynamic</span></span> | <span data-ttu-id="3c4f8-186">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-186">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="3c4f8-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c4f8-187">Response</span></span>

<span data-ttu-id="3c4f8-188">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-188">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="3c4f8-189">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-189">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="3c4f8-190">Примеры</span><span class="sxs-lookup"><span data-stu-id="3c4f8-190">Examples</span></span>

### <a name="example-1-create-an-office-365-group"></a><span data-ttu-id="3c4f8-191">Пример 1. Создание группы Office 365</span><span class="sxs-lookup"><span data-stu-id="3c4f8-191">Example 1: Create an Office 365 group</span></span>

<span data-ttu-id="3c4f8-192">В приведенном ниже примере создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-192">The following example creates an Office 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="3c4f8-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c4f8-193">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c4f8-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c4f8-194">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3c4f8-195">C#</span><span class="sxs-lookup"><span data-stu-id="3c4f8-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c4f8-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c4f8-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c4f8-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c4f8-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c4f8-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c4f8-198">Response</span></span>

<span data-ttu-id="3c4f8-199">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-199">The following is an example of the response.</span></span>

><span data-ttu-id="3c4f8-200">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-200">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c4f8-201">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-201">All the default properties are returned from an actual call.</span></span>

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

### <a name="example-2-create-an-office-365-group-with-an-owner-and-members"></a><span data-ttu-id="3c4f8-202">Пример 2. Создание группы Office 365 с владельцем и участниками</span><span class="sxs-lookup"><span data-stu-id="3c4f8-202">Example 2: Create an Office 365 group with an owner and members</span></span>

<span data-ttu-id="3c4f8-203">В следующем примере создается группа Office 365 с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-203">The following example creates an Office 365 group with an owner and members specified.</span></span> <span data-ttu-id="3c4f8-204">Обратите внимание на то, что в рамках создания группы можно добавить не более 20 отношений, например владельцев и участников.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-204">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="3c4f8-205">Позже вы можете добавить дополнительных участников с помощью API [добавления участников](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) или пакетной обработки JSON.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-205">You can subsequently add more members by using the [add member](https://docs.microsoft.com/graph/api/group-post-members?view=graph-rest-beta&tabs=http) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="3c4f8-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c4f8-206">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c4f8-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c4f8-207">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3c4f8-208">C#</span><span class="sxs-lookup"><span data-stu-id="3c4f8-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c4f8-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c4f8-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c4f8-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c4f8-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c4f8-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c4f8-211">Response</span></span> 

<span data-ttu-id="3c4f8-212">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-212">The following is an example of a successful response.</span></span> <span data-ttu-id="3c4f8-213">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-213">It includes only default properties.</span></span> <span data-ttu-id="3c4f8-214">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-214">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="3c4f8-215">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-215">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c4f8-216">В результате реального вызова возвращаются все свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c4f8-216">All the default properties are returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="3c4f8-217">См. также</span><span class="sxs-lookup"><span data-stu-id="3c4f8-217">See also</span></span>

- [<span data-ttu-id="3c4f8-218">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="3c4f8-218">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3c4f8-219">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-219">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3c4f8-220">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3c4f8-220">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
