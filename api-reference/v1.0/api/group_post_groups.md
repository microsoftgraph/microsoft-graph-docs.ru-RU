# <a name="create-group"></a><span data-ttu-id="efda0-101">Создание группы</span><span class="sxs-lookup"><span data-stu-id="efda0-101">Create group</span></span>
<span data-ttu-id="efda0-p101">Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="efda0-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="efda0-104">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="efda0-104">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="efda0-105">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="efda0-105">Dynamic group</span></span>
* <span data-ttu-id="efda0-106">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="efda0-106">Security group</span></span>

> <span data-ttu-id="efda0-p102">**Примечание.** Несмотря на то что Microsoft Teams создан на основе Групп Office 365, в настоящее время невозможно создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="efda0-p102">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="efda0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efda0-109">Permissions</span></span>
<span data-ttu-id="efda0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="efda0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="efda0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efda0-112">Permission type</span></span>      | <span data-ttu-id="efda0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efda0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efda0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efda0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="efda0-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efda0-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="efda0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efda0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efda0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efda0-117">Not supported.</span></span>    |
|<span data-ttu-id="efda0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efda0-118">Application</span></span> | <span data-ttu-id="efda0-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efda0-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efda0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efda0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="efda0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efda0-121">Request headers</span></span>
| <span data-ttu-id="efda0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="efda0-122">Name</span></span>       | <span data-ttu-id="efda0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="efda0-123">Type</span></span> | <span data-ttu-id="efda0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="efda0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efda0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efda0-125">Authorization</span></span>  | <span data-ttu-id="efda0-126">string</span><span class="sxs-lookup"><span data-stu-id="efda0-126">string</span></span>  | <span data-ttu-id="efda0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efda0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efda0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efda0-129">Request body</span></span>
<span data-ttu-id="efda0-130">В таблице ниже представлены свойства ресурса [group](../resources/group.md) для указания при создании группы.</span><span class="sxs-lookup"><span data-stu-id="efda0-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="efda0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="efda0-131">Property</span></span> | <span data-ttu-id="efda0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="efda0-132">Type</span></span> | <span data-ttu-id="efda0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="efda0-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="efda0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="efda0-134">displayName</span></span> | <span data-ttu-id="efda0-135">string</span><span class="sxs-lookup"><span data-stu-id="efda0-135">string</span></span> | <span data-ttu-id="efda0-136">Имя для отображения в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="efda0-136">The name to display in the address book for the group.</span></span> <span data-ttu-id="efda0-137">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="efda0-137">Required.</span></span> |
| <span data-ttu-id="efda0-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="efda0-138">mailEnabled</span></span> | <span data-ttu-id="efda0-139">boolean</span><span class="sxs-lookup"><span data-stu-id="efda0-139">boolean</span></span> | <span data-ttu-id="efda0-140">Устанавливает значение **true** для групп с поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="efda0-140">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="efda0-141">Установите значение **true** при создании группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="efda0-141">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="efda0-142">Установите значение **false** при создании динамической группы или группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="efda0-142">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="efda0-143">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="efda0-143">Required.</span></span> |
| <span data-ttu-id="efda0-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="efda0-144">mailNickname</span></span> | <span data-ttu-id="efda0-145">string</span><span class="sxs-lookup"><span data-stu-id="efda0-145">string</span></span> | <span data-ttu-id="efda0-146">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="efda0-146">The mail alias for the group.</span></span> <span data-ttu-id="efda0-147">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="efda0-147">Required.</span></span> |
| <span data-ttu-id="efda0-148">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="efda0-148">securityEnabled</span></span> | <span data-ttu-id="efda0-149">boolean</span><span class="sxs-lookup"><span data-stu-id="efda0-149">boolean</span></span> | <span data-ttu-id="efda0-150">Значение **true** для групп с поддержкой безопасности.</span><span class="sxs-lookup"><span data-stu-id="efda0-150">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="efda0-151">Установите значение **true** при создании динамической группы или группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="efda0-151">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="efda0-152">Установите значение **false**при создании группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="efda0-152">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="efda0-153">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="efda0-153">Required.</span></span> |
| <span data-ttu-id="efda0-154">владельцы</span><span class="sxs-lookup"><span data-stu-id="efda0-154">owners</span></span> | <span data-ttu-id="efda0-155">коллекция строк</span><span class="sxs-lookup"><span data-stu-id="efda0-155">string collection</span></span> | <span data-ttu-id="efda0-156">Это свойство представляет владельцев группы во время создания.</span><span class="sxs-lookup"><span data-stu-id="efda0-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="efda0-157">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="efda0-157">Optional.</span></span> |
| <span data-ttu-id="efda0-158">члены</span><span class="sxs-lookup"><span data-stu-id="efda0-158">members</span></span> | <span data-ttu-id="efda0-159">коллекция строк</span><span class="sxs-lookup"><span data-stu-id="efda0-159">string collection</span></span> | <span data-ttu-id="efda0-160">Это свойство представляет членов группы во время создания.</span><span class="sxs-lookup"><span data-stu-id="efda0-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="efda0-161">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="efda0-161">Optional.</span></span> |


