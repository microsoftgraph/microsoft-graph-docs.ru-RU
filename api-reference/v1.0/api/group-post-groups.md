---
title: Создание группы
description: 'Создание группы согласно инструкциям в тексте запроса. '
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e90157f8139de8524bcf497c7aa0c9c496aceac7
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209708"
---
# <a name="create-group"></a><span data-ttu-id="dfd9c-103">Создание группы</span><span class="sxs-lookup"><span data-stu-id="dfd9c-103">Create group</span></span>

<span data-ttu-id="dfd9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfd9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfd9c-p101">Создайте новую группу согласно инструкциям в тексте запроса. Можно создать один из следующих типов групп.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p101">Create a new group as specified in the request body. You can create the following types of groups:</span></span>

* <span data-ttu-id="dfd9c-107">Группа Microsoft 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="dfd9c-107">Microsoft 365 group (unified group)</span></span>
* <span data-ttu-id="dfd9c-108">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="dfd9c-108">Security group</span></span>

<span data-ttu-id="dfd9c-109">Эта операция по умолчанию возвращает только подмножество свойств для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-109">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="dfd9c-110">Эти свойства по умолчанию указаны в разделе [Свойства](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="dfd9c-110">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span>

<span data-ttu-id="dfd9c-111">Чтобы получить свойства, которые _не_ возвращаются по умолчанию, выполните [операцию GET](group-get.md) и укажите их в параметре запроса OData `$select`.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-111">To get properties that are _not_ returned by default, do a [GET operation](group-get.md) and specify the properties in a `$select` OData query option.</span></span>

