---
title: Создание группы
description: 'Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:'
ms.openlocfilehash: a43ce33d71493d01a53a6d357937a10e29810230
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075126"
---
# <a name="create-group"></a><span data-ttu-id="df954-104">Создание группы</span><span class="sxs-lookup"><span data-stu-id="df954-104">Create group</span></span>

> <span data-ttu-id="df954-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="df954-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df954-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df954-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df954-107">Используйте этот интерфейс API для создания новой [группы](../resources/group.md) , указанный в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="df954-107">Use this API to create a new [group](../resources/group.md) as specified in the request body.</span></span> <span data-ttu-id="df954-108">Можно создать одну из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="df954-108">You can create one of three types of groups:</span></span>

* <span data-ttu-id="df954-109">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="df954-109">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="df954-110">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="df954-110">Dynamic group</span></span>
* <span data-ttu-id="df954-111">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="df954-111">Security group</span></span>

> <span data-ttu-id="df954-112">**Примечание**: чтобы создать [группы](../resources/team.md), сначала создайте группу затем добавьте группы, обратитесь к разделу [Создание группы](../api/team-put-teams.md).</span><span class="sxs-lookup"><span data-stu-id="df954-112">**Note**: To create a [team](../resources/team.md), first create a group then add a team to it, see [create team](../api/team-put-teams.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df954-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df954-113">Permissions</span></span>
<span data-ttu-id="df954-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df954-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df954-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df954-116">Permission type</span></span>      | <span data-ttu-id="df954-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df954-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df954-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df954-118">Delegated (work or school account)</span></span> | <span data-ttu-id="df954-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df954-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df954-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df954-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df954-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df954-121">Not supported.</span></span>    |
|<span data-ttu-id="df954-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df954-122">Application</span></span> | <span data-ttu-id="df954-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df954-123">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df954-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df954-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="df954-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df954-125">Request headers</span></span>
| <span data-ttu-id="df954-126">Имя</span><span class="sxs-lookup"><span data-stu-id="df954-126">Name</span></span>       | <span data-ttu-id="df954-127">Тип</span><span class="sxs-lookup"><span data-stu-id="df954-127">Type</span></span> | <span data-ttu-id="df954-128">Описание</span><span class="sxs-lookup"><span data-stu-id="df954-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="df954-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="df954-129">Authorization</span></span>  | <span data-ttu-id="df954-130">string</span><span class="sxs-lookup"><span data-stu-id="df954-130">string</span></span>  | <span data-ttu-id="df954-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df954-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df954-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df954-133">Request body</span></span>
<span data-ttu-id="df954-134">В следующей таблице приведены свойства [группы](../resources/group.md) ресурса для указания при создании группы.</span><span class="sxs-lookup"><span data-stu-id="df954-134">The following table shows the properties of the [group](../resources/group.md) resource to specify when you create a group.</span></span> 

| <span data-ttu-id="df954-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="df954-135">Property</span></span> | <span data-ttu-id="df954-136">Тип</span><span class="sxs-lookup"><span data-stu-id="df954-136">Type</span></span> | <span data-ttu-id="df954-137">Описание</span><span class="sxs-lookup"><span data-stu-id="df954-137">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="df954-138">displayName</span><span class="sxs-lookup"><span data-stu-id="df954-138">displayName</span></span> | <span data-ttu-id="df954-139">строка</span><span class="sxs-lookup"><span data-stu-id="df954-139">string</span></span> | <span data-ttu-id="df954-140">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="df954-140">The name to display in the address book for the group.</span></span> <span data-ttu-id="df954-141">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="df954-141">Required.</span></span> |
| <span data-ttu-id="df954-142">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="df954-142">mailEnabled</span></span> | <span data-ttu-id="df954-143">boolean</span><span class="sxs-lookup"><span data-stu-id="df954-143">boolean</span></span> | <span data-ttu-id="df954-144">Устанавливает значение **true** для групп с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="df954-144">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="df954-145">Установите значение **true,** Если создание группы с Office 365.</span><span class="sxs-lookup"><span data-stu-id="df954-145">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="df954-146">Установите значение **false,** Если создание динамических или группу безопасности.</span><span class="sxs-lookup"><span data-stu-id="df954-146">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="df954-147">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="df954-147">Required.</span></span> |
| <span data-ttu-id="df954-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="df954-148">mailNickname</span></span> | <span data-ttu-id="df954-149">string</span><span class="sxs-lookup"><span data-stu-id="df954-149">string</span></span> | <span data-ttu-id="df954-150">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="df954-150">The mail alias for the group.</span></span> <span data-ttu-id="df954-151">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="df954-151">Required.</span></span> |
| <span data-ttu-id="df954-152">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="df954-152">securityEnabled</span></span> | <span data-ttu-id="df954-153">boolean</span><span class="sxs-lookup"><span data-stu-id="df954-153">boolean</span></span> | <span data-ttu-id="df954-154">Значение **true** для группы с включенной поддержкой безопасности.</span><span class="sxs-lookup"><span data-stu-id="df954-154">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="df954-155">Установите значение **true,** Если создание динамической или группу безопасности.</span><span class="sxs-lookup"><span data-stu-id="df954-155">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="df954-156">При создании группы с Office 365, задайте это значение **false** .</span><span class="sxs-lookup"><span data-stu-id="df954-156">Set this to **false** if creating an Office 365 Group.</span></span> <span data-ttu-id="df954-157">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="df954-157">Required.</span></span> |
| <span data-ttu-id="df954-158">owners</span><span class="sxs-lookup"><span data-stu-id="df954-158">owners</span></span> | <span data-ttu-id="df954-159">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="df954-159">string collection</span></span> | <span data-ttu-id="df954-160">Это свойство представляет владельцев группы во время создания.</span><span class="sxs-lookup"><span data-stu-id="df954-160">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="df954-161">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="df954-161">Optional.</span></span> |
| <span data-ttu-id="df954-162">members</span><span class="sxs-lookup"><span data-stu-id="df954-162">members</span></span> | <span data-ttu-id="df954-163">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="df954-163">string collection</span></span> | <span data-ttu-id="df954-164">Это свойство представляет члены группы во время создания.</span><span class="sxs-lookup"><span data-stu-id="df954-164">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="df954-165">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="df954-165">Optional.</span></span> |

<span data-ttu-id="df954-166">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="df954-166">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="df954-167">Тип группы</span><span class="sxs-lookup"><span data-stu-id="df954-167">Type of group</span></span> | <span data-ttu-id="df954-168">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="df954-168">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="df954-169">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="df954-169">Office 365 (aka unified group)</span></span>| <span data-ttu-id="df954-170">"Unified"</span><span class="sxs-lookup"><span data-stu-id="df954-170">"Unified"</span></span> |
| <span data-ttu-id="df954-171">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="df954-171">Dynamic</span></span> | <span data-ttu-id="df954-172">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="df954-172">"DynamicMembership"</span></span> |
| <span data-ttu-id="df954-173">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="df954-173">Security</span></span> | <span data-ttu-id="df954-174">Не следует устанавливать.</span><span class="sxs-lookup"><span data-stu-id="df954-174">Do not set.</span></span> |

<span data-ttu-id="df954-175">Поскольку **группы** ресурсов поддерживает [расширения](/graph/extensibility-overview), можно использовать `POST` операции и Добавление настраиваемых свойств с собственными данными в группе при его создании.</span><span class="sxs-lookup"><span data-stu-id="df954-175">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the group while creating it.</span></span>

><span data-ttu-id="df954-176">**Примечание:** Создание группу Office 365 программными средствами без контекста пользователя и указание владельцев будет создать группу анонимных пользователей.</span><span class="sxs-lookup"><span data-stu-id="df954-176">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="df954-177">Это может привести к связанного сайта SharePoint Online, не создается автоматически до дальнейшей вручную действия предпринимаются.</span><span class="sxs-lookup"><span data-stu-id="df954-177">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="df954-p113">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="df954-p113">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="df954-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="df954-180">Response</span></span>
<span data-ttu-id="df954-181">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df954-181">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df954-182">Пример</span><span class="sxs-lookup"><span data-stu-id="df954-182">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="df954-183">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="df954-183">Request 1</span></span>
<span data-ttu-id="df954-184">Первый запрос пример создает группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="df954-184">The first example request creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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

#### <a name="response"></a><span data-ttu-id="df954-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="df954-185">Response</span></span>
<span data-ttu-id="df954-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="df954-186">The following is an example of the response.</span></span>
><span data-ttu-id="df954-187">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="df954-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="df954-188">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df954-188">All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="df954-189">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="df954-189">Request 2</span></span>
<span data-ttu-id="df954-190">Второй запрос на примере создает группу Office 365 с помощью указанных владельцев.</span><span class="sxs-lookup"><span data-stu-id="df954-190">The second example request creates an Office 365 Group with owners specified.</span></span>
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

 #### <a name="response-2"></a><span data-ttu-id="df954-191">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="df954-191">Response 2</span></span>
<span data-ttu-id="df954-192">Ниже приведен пример успешного ответа.</span><span class="sxs-lookup"><span data-stu-id="df954-192">The following is an example of the successful response.</span></span>
><span data-ttu-id="df954-p115">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df954-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="df954-195">См. также</span><span class="sxs-lookup"><span data-stu-id="df954-195">See also</span></span>

- [<span data-ttu-id="df954-196">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="df954-196">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="df954-197">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="df954-197">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="df954-198">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="df954-198">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