<span data-ttu-id="efda0-162">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="efda0-162">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="efda0-163">Параметры groupTypes</span><span class="sxs-lookup"><span data-stu-id="efda0-163">groupTypes options</span></span>

| <span data-ttu-id="efda0-164">Тип группы</span><span class="sxs-lookup"><span data-stu-id="efda0-164">Type of group</span></span> | <span data-ttu-id="efda0-165">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="efda0-165">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="efda0-166">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="efda0-166">Office 365 (aka unified group)</span></span>| <span data-ttu-id="efda0-167">"Unified"</span><span class="sxs-lookup"><span data-stu-id="efda0-167">"Unified"</span></span> |
| <span data-ttu-id="efda0-168">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="efda0-168">Dynamic</span></span> | <span data-ttu-id="efda0-169">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="efda0-169">"DynamicMembership"</span></span> |
| <span data-ttu-id="efda0-170">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="efda0-170">Security</span></span> | <span data-ttu-id="efda0-171">Не следует устанавливать.</span><span class="sxs-lookup"><span data-stu-id="efda0-171">Do not set.</span></span> |


><span data-ttu-id="efda0-172">**Примечание.** При создании группы Office 365 программными средствами без контекста пользователя и указания владельцев будет создана анонимная группа.</span><span class="sxs-lookup"><span data-stu-id="efda0-172">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="efda0-173">Это может привести к тому, что связанный сайт SharePoint Online не будет создаваться автоматически, пока не будут вручную предприняты дальнейшие действия.</span><span class="sxs-lookup"><span data-stu-id="efda0-173">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="efda0-p112">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="efda0-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="efda0-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="efda0-176">Response</span></span>
<span data-ttu-id="efda0-177">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efda0-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efda0-178">Пример</span><span class="sxs-lookup"><span data-stu-id="efda0-178">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="efda0-179">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="efda0-179">Request 1</span></span>
<span data-ttu-id="efda0-180">В первом примере запроса создается группа Office 365.</span><span class="sxs-lookup"><span data-stu-id="efda0-180">The following is an example of a request that creates an Office 365 Group.</span></span>
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

#### <a name="response-1"></a><span data-ttu-id="efda0-181">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="efda0-181">Response 1</span></span>
<span data-ttu-id="efda0-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="efda0-182">The following is an example of the response.</span></span>
><span data-ttu-id="efda0-p113">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efda0-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="efda0-185">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="efda0-185">Request 2</span></span>
<span data-ttu-id="efda0-186">Во втором примере запроса создается группа Office 365 с указанными владельцами.</span><span class="sxs-lookup"><span data-stu-id="efda0-186">The second example request creates an Office 365 Group with owners specified.</span></span>
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

#### <a name="response-2"></a><span data-ttu-id="efda0-187">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="efda0-187">Response 2</span></span>
<span data-ttu-id="efda0-188">Ниже приведен пример успешного отклика.</span><span class="sxs-lookup"><span data-stu-id="efda0-188">The following is an example of the response.</span></span>
><span data-ttu-id="efda0-p114">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efda0-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