> <span data-ttu-id="dfd9c-112">**Примечание.** Несмотря на то, что Microsoft Teams создан на основе групп Microsoft 365, в настоящее время нельзя создать команду через этот API.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-112">**Note**: Although Microsoft Teams is built on Microsoft 365 groups, you can't currently create a team via this API.</span></span> <span data-ttu-id="dfd9c-113">Вы можете использовать другие API групп для управления командой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-113">You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfd9c-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfd9c-114">Permissions</span></span>
<span data-ttu-id="dfd9c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfd9c-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfd9c-117">Permission type</span></span>      | <span data-ttu-id="dfd9c-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfd9c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfd9c-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfd9c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="dfd9c-120">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfd9c-120">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="dfd9c-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfd9c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfd9c-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-122">Not supported.</span></span>    |
|<span data-ttu-id="dfd9c-123">Приложение</span><span class="sxs-lookup"><span data-stu-id="dfd9c-123">Application</span></span> | <span data-ttu-id="dfd9c-124">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd9c-124">Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfd9c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfd9c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="dfd9c-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfd9c-126">Request headers</span></span>
| <span data-ttu-id="dfd9c-127">Имя</span><span class="sxs-lookup"><span data-stu-id="dfd9c-127">Name</span></span>       | <span data-ttu-id="dfd9c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="dfd9c-128">Type</span></span> | <span data-ttu-id="dfd9c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dfd9c-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfd9c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfd9c-130">Authorization</span></span>  | <span data-ttu-id="dfd9c-131">string</span><span class="sxs-lookup"><span data-stu-id="dfd9c-131">string</span></span>  | <span data-ttu-id="dfd9c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfd9c-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfd9c-134">Content-Type</span></span>  | <span data-ttu-id="dfd9c-135">application/json</span><span class="sxs-lookup"><span data-stu-id="dfd9c-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfd9c-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfd9c-136">Request body</span></span>
<span data-ttu-id="dfd9c-137">В приведенной ниже таблице показаны свойства ресурса [group](../resources/group.md), которые необходимо указать при создании группы.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-137">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="dfd9c-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfd9c-138">Property</span></span> | <span data-ttu-id="dfd9c-139">Тип</span><span class="sxs-lookup"><span data-stu-id="dfd9c-139">Type</span></span> | <span data-ttu-id="dfd9c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="dfd9c-140">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfd9c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="dfd9c-141">displayName</span></span> | <span data-ttu-id="dfd9c-142">string</span><span class="sxs-lookup"><span data-stu-id="dfd9c-142">string</span></span> | <span data-ttu-id="dfd9c-p106">Имя, которое следует отобразить в адресной книге для группы. Максимальная длина: 256 символов. Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p106">The name to display in the address book for the group. Maximum length: 256 characters. Required.</span></span> |
| <span data-ttu-id="dfd9c-146">description</span><span class="sxs-lookup"><span data-stu-id="dfd9c-146">description</span></span> | <span data-ttu-id="dfd9c-147">строка</span><span class="sxs-lookup"><span data-stu-id="dfd9c-147">string</span></span> | <span data-ttu-id="dfd9c-148">Описание группы.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-148">A description for the group.</span></span> <span data-ttu-id="dfd9c-149">Максимальная</span><span class="sxs-lookup"><span data-stu-id="dfd9c-149">Max.</span></span> <span data-ttu-id="dfd9c-150">длина: 1024 символа.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-150">length: 1024 characters.</span></span> <span data-ttu-id="dfd9c-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-151">Optional.</span></span> |
| <span data-ttu-id="dfd9c-152">isAssignableToRole</span><span class="sxs-lookup"><span data-stu-id="dfd9c-152">isAssignableToRole</span></span> | <span data-ttu-id="dfd9c-153">Логическое</span><span class="sxs-lookup"><span data-stu-id="dfd9c-153">Boolean</span></span> | <span data-ttu-id="dfd9c-154">Значение **true**, чтобы группу можно было назначить роли Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-154">Set to **true** to enable the group to be assigned to an Azure AD role.</span></span> <span data-ttu-id="dfd9c-155">Только администратор привилегированных ролей и глобальный администратор может настроить значение этого свойства.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-155">Only Privileged Role Administrator and Global Administrator can set the value of this property.</span></span> <span data-ttu-id="dfd9c-156">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-156">Optional.</span></span> |
| <span data-ttu-id="dfd9c-157">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="dfd9c-157">mailEnabled</span></span> | <span data-ttu-id="dfd9c-158">boolean</span><span class="sxs-lookup"><span data-stu-id="dfd9c-158">boolean</span></span> | <span data-ttu-id="dfd9c-159">Установите значение **true** для групп, поддерживающих почту.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-159">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="dfd9c-160">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-160">Required.</span></span> |
| <span data-ttu-id="dfd9c-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="dfd9c-161">mailNickname</span></span> | <span data-ttu-id="dfd9c-162">string</span><span class="sxs-lookup"><span data-stu-id="dfd9c-162">string</span></span> | <span data-ttu-id="dfd9c-163">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-163">The mail alias for the group.</span></span> <span data-ttu-id="dfd9c-164">Максимальная</span><span class="sxs-lookup"><span data-stu-id="dfd9c-164">Max.</span></span> <span data-ttu-id="dfd9c-165">длина: 64 символа.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-165">length: 64 characters.</span></span> <span data-ttu-id="dfd9c-166">Такие символы нельзя использовать в mailNickName: `@()\[]";:.<>,SPACE`.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-166">These characters cannot be used in the mailNickName: `@()\[]";:.<>,SPACE`.</span></span> <span data-ttu-id="dfd9c-167">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-167">Required.</span></span> |
| <span data-ttu-id="dfd9c-168">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="dfd9c-168">securityEnabled</span></span> | <span data-ttu-id="dfd9c-169">boolean</span><span class="sxs-lookup"><span data-stu-id="dfd9c-169">boolean</span></span> | <span data-ttu-id="dfd9c-170">Значение **true** для групп безопасности, включая группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-170">Set to **true** for security-enabled groups, including Microsoft 365 groups.</span></span> <span data-ttu-id="dfd9c-171">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-171">Required.</span></span> |
| <span data-ttu-id="dfd9c-172">owners</span><span class="sxs-lookup"><span data-stu-id="dfd9c-172">owners</span></span> | <span data-ttu-id="dfd9c-173">string collection</span><span class="sxs-lookup"><span data-stu-id="dfd9c-173">string collection</span></span> | <span data-ttu-id="dfd9c-p112">Это свойство представляет владельцев группы на момент создания. Необязательно.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p112">This property represents the owners for the group at creation time. Optional.</span></span> |
| <span data-ttu-id="dfd9c-176">members</span><span class="sxs-lookup"><span data-stu-id="dfd9c-176">members</span></span> | <span data-ttu-id="dfd9c-177">string collection</span><span class="sxs-lookup"><span data-stu-id="dfd9c-177">string collection</span></span> | <span data-ttu-id="dfd9c-p113">Это свойство представляет участников группы на момент создания. Необязательно.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p113">This property represents the members for the group at creation time. Optional.</span></span> |
|<span data-ttu-id="dfd9c-180">visibility</span><span class="sxs-lookup"><span data-stu-id="dfd9c-180">visibility</span></span>|<span data-ttu-id="dfd9c-181">String</span><span class="sxs-lookup"><span data-stu-id="dfd9c-181">String</span></span>|<span data-ttu-id="dfd9c-182">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-182">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="dfd9c-183">Возможные значения: `Private`, `Public`, `HiddenMembership` или пустое значение (обрабатывается как `Public`).</span><span class="sxs-lookup"><span data-stu-id="dfd9c-183">Possible values are: `Private`, `Public`, `HiddenMembership`, or empty (which is interpreted as `Public`).</span></span>|

