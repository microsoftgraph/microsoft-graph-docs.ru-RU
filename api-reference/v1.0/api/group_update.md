# <a name="update-group"></a><span data-ttu-id="ae498-101">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="ae498-101">Update group</span></span>
<span data-ttu-id="ae498-102">Обновление свойств, принадлежащих объекту группы.</span><span class="sxs-lookup"><span data-stu-id="ae498-102">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae498-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae498-103">Permissions</span></span>
<span data-ttu-id="ae498-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae498-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae498-106">Permission type</span></span>      | <span data-ttu-id="ae498-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae498-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae498-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae498-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ae498-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae498-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae498-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae498-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae498-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae498-111">Not supported.</span></span>    |
|<span data-ttu-id="ae498-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae498-112">Application</span></span> | <span data-ttu-id="ae498-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae498-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae498-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae498-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ae498-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae498-115">Request headers</span></span>

| <span data-ttu-id="ae498-116">Имя</span><span class="sxs-lookup"><span data-stu-id="ae498-116">Name</span></span>       | <span data-ttu-id="ae498-117">Тип</span><span class="sxs-lookup"><span data-stu-id="ae498-117">Type</span></span> | <span data-ttu-id="ae498-118">Описание</span><span class="sxs-lookup"><span data-stu-id="ae498-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae498-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae498-119">Authorization</span></span>  | <span data-ttu-id="ae498-120">string</span><span class="sxs-lookup"><span data-stu-id="ae498-120">string</span></span>  | <span data-ttu-id="ae498-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae498-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae498-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae498-123">Request body</span></span>

<span data-ttu-id="ae498-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ae498-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ae498-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae498-127">Property</span></span>     | <span data-ttu-id="ae498-128">Тип</span><span class="sxs-lookup"><span data-stu-id="ae498-128">Type</span></span>   |<span data-ttu-id="ae498-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ae498-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae498-130">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="ae498-130">autoSubscribeNewMembers</span></span>|<span data-ttu-id="ae498-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae498-131">Boolean</span></span>|<span data-ttu-id="ae498-p104">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="ae498-p104">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="ae498-134">description</span><span class="sxs-lookup"><span data-stu-id="ae498-134">description</span></span>|<span data-ttu-id="ae498-135">String</span><span class="sxs-lookup"><span data-stu-id="ae498-135">String</span></span>|<span data-ttu-id="ae498-136">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="ae498-136">An optional description for the group.</span></span> |
|<span data-ttu-id="ae498-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ae498-137">displayName</span></span>|<span data-ttu-id="ae498-138">String</span><span class="sxs-lookup"><span data-stu-id="ae498-138">String</span></span>|<span data-ttu-id="ae498-p105">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="ae498-p105">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="ae498-142">groupTypes</span><span class="sxs-lookup"><span data-stu-id="ae498-142">groupTypes</span></span>|<span data-ttu-id="ae498-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ae498-143">String collection</span></span>|<span data-ttu-id="ae498-p106">Указывает тип создаваемой группы. Возможные значения: **Unified** для создания группы Office 365 или **DynamicMembership** для создания динамических групп.  Для остальных типов групп, таких как группы безопасности и поддерживающие почту группы безопасности, это свойство не задается.</span><span class="sxs-lookup"><span data-stu-id="ae498-p106">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="ae498-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="ae498-147">mailEnabled</span></span>|<span data-ttu-id="ae498-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae498-148">Boolean</span></span>|<span data-ttu-id="ae498-p107">Указывает, включена ли для этой группы поддержка почты. Если для свойства **securityEnabled** также задано значение **true**, это группа безопасности с включенной поддержкой почты. В противном случае это группа рассылки Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae498-p107">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="ae498-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ae498-151">mailNickname</span></span>|<span data-ttu-id="ae498-152">String</span><span class="sxs-lookup"><span data-stu-id="ae498-152">String</span></span>|<span data-ttu-id="ae498-p108">Почтовый псевдоним для группы. Это свойство должно быть указано при создании группы. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="ae498-p108">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="ae498-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="ae498-156">securityEnabled</span></span>|<span data-ttu-id="ae498-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae498-157">Boolean</span></span>|<span data-ttu-id="ae498-p109">Указывает, является ли эта группа группой безопасности. Если для свойства **mailEnabled** также задано значение true, эта группа является группой безопасности, поддерживающей почту; в противном случае — это группа безопасности. Для групп Office 365 должно быть задано значение **false**. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="ae498-p109">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="ae498-162">visibility</span><span class="sxs-lookup"><span data-stu-id="ae498-162">visibility</span></span>|<span data-ttu-id="ae498-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae498-163">Boolean</span></span>|<span data-ttu-id="ae498-p110">Определяет видимость группы Office 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="ae498-p110">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="ae498-166">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="ae498-166">**Note**</span></span>

- <span data-ttu-id="ae498-167">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="ae498-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="ae498-p111">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="ae498-p111">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="ae498-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae498-171">Response</span></span>
<span data-ttu-id="ae498-172">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ae498-172">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ae498-173">Пример</span><span class="sxs-lookup"><span data-stu-id="ae498-173">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ae498-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae498-174">Request</span></span>
<span data-ttu-id="ae498-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae498-175">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```

#### <a name="response"></a><span data-ttu-id="ae498-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae498-176">Response</span></span>
<span data-ttu-id="ae498-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae498-177">The following is an example of the response.</span></span>
><span data-ttu-id="ae498-178">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ae498-178">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ae498-179">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae498-179">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->