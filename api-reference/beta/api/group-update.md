---
title: Обновление группы
description: Обновление свойств [группового](../resources/group.md) объекта.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 35f9243eb0aa6ecb21447fdb7550b07bf73efdb4
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316869"
---
# <a name="update-group"></a><span data-ttu-id="69841-103">Update group</span><span class="sxs-lookup"><span data-stu-id="69841-103">Update group</span></span>

<span data-ttu-id="69841-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69841-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69841-105">Обновление свойств [группового](../resources/group.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="69841-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="69841-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69841-106">Permissions</span></span>

<span data-ttu-id="69841-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69841-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69841-109">Permission type</span></span>      | <span data-ttu-id="69841-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69841-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69841-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69841-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69841-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="69841-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="69841-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69841-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69841-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69841-114">Not supported.</span></span>    |
|<span data-ttu-id="69841-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69841-115">Application</span></span> | <span data-ttu-id="69841-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69841-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69841-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69841-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="69841-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69841-118">Request headers</span></span>

| <span data-ttu-id="69841-119">Имя</span><span class="sxs-lookup"><span data-stu-id="69841-119">Name</span></span>       | <span data-ttu-id="69841-120">Тип</span><span class="sxs-lookup"><span data-stu-id="69841-120">Type</span></span> | <span data-ttu-id="69841-121">Описание</span><span class="sxs-lookup"><span data-stu-id="69841-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="69841-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69841-122">Authorization</span></span>  | <span data-ttu-id="69841-123">string</span><span class="sxs-lookup"><span data-stu-id="69841-123">string</span></span>  | <span data-ttu-id="69841-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69841-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69841-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69841-126">Request body</span></span>

<span data-ttu-id="69841-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="69841-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="69841-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="69841-130">Property</span></span>   | <span data-ttu-id="69841-131">Тип</span><span class="sxs-lookup"><span data-stu-id="69841-131">Type</span></span> |<span data-ttu-id="69841-132">Описание</span><span class="sxs-lookup"><span data-stu-id="69841-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69841-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="69841-133">allowExternalSenders</span></span>|<span data-ttu-id="69841-134">Логический</span><span class="sxs-lookup"><span data-stu-id="69841-134">Boolean</span></span>|<span data-ttu-id="69841-p104">Значение по умолчанию: `false`. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="69841-p104">Default is `false`. Indicates whether people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="69841-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="69841-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="69841-138">Логический</span><span class="sxs-lookup"><span data-stu-id="69841-138">Boolean</span></span>|<span data-ttu-id="69841-139">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="69841-139">Default is `false`.</span></span> <span data-ttu-id="69841-140">Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="69841-140">Indicates whether new members added to the group will be auto-subscribed to receive email notifications.</span></span> <span data-ttu-id="69841-141">**AutoSubscribeNewMembers** не может быть `true`, если в группе установлено `false` для **subscriptionEnabled**.</span><span class="sxs-lookup"><span data-stu-id="69841-141">**autoSubscribeNewMembers** can't be `true` when **subscriptionEnabled** is set to `false` on the group.</span></span>|
|<span data-ttu-id="69841-142">description</span><span class="sxs-lookup"><span data-stu-id="69841-142">description</span></span>|<span data-ttu-id="69841-143">String</span><span class="sxs-lookup"><span data-stu-id="69841-143">String</span></span>|<span data-ttu-id="69841-144">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="69841-144">An optional description for the group.</span></span>|
|<span data-ttu-id="69841-145">displayName</span><span class="sxs-lookup"><span data-stu-id="69841-145">displayName</span></span>|<span data-ttu-id="69841-146">String</span><span class="sxs-lookup"><span data-stu-id="69841-146">String</span></span>|<span data-ttu-id="69841-p106">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления.</span><span class="sxs-lookup"><span data-stu-id="69841-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="69841-149">groupTypes</span><span class="sxs-lookup"><span data-stu-id="69841-149">groupTypes</span></span>|<span data-ttu-id="69841-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="69841-150">String collection</span></span>|<span data-ttu-id="69841-151">Задает тип группы и участие в ней.</span><span class="sxs-lookup"><span data-stu-id="69841-151">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="69841-152">Если коллекция содержит **Unified,** то группа является Microsoft 365 группой; в противном случае это группа безопасности.</span><span class="sxs-lookup"><span data-stu-id="69841-152">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise, it's a security group.</span></span>  <br><br><span data-ttu-id="69841-153">Если коллекция включает объект **DynamicMembership**, то в этой группе используется динамическое членство. В противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="69841-153">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="69841-154">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="69841-154">mailEnabled</span></span>|<span data-ttu-id="69841-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="69841-155">Boolean</span></span>|<span data-ttu-id="69841-156">Указывает, включена ли для этой группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="69841-156">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="69841-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="69841-157">mailNickname</span></span>|<span data-ttu-id="69841-158">String</span><span class="sxs-lookup"><span data-stu-id="69841-158">String</span></span>|<span data-ttu-id="69841-p107">Почтовый псевдоним для группы. Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="69841-p107">The mail alias for the group. This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="69841-161">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="69841-161">securityEnabled</span></span>|<span data-ttu-id="69841-162">Логический</span><span class="sxs-lookup"><span data-stu-id="69841-162">Boolean</span></span>|<span data-ttu-id="69841-163">Указывает, является ли группа группой безопасности, в том числе Microsoft 365 группами.</span><span class="sxs-lookup"><span data-stu-id="69841-163">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="69841-164">visibility</span><span class="sxs-lookup"><span data-stu-id="69841-164">visibility</span></span>|<span data-ttu-id="69841-165">String</span><span class="sxs-lookup"><span data-stu-id="69841-165">String</span></span>|<span data-ttu-id="69841-166">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="69841-166">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="69841-167">Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="69841-167">Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="69841-168">Поскольку **ресурс группы** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` группы. </span><span class="sxs-lookup"><span data-stu-id="69841-168">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="69841-169">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="69841-169">**Note:**</span></span>
>
> - <span data-ttu-id="69841-170">Чтобы обновить следующие свойства Exchange, необходимо указать их в собственном запросе PATCH, не включая другие свойства, перечисленные в таблице выше: **allowExternalSenders,** **autoSubscribeNewMembers,** **hideFromAddressLists,** **hideFromOutlookClients,** **isSubscribedByMail**, **unseenCount**.</span><span class="sxs-lookup"><span data-stu-id="69841-170">To update the following Exchange-specific properties, you must specify them in their own PATCH request, without including the other properties listed in the table above: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>
> - <span data-ttu-id="69841-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](/graph/known-issues#group).</span><span class="sxs-lookup"><span data-stu-id="69841-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#group) for examples.</span></span>
> - <span data-ttu-id="69841-174">Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="69841-174">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="69841-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="69841-175">Response</span></span>

<span data-ttu-id="69841-176">В случае успеха этот метод возвращает код отклика `204 No Content`, за исключением кода отклика `200 OK` при обновлении следующих свойств: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span><span class="sxs-lookup"><span data-stu-id="69841-176">If successful, this method returns a `204 No Content` response code—except a `200 OK` response code when updating the following properties: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>

## <a name="examples"></a><span data-ttu-id="69841-177">Примеры</span><span class="sxs-lookup"><span data-stu-id="69841-177">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="69841-178">Пример 1. Обновление имени отображения и описания группы</span><span class="sxs-lookup"><span data-stu-id="69841-178">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="69841-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="69841-179">Request</span></span>

<span data-ttu-id="69841-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69841-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="69841-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="69841-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json

{
   "description":"Contoso Life v2.0",
   "displayName":"Contoso Life Renewed"
}
```
# <a name="c"></a>[<span data-ttu-id="69841-182">C#</span><span class="sxs-lookup"><span data-stu-id="69841-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69841-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69841-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69841-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69841-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69841-185">Java</span><span class="sxs-lookup"><span data-stu-id="69841-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="69841-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="69841-186">Response</span></span>

<span data-ttu-id="69841-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="69841-187">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="69841-188">Пример 2. Применение метки конфиденциальности к группе Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="69841-188">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="69841-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="69841-189">Request</span></span>

<span data-ttu-id="69841-190">Вы можете получить ID метки, которая будет применяться к группе Microsoft 365 с помощью [метки List.](informationprotectionpolicy-list-labels.md)</span><span class="sxs-lookup"><span data-stu-id="69841-190">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="69841-191">Затем вы можете обновить свойство [назначенногоLabels](../resources/assignedlabel.md) группы с помощью ID метки.</span><span class="sxs-lookup"><span data-stu-id="69841-191">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 


# <a name="http"></a>[<span data-ttu-id="69841-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="69841-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "assignedLabels": 
  [
    {
        "labelId" : "45cd0c48-c540-4358-ad79-a3658cdc5b88"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="69841-193">C#</span><span class="sxs-lookup"><span data-stu-id="69841-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69841-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69841-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69841-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69841-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69841-196">Java</span><span class="sxs-lookup"><span data-stu-id="69841-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="69841-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="69841-197">Response</span></span>

<span data-ttu-id="69841-198">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="69841-198">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="69841-199">См. также</span><span class="sxs-lookup"><span data-stu-id="69841-199">See also</span></span>

- [<span data-ttu-id="69841-200">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="69841-200">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="69841-201">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="69841-201">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="69841-202">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="69841-202">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