> <span data-ttu-id="dfd9c-184">**Примечание.** В группах, созданных с помощью портала Microsoft Azure, для свойства **securityEnabled** всегда устанавливается значение `true`.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-184">**Note:** Groups created using the Microsoft Azure portal always have **securityEnabled** initially set to `true`.</span></span>

<span data-ttu-id="dfd9c-p115">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p115">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

><span data-ttu-id="dfd9c-187">**Примечание:** создание группы с помощью разрешения приложения Group.Create без указания владельцев анонимно создает группу, которая не будет изменяться.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-187">**Note:** Creating a group using the Group.Create application permission without specifying owners will create the group anonymously and the group will not be modifiable.</span></span> <span data-ttu-id="dfd9c-188">Вы можете использовать операцию `POST` и добавить владельцев в группу при ее создании, чтобы указать владельцев, которые могут изменять группу.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-188">You can use the `POST` operation and add owners to the group while creating it to specify owners who can modify the group.</span></span>

> <span data-ttu-id="dfd9c-189">Создание группы Microsoft 365 программным путем с контекстом только для приложений, а также без указания владельцев будет анонимным.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-189">Creating a Microsoft 365 group programmatically with an app-only context and without specifying owners will create the group anonymously.</span></span> <span data-ttu-id="dfd9c-190">Это может привести к тому, что связанный с ней сайт SharePoint Online не будет создан автоматически, пока дальнейшие действия не будут выполнены вручную.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-190">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  


### <a name="grouptypes-options"></a><span data-ttu-id="dfd9c-191">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="dfd9c-191">groupTypes options</span></span>

<span data-ttu-id="dfd9c-192">Свойство **groupTypes** используется для управления типом группы и участием в ней, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-192">Use the **groupTypes** property to control the type of group and its membership, as shown.</span></span>

| <span data-ttu-id="dfd9c-193">Тип группы</span><span class="sxs-lookup"><span data-stu-id="dfd9c-193">Type of group</span></span> | <span data-ttu-id="dfd9c-194">Назначенное участие</span><span class="sxs-lookup"><span data-stu-id="dfd9c-194">Assigned membership</span></span> | <span data-ttu-id="dfd9c-195">Динамическое членство</span><span class="sxs-lookup"><span data-stu-id="dfd9c-195">Dynamic membership</span></span> |
|:--------------|:------------------------|:---------------|
| <span data-ttu-id="dfd9c-196">Microsoft 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="dfd9c-196">Microsoft 365 (aka unified group)</span></span>| `["Unified"]` | `["Unified","DynamicMembership"]`
| <span data-ttu-id="dfd9c-197">Динамический</span><span class="sxs-lookup"><span data-stu-id="dfd9c-197">Dynamic</span></span> | <span data-ttu-id="dfd9c-198">`[]` (_null_)</span><span class="sxs-lookup"><span data-stu-id="dfd9c-198">`[]` (_null_)</span></span> | `["DynamicMembership"]`|

## <a name="response"></a><span data-ttu-id="dfd9c-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfd9c-199">Response</span></span>
<span data-ttu-id="dfd9c-200">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-200">If successful, this method returns a `201 Created` response code and a [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="dfd9c-201">Отклик включает в себя только свойства по умолчанию для группы.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-201">The response includes only the default properties of the group.</span></span>

## <a name="examples"></a><span data-ttu-id="dfd9c-202">Примеры</span><span class="sxs-lookup"><span data-stu-id="dfd9c-202">Examples</span></span>

### <a name="example-1-create-a-microsoft-365-group"></a><span data-ttu-id="dfd9c-203">Пример 1. Создание группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="dfd9c-203">Example 1: Create a Microsoft 365 group</span></span>

<span data-ttu-id="dfd9c-204">В следующем примере создается группа Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-204">The following example creates a Microsoft 365 group.</span></span>

