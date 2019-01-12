---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 2a3e0e20622db47d410b578249df94f3354e75ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981548"
---
# <a name="create-group"></a><span data-ttu-id="7b9c6-104">Создание группы</span><span class="sxs-lookup"><span data-stu-id="7b9c6-104">Create group</span></span>
<span data-ttu-id="7b9c6-p102">Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="7b9c6-p102">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="7b9c6-107">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="7b9c6-107">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="7b9c6-108">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="7b9c6-108">Dynamic group</span></span>
* <span data-ttu-id="7b9c6-109">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="7b9c6-109">Security group</span></span>

> <span data-ttu-id="7b9c6-p103">**Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-p103">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b9c6-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b9c6-112">Permissions</span></span>
<span data-ttu-id="7b9c6-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b9c6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b9c6-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b9c6-115">Permission type</span></span>      | <span data-ttu-id="7b9c6-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b9c6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b9c6-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b9c6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7b9c6-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b9c6-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b9c6-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b9c6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b9c6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-120">Not supported.</span></span>    |
|<span data-ttu-id="7b9c6-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b9c6-121">Application</span></span> | <span data-ttu-id="7b9c6-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b9c6-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b9c6-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b9c6-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="7b9c6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b9c6-124">Request headers</span></span>
| <span data-ttu-id="7b9c6-125">Имя</span><span class="sxs-lookup"><span data-stu-id="7b9c6-125">Name</span></span>       | <span data-ttu-id="7b9c6-126">Тип</span><span class="sxs-lookup"><span data-stu-id="7b9c6-126">Type</span></span> | <span data-ttu-id="7b9c6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7b9c6-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b9c6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b9c6-128">Authorization</span></span>  | <span data-ttu-id="7b9c6-129">строка</span><span class="sxs-lookup"><span data-stu-id="7b9c6-129">string</span></span>  | <span data-ttu-id="7b9c6-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b9c6-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b9c6-132">Request body</span></span>
<span data-ttu-id="7b9c6-133">В следующей таблице приведены свойства [группы](../resources/group.md) ресурса для указания при создании группы.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-133">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="7b9c6-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b9c6-134">Property</span></span> | <span data-ttu-id="7b9c6-135">Тип</span><span class="sxs-lookup"><span data-stu-id="7b9c6-135">Type</span></span> | <span data-ttu-id="7b9c6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="7b9c6-136">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b9c6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7b9c6-137">displayName</span></span> | <span data-ttu-id="7b9c6-138">строка</span><span class="sxs-lookup"><span data-stu-id="7b9c6-138">string</span></span> | <span data-ttu-id="7b9c6-139">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-139">The name to display in the address book for the group.</span></span> <span data-ttu-id="7b9c6-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-140">Required.</span></span> |
| <span data-ttu-id="7b9c6-141">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="7b9c6-141">mailEnabled</span></span> | <span data-ttu-id="7b9c6-142">boolean</span><span class="sxs-lookup"><span data-stu-id="7b9c6-142">boolean</span></span> | <span data-ttu-id="7b9c6-143">Устанавливает значение **true** для групп с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-143">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="7b9c6-144">Установите значение **true,** Если создание группы с Office 365.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-144">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="7b9c6-145">Установите значение **false,** Если создание динамических или группу безопасности.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-145">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="7b9c6-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-146">Required.</span></span> |
| <span data-ttu-id="7b9c6-147">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7b9c6-147">mailNickname</span></span> | <span data-ttu-id="7b9c6-148">строка</span><span class="sxs-lookup"><span data-stu-id="7b9c6-148">string</span></span> | <span data-ttu-id="7b9c6-149">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-149">The mail alias for the group.</span></span> <span data-ttu-id="7b9c6-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-150">Required.</span></span> |
| <span data-ttu-id="7b9c6-151">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="7b9c6-151">securityEnabled</span></span> | <span data-ttu-id="7b9c6-152">boolean</span><span class="sxs-lookup"><span data-stu-id="7b9c6-152">boolean</span></span> | <span data-ttu-id="7b9c6-153">Значение **true** для группы с включенной поддержкой безопасности.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-153">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="7b9c6-154">Установите значение **true,** Если создание динамической или группу безопасности.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-154">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="7b9c6-155">При создании группы с Office 365, задайте это значение **false** .</span><span class="sxs-lookup"><span data-stu-id="7b9c6-155">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="7b9c6-156">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-156">Required.</span></span> |
| <span data-ttu-id="7b9c6-157">owners</span><span class="sxs-lookup"><span data-stu-id="7b9c6-157">owners</span></span> | <span data-ttu-id="7b9c6-158">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b9c6-158">string collection</span></span> | <span data-ttu-id="7b9c6-159">Это свойство представляет владельцев группы во время создания.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-159">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="7b9c6-160">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-160">Optional.</span></span> |
| <span data-ttu-id="7b9c6-161">members</span><span class="sxs-lookup"><span data-stu-id="7b9c6-161">members</span></span> | <span data-ttu-id="7b9c6-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b9c6-162">string collection</span></span> | <span data-ttu-id="7b9c6-163">Это свойство представляет члены группы во время создания.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-163">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="7b9c6-164">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-164">Optional.</span></span> |


<span data-ttu-id="7b9c6-165">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-165">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="7b9c6-166">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="7b9c6-166">groupTypes options</span></span>

| <span data-ttu-id="7b9c6-167">Тип группы</span><span class="sxs-lookup"><span data-stu-id="7b9c6-167">Type of group</span></span> | <span data-ttu-id="7b9c6-168">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="7b9c6-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="7b9c6-169">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="7b9c6-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="7b9c6-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="7b9c6-170">"Unified"</span></span> |
| <span data-ttu-id="7b9c6-171">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="7b9c6-171">Dynamic</span></span> | <span data-ttu-id="7b9c6-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="7b9c6-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="7b9c6-173">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="7b9c6-173">Security</span></span> | <span data-ttu-id="7b9c6-174">Не следует устанавливать.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-174">Do not set.</span></span> |


><span data-ttu-id="7b9c6-175">**Примечание:** Создание группу Office 365 программными средствами без контекста пользователя и указание владельцев будет создать группу анонимных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-175">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="7b9c6-176">Это может привести к связанного сайта SharePoint Online, не создается автоматически до дальнейшей вручную действия предпринимаются.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-176">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="7b9c6-p113">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="7b9c6-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="7b9c6-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b9c6-179">Response</span></span>
<span data-ttu-id="7b9c6-180">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-180">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b9c6-181">Пример</span><span class="sxs-lookup"><span data-stu-id="7b9c6-181">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="7b9c6-182">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="7b9c6-182">Request 1</span></span>
<span data-ttu-id="7b9c6-183">Первый запрос пример создает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-183">The first example request creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="7b9c6-184">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="7b9c6-184">Response 1</span></span>
<span data-ttu-id="7b9c6-185">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-185">The following is an example of the response.</span></span>
><span data-ttu-id="7b9c6-186">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-186">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b9c6-187">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-187">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a><span data-ttu-id="7b9c6-188">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="7b9c6-188">Request 2</span></span>
<span data-ttu-id="7b9c6-189">Второй запрос на примере создает группу Office 365 с помощью указанных владельцев.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-189">The second example request creates an Office 365 Group with owners specified.</span></span>
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="7b9c6-190">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="7b9c6-190">Response 2</span></span>
<span data-ttu-id="7b9c6-191">Ниже приведен пример успешного ответа.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-191">The following is an example of the successful response.</span></span>
><span data-ttu-id="7b9c6-192">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-192">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b9c6-193">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b9c6-193">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
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
