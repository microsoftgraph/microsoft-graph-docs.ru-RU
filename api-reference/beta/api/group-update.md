---
title: Обновление группы
description: Обновление свойств объекта [Group](../resources/group.md) .
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d38fdab04f4f470ba9c712f4447ecae3aa7d79bb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895778"
---
# <a name="update-group"></a><span data-ttu-id="e8a7a-103">Update group</span><span class="sxs-lookup"><span data-stu-id="e8a7a-103">Update group</span></span>

<span data-ttu-id="e8a7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8a7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8a7a-105">Обновление свойств объекта [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="e8a7a-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8a7a-106">Permissions</span></span>

<span data-ttu-id="e8a7a-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e8a7a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8a7a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8a7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8a7a-109">Permission type</span></span>      | <span data-ttu-id="e8a7a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8a7a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8a7a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8a7a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e8a7a-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8a7a-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e8a7a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8a7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-114">Not supported.</span></span>    |
|<span data-ttu-id="e8a7a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8a7a-115">Application</span></span> | <span data-ttu-id="e8a7a-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a7a-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8a7a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8a7a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8a7a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8a7a-118">Request headers</span></span>

| <span data-ttu-id="e8a7a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e8a7a-119">Name</span></span>       | <span data-ttu-id="e8a7a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e8a7a-120">Type</span></span> | <span data-ttu-id="e8a7a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e8a7a-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8a7a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8a7a-122">Authorization</span></span>  | <span data-ttu-id="e8a7a-123">string</span><span class="sxs-lookup"><span data-stu-id="e8a7a-123">string</span></span>  | <span data-ttu-id="e8a7a-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-124">Bearer {token}.</span></span> <span data-ttu-id="e8a7a-125">Required.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8a7a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8a7a-126">Request body</span></span>

<span data-ttu-id="e8a7a-127">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e8a7a-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e8a7a-129">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e8a7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8a7a-130">Property</span></span>   | <span data-ttu-id="e8a7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e8a7a-131">Type</span></span> |<span data-ttu-id="e8a7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e8a7a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8a7a-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="e8a7a-133">allowExternalSenders</span></span>|<span data-ttu-id="e8a7a-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="e8a7a-134">Boolean</span></span>|<span data-ttu-id="e8a7a-135">Default is **false**.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-135">Default is **false**.</span></span> <span data-ttu-id="e8a7a-136">Indicates if people external to the organization can send messages to the group.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-136">Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="e8a7a-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="e8a7a-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="e8a7a-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8a7a-138">Boolean</span></span>|<span data-ttu-id="e8a7a-139">Default is **false**.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-139">Default is **false**.</span></span> <span data-ttu-id="e8a7a-140">Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-140">Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="e8a7a-141">description</span><span class="sxs-lookup"><span data-stu-id="e8a7a-141">description</span></span>|<span data-ttu-id="e8a7a-142">String</span><span class="sxs-lookup"><span data-stu-id="e8a7a-142">String</span></span>|<span data-ttu-id="e8a7a-143">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-143">An optional description for the group.</span></span> |
|<span data-ttu-id="e8a7a-144">displayName</span><span class="sxs-lookup"><span data-stu-id="e8a7a-144">displayName</span></span>|<span data-ttu-id="e8a7a-145">String</span><span class="sxs-lookup"><span data-stu-id="e8a7a-145">String</span></span>|<span data-ttu-id="e8a7a-146">The display name for the group.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-146">The display name for the group.</span></span> <span data-ttu-id="e8a7a-147">This property is required when a group is created and it cannot be cleared during updates.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-147">This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="e8a7a-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="e8a7a-148">groupTypes</span></span>|<span data-ttu-id="e8a7a-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8a7a-149">String collection</span></span>|<span data-ttu-id="e8a7a-150">Задает тип группы и членства в ней.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-150">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="e8a7a-151">Если коллекция содержит **Unified** , то эта группа является группой Microsoft 365; в противном случае это группа безопасности.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-151">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="e8a7a-152">Если коллекция включает объект **DynamicMembership**, то в этой группе используется динамическое членство. В противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-152">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="e8a7a-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="e8a7a-153">mailEnabled</span></span>|<span data-ttu-id="e8a7a-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8a7a-154">Boolean</span></span>|<span data-ttu-id="e8a7a-155">Указывает, включена ли для этой группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-155">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="e8a7a-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="e8a7a-156">mailNickname</span></span>|<span data-ttu-id="e8a7a-157">String</span><span class="sxs-lookup"><span data-stu-id="e8a7a-157">String</span></span>|<span data-ttu-id="e8a7a-158">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-158">The mail alias for the group.</span></span> <span data-ttu-id="e8a7a-159">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-159">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="e8a7a-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="e8a7a-160">securityEnabled</span></span>|<span data-ttu-id="e8a7a-161">Логический</span><span class="sxs-lookup"><span data-stu-id="e8a7a-161">Boolean</span></span>|<span data-ttu-id="e8a7a-162">Указывает, является ли группа группой безопасности, включая группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-162">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="e8a7a-163">visibility</span><span class="sxs-lookup"><span data-stu-id="e8a7a-163">visibility</span></span>|<span data-ttu-id="e8a7a-164">String</span><span class="sxs-lookup"><span data-stu-id="e8a7a-164">String</span></span>|<span data-ttu-id="e8a7a-165">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-165">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="e8a7a-166">Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="e8a7a-166">Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="e8a7a-167">Так как ресурс **Group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции можно `PATCH` добавлять, обновлять или удалять собственные данные, зависящие от приложения, в настраиваемых свойствах расширения в существующем экземпляре **группы** .</span><span class="sxs-lookup"><span data-stu-id="e8a7a-167">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="e8a7a-168">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="e8a7a-168">**Note:**</span></span>
>
> - <span data-ttu-id="e8a7a-169">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-169">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="e8a7a-170">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-170">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions.</span></span> <span data-ttu-id="e8a7a-171">All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-171">All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions.</span></span> <span data-ttu-id="e8a7a-172">See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-172">See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="e8a7a-173">Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="e8a7a-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="e8a7a-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8a7a-174">Response</span></span>

<span data-ttu-id="e8a7a-175">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e8a7a-176">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8a7a-176">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="e8a7a-177">Пример 1: обновление отображаемого имени и описания группы</span><span class="sxs-lookup"><span data-stu-id="e8a7a-177">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="e8a7a-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8a7a-178">Request</span></span>

<span data-ttu-id="e8a7a-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e8a7a-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8a7a-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="e8a7a-181">C#</span><span class="sxs-lookup"><span data-stu-id="e8a7a-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8a7a-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8a7a-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8a7a-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8a7a-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e8a7a-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8a7a-184">Response</span></span>

<span data-ttu-id="e8a7a-185">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-185">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="e8a7a-186">Пример 2: применение метки конфиденциальности к группе Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e8a7a-186">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="e8a7a-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8a7a-187">Request</span></span>

<span data-ttu-id="e8a7a-188">Вы можете получить идентификатор метки, которую нужно применить к группе Microsoft 365, с помощью [метки списка](informationprotectionpolicy-list-labels.md).</span><span class="sxs-lookup"><span data-stu-id="e8a7a-188">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="e8a7a-189">После этого можно обновить свойство [ассигнедлабелс](../resources/assignedlabel.md) группы, указав идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-189">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_group"
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

#### <a name="response"></a><span data-ttu-id="e8a7a-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8a7a-190">Response</span></span>

<span data-ttu-id="e8a7a-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8a7a-191">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="e8a7a-192">См. также</span><span class="sxs-lookup"><span data-stu-id="e8a7a-192">See also</span></span>

- [<span data-ttu-id="e8a7a-193">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e8a7a-193">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e8a7a-194">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e8a7a-194">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e8a7a-195">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e8a7a-195">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