#### <a name="request"></a><span data-ttu-id="dfd9c-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfd9c-205">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dfd9c-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfd9c-206">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dfd9c-207">C#</span><span class="sxs-lookup"><span data-stu-id="dfd9c-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfd9c-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfd9c-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfd9c-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfd9c-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfd9c-210">Java</span><span class="sxs-lookup"><span data-stu-id="dfd9c-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dfd9c-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfd9c-211">Response</span></span>

<span data-ttu-id="dfd9c-212">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-212">The following is an example of the response.</span></span>

><span data-ttu-id="dfd9c-213">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-213">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-create-a-group-with-owners-and-members"></a><span data-ttu-id="dfd9c-214">Пример 2. Создание группы с владельцами и участниками</span><span class="sxs-lookup"><span data-stu-id="dfd9c-214">Example 2: Create a group with owners and members</span></span>

<span data-ttu-id="dfd9c-215">В следующем примере создается группа безопасности с указанным владельцем и участниками.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-215">The following example creates a Security group with an owner and members specified.</span></span> <span data-ttu-id="dfd9c-216">Обратите внимание на то, что в рамках создания группы можно добавить не более 20 отношений, например владельцев и участников.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-216">Note that a maximum of 20 relationships, such as owners and members, can be added as part of group creation.</span></span> <span data-ttu-id="dfd9c-217">Позже вы можете добавить дополнительных участников с помощью API [добавления участников](group-post-members.md) или пакетной обработки JSON.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-217">You can subsequently add more members by using the [add member](group-post-members.md) API or JSON batching.</span></span>

#### <a name="request"></a><span data-ttu-id="dfd9c-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfd9c-218">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dfd9c-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfd9c-219">HTTP</span></span>](#tab/http)
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
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="dfd9c-220">C#</span><span class="sxs-lookup"><span data-stu-id="dfd9c-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-prepopulated-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfd9c-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfd9c-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-prepopulated-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfd9c-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfd9c-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-prepopulated-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfd9c-223">Java</span><span class="sxs-lookup"><span data-stu-id="dfd9c-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-prepopulated-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dfd9c-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfd9c-224">Response</span></span>

<span data-ttu-id="dfd9c-225">Ниже представлен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-225">The following is an example of a successful response.</span></span> <span data-ttu-id="dfd9c-226">Он включает только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-226">It includes only default properties.</span></span> <span data-ttu-id="dfd9c-227">Вы можете получить свойства навигации **owners** или **members** группы, чтобы проверить владельца или участников.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-227">You can subsequently get the **owners** or **members** navigation properties of the group to verify the owner or members.</span></span> 

><span data-ttu-id="dfd9c-228">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-228">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-group-that-can-be-assigned-to-an-azure-ad-role"></a><span data-ttu-id="dfd9c-229">Пример 3. Создание группы, которую можно назначить роли Azure AD</span><span class="sxs-lookup"><span data-stu-id="dfd9c-229">Example 3: Create a group that can be assigned to an Azure AD role</span></span>

#### <a name="request"></a><span data-ttu-id="dfd9c-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfd9c-230">Request</span></span>

<span data-ttu-id="dfd9c-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-231">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dfd9c-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfd9c-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups
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
# <a name="c"></a>[<span data-ttu-id="dfd9c-233">C#</span><span class="sxs-lookup"><span data-stu-id="dfd9c-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfd9c-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfd9c-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfd9c-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfd9c-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfd9c-236">Java</span><span class="sxs-lookup"><span data-stu-id="dfd9c-236">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="dfd9c-237">**Примечание.** Свойства **visibility** и **groupTypes** необязательны для создания, но заполняются автоматически этими значениями.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-237">**Note:** The **visibility** and **groupTypes** properties are not required for creation, but are auto-populated with these values.</span></span> <span data-ttu-id="dfd9c-238">Группа, свойству **isAssignableToRole** которой присвоено значение `true`, не может относиться к типу с динамическим членством и иметь владельца.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-238">A group with **isAssignableToRole** property set to `true` cannot be of dynamic membership type and cannot have an owner.</span></span> <span data-ttu-id="dfd9c-239">Дополнительные сведения см. в статье [Использование группы для управления назначениями ролей Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).</span><span class="sxs-lookup"><span data-stu-id="dfd9c-239">For more information, see [Using a group to manage Azure AD role assignments](https://go.microsoft.com/fwlink/?linkid=2103037).</span></span>

#### <a name="response"></a><span data-ttu-id="dfd9c-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfd9c-240">Response</span></span>

<span data-ttu-id="dfd9c-p122">Ниже приведен пример отклика. Он содержит только свойства по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dfd9c-p122">The following is an example of the response. It includes only default properties.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
} -->

