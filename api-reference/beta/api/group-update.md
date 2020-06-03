---
title: Обновление группы
description: Обновление свойств объекта [Group](../resources/group.md) .
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 98a2f1188cb86530414f3d8b3ed5a66296f27e32
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524541"
---
# <a name="update-group"></a><span data-ttu-id="9bd5d-103">Update group</span><span class="sxs-lookup"><span data-stu-id="9bd5d-103">Update group</span></span>

<span data-ttu-id="9bd5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bd5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd5d-105">Обновление свойств объекта [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="9bd5d-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bd5d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bd5d-106">Permissions</span></span>

<span data-ttu-id="9bd5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bd5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bd5d-109">Permission type</span></span>      | <span data-ttu-id="9bd5d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bd5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bd5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bd5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9bd5d-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9bd5d-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="9bd5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bd5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bd5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-114">Not supported.</span></span>    |
|<span data-ttu-id="9bd5d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bd5d-115">Application</span></span> | <span data-ttu-id="9bd5d-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bd5d-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bd5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bd5d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9bd5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bd5d-118">Request headers</span></span>

| <span data-ttu-id="9bd5d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9bd5d-119">Name</span></span>       | <span data-ttu-id="9bd5d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9bd5d-120">Type</span></span> | <span data-ttu-id="9bd5d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9bd5d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9bd5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bd5d-122">Authorization</span></span>  | <span data-ttu-id="9bd5d-123">string</span><span class="sxs-lookup"><span data-stu-id="9bd5d-123">string</span></span>  | <span data-ttu-id="9bd5d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bd5d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bd5d-126">Request body</span></span>

<span data-ttu-id="9bd5d-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9bd5d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bd5d-130">Property</span></span>   | <span data-ttu-id="9bd5d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9bd5d-131">Type</span></span> |<span data-ttu-id="9bd5d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9bd5d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bd5d-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="9bd5d-133">allowExternalSenders</span></span>|<span data-ttu-id="9bd5d-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="9bd5d-134">Boolean</span></span>|<span data-ttu-id="9bd5d-p104">Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="9bd5d-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="9bd5d-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="9bd5d-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd5d-138">Boolean</span></span>|<span data-ttu-id="9bd5d-p105">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="9bd5d-141">description</span><span class="sxs-lookup"><span data-stu-id="9bd5d-141">description</span></span>|<span data-ttu-id="9bd5d-142">String</span><span class="sxs-lookup"><span data-stu-id="9bd5d-142">String</span></span>|<span data-ttu-id="9bd5d-143">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-143">An optional description for the group.</span></span> |
|<span data-ttu-id="9bd5d-144">displayName</span><span class="sxs-lookup"><span data-stu-id="9bd5d-144">displayName</span></span>|<span data-ttu-id="9bd5d-145">String</span><span class="sxs-lookup"><span data-stu-id="9bd5d-145">String</span></span>|<span data-ttu-id="9bd5d-p106">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="9bd5d-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="9bd5d-148">groupTypes</span></span>|<span data-ttu-id="9bd5d-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9bd5d-149">String collection</span></span>|<span data-ttu-id="9bd5d-150">Задает тип группы и членства в ней.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-150">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="9bd5d-151">Если коллекция содержит объект **Unified**, то эта группа является группой Office 365. В противном случае она является группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-151">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="9bd5d-152">Если коллекция включает объект **DynamicMembership**, то в этой группе используется динамическое членство. В противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-152">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="9bd5d-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="9bd5d-153">mailEnabled</span></span>|<span data-ttu-id="9bd5d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bd5d-154">Boolean</span></span>|<span data-ttu-id="9bd5d-155">Указывает, включена ли для этой группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-155">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="9bd5d-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9bd5d-156">mailNickname</span></span>|<span data-ttu-id="9bd5d-157">String</span><span class="sxs-lookup"><span data-stu-id="9bd5d-157">String</span></span>|<span data-ttu-id="9bd5d-158">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-158">The mail alias for the group.</span></span> <span data-ttu-id="9bd5d-159">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-159">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="9bd5d-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="9bd5d-160">securityEnabled</span></span>|<span data-ttu-id="9bd5d-161">Логический</span><span class="sxs-lookup"><span data-stu-id="9bd5d-161">Boolean</span></span>|<span data-ttu-id="9bd5d-162">Указывает, является ли группа группой безопасности, в том числе группами Office 365.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-162">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="9bd5d-163">visibility</span><span class="sxs-lookup"><span data-stu-id="9bd5d-163">visibility</span></span>|<span data-ttu-id="9bd5d-164">String</span><span class="sxs-lookup"><span data-stu-id="9bd5d-164">String</span></span>|<span data-ttu-id="9bd5d-p108">Определяет видимость группы Office 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="9bd5d-167">Так как ресурс **Group** поддерживает [расширения](/graph/extensibility-overview), с помощью операции можно `PATCH` добавлять, обновлять или удалять собственные данные, зависящие от приложения, в настраиваемых свойствах расширения в существующем экземпляре **группы** .</span><span class="sxs-lookup"><span data-stu-id="9bd5d-167">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="9bd5d-168">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="9bd5d-168">**Note:**</span></span>
>
> - <span data-ttu-id="9bd5d-169">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-169">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="9bd5d-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="9bd5d-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="9bd5d-173">Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="9bd5d-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="9bd5d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bd5d-174">Response</span></span>

<span data-ttu-id="9bd5d-175">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9bd5d-176">Примеры</span><span class="sxs-lookup"><span data-stu-id="9bd5d-176">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="9bd5d-177">Пример 1: обновление отображаемого имени и описания группы</span><span class="sxs-lookup"><span data-stu-id="9bd5d-177">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="9bd5d-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bd5d-178">Request</span></span>

<span data-ttu-id="9bd5d-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9bd5d-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bd5d-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9bd5d-181">C#</span><span class="sxs-lookup"><span data-stu-id="9bd5d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bd5d-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bd5d-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bd5d-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bd5d-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9bd5d-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bd5d-184">Response</span></span>

<span data-ttu-id="9bd5d-185">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-185">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-an-office-365-group"></a><span data-ttu-id="9bd5d-186">Пример 2: применение метки конфиденциальности к группе Office 365</span><span class="sxs-lookup"><span data-stu-id="9bd5d-186">Example 2: Apply sensitivity label to an Office 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="9bd5d-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bd5d-187">Request</span></span>

<span data-ttu-id="9bd5d-188">Вы можете получить идентификатор метки, которую нужно применить к группе Office 365, с помощью [метки списка](informationprotectionpolicy-list-labels.md).</span><span class="sxs-lookup"><span data-stu-id="9bd5d-188">You can obtain the ID of the label you want to apply to an Office 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="9bd5d-189">После этого можно обновить свойство [ассигнедлабелс](../resources/assignedlabel.md) группы, указав идентификатор метки.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-189">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 

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

#### <a name="response"></a><span data-ttu-id="9bd5d-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bd5d-190">Response</span></span>

<span data-ttu-id="9bd5d-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bd5d-191">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="9bd5d-192">См. также</span><span class="sxs-lookup"><span data-stu-id="9bd5d-192">See also</span></span>

- [<span data-ttu-id="9bd5d-193">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9bd5d-193">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9bd5d-194">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9bd5d-194">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9bd5d-195">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9bd5d-195">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
