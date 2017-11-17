# <a name="create-group"></a><span data-ttu-id="9a525-101">Создание группы</span><span class="sxs-lookup"><span data-stu-id="9a525-101">Create group</span></span>

<span data-ttu-id="9a525-p101">Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:</span><span class="sxs-lookup"><span data-stu-id="9a525-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="9a525-104">Группа Office 365 (единая группа)</span><span class="sxs-lookup"><span data-stu-id="9a525-104">Office 365 group (unified group)</span></span>
* <span data-ttu-id="9a525-105">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="9a525-105">Dynamic group</span></span>
* <span data-ttu-id="9a525-106">Группа безопасности</span><span class="sxs-lookup"><span data-stu-id="9a525-106">Security group</span></span>

> <span data-ttu-id="9a525-p102">**Примечание.** Несмотря на то что Microsoft Teams создан на основе групп Office 365, в настоящее время нельзя создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9a525-p102">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a525-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a525-109">Permissions</span></span>
<span data-ttu-id="9a525-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a525-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a525-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a525-112">Permission type</span></span>      | <span data-ttu-id="9a525-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a525-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a525-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a525-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9a525-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a525-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a525-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a525-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a525-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a525-117">Not supported.</span></span>    |
|<span data-ttu-id="9a525-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a525-118">Application</span></span> | <span data-ttu-id="9a525-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a525-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a525-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a525-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```
## <a name="request-headers"></a><span data-ttu-id="9a525-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a525-121">Request headers</span></span>
| <span data-ttu-id="9a525-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9a525-122">Name</span></span>       | <span data-ttu-id="9a525-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9a525-123">Type</span></span> | <span data-ttu-id="9a525-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9a525-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a525-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a525-125">Authorization</span></span>  | <span data-ttu-id="9a525-126">string</span><span class="sxs-lookup"><span data-stu-id="9a525-126">string</span></span>  | <span data-ttu-id="9a525-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a525-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a525-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a525-129">Request body</span></span>
<span data-ttu-id="9a525-130">В таблице ниже представлены свойства ресурса [group](../resources/group.md), который необходимо указать по крайней мере при создании группы.</span><span class="sxs-lookup"><span data-stu-id="9a525-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="9a525-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a525-131">Property</span></span> | <span data-ttu-id="9a525-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9a525-132">Type</span></span> | <span data-ttu-id="9a525-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9a525-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a525-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9a525-134">displayName</span></span> | <span data-ttu-id="9a525-135">string</span><span class="sxs-lookup"><span data-stu-id="9a525-135">string</span></span> | <span data-ttu-id="9a525-136">Имя, которое следует отобразить в адресной книге для группы.</span><span class="sxs-lookup"><span data-stu-id="9a525-136">The name to display in the address book for the group.</span></span> |
| <span data-ttu-id="9a525-137">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="9a525-137">mailEnabled</span></span> | <span data-ttu-id="9a525-138">boolean</span><span class="sxs-lookup"><span data-stu-id="9a525-138">boolean</span></span> | <span data-ttu-id="9a525-p105">Устанавливает значение **true** для групп с включенной поддержкой почты. Установите значение **true** при создании группы Office 365. При создании динамической группы или группы безопасности установите для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="9a525-p105">Set to **true** for mail-enabled groups. Set this to **true** if creating an Office 365 group. Set this to **false** if creating dynamic or security group.</span></span>|
| <span data-ttu-id="9a525-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9a525-142">mailNickname</span></span> | <span data-ttu-id="9a525-143">string</span><span class="sxs-lookup"><span data-stu-id="9a525-143">string</span></span> | <span data-ttu-id="9a525-144">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="9a525-144">The mail alias for the group.</span></span> |
| <span data-ttu-id="9a525-145">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="9a525-145">securityEnabled</span></span> | <span data-ttu-id="9a525-146">boolean</span><span class="sxs-lookup"><span data-stu-id="9a525-146">boolean</span></span> | <span data-ttu-id="9a525-p106">Устанавливает значение **true** для групп безопасности. При создании динамической группы или группы безопасности установите для этого свойства значение **true**. Устанавливает значение **false** при создании группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="9a525-p106">Set to **true** for security-enabled groups. Set this to **true** if creating a dynamic or security group. Set this to **false** if creating an Office 365 group.</span></span> |

<span data-ttu-id="9a525-150">При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.</span><span class="sxs-lookup"><span data-stu-id="9a525-150">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="9a525-151">Тип группы</span><span class="sxs-lookup"><span data-stu-id="9a525-151">Type of group</span></span> | <span data-ttu-id="9a525-152">Свойство **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="9a525-152">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="9a525-153">Office 365 (как единая группа)</span><span class="sxs-lookup"><span data-stu-id="9a525-153">Office 365 (aka unified group)</span></span>| <span data-ttu-id="9a525-154">"Unified"</span><span class="sxs-lookup"><span data-stu-id="9a525-154">"Unified"</span></span> |
| <span data-ttu-id="9a525-155">Динамическая группа</span><span class="sxs-lookup"><span data-stu-id="9a525-155">Dynamic</span></span> | <span data-ttu-id="9a525-156">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="9a525-156">"DynamicMembership"</span></span> |
| <span data-ttu-id="9a525-157">Система безопасности</span><span class="sxs-lookup"><span data-stu-id="9a525-157">Security</span></span> | <span data-ttu-id="9a525-158">Не следует устанавливать.</span><span class="sxs-lookup"><span data-stu-id="9a525-158">Do not set.</span></span> |

<span data-ttu-id="9a525-p107">При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="9a525-p107">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="9a525-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a525-161">Response</span></span>

<span data-ttu-id="9a525-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a525-162">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a525-163">Пример</span><span class="sxs-lookup"><span data-stu-id="9a525-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a525-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a525-164">Request</span></span>
<span data-ttu-id="9a525-165">Ознакомьтесь с примером запроса, создающего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="9a525-165">Here is an example of a request that creates an Office 365 group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
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

##### <a name="response"></a><span data-ttu-id="9a525-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a525-166">Response</span></span>
<span data-ttu-id="9a525-p108">Ниже приведен пример отклика. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будет возвращено больше свойств.</span><span class="sxs-lookup"><span data-stu-id="9a525-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. More properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
