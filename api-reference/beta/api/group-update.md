---
title: Обновление группы
description: Обновление свойств [группового](../resources/group.md) объекта.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 13d605efafb3d74cbaa78d79fb7fc634168b016a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468865"
---
# <a name="update-group"></a><span data-ttu-id="c36fc-103">Update group</span><span class="sxs-lookup"><span data-stu-id="c36fc-103">Update group</span></span>

<span data-ttu-id="c36fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c36fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c36fc-105">Обновление свойств [группового](../resources/group.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="c36fc-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c36fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c36fc-106">Permissions</span></span>

<span data-ttu-id="c36fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c36fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c36fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c36fc-109">Permission type</span></span>      | <span data-ttu-id="c36fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c36fc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c36fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c36fc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c36fc-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c36fc-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="c36fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c36fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c36fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c36fc-114">Not supported.</span></span>    |
|<span data-ttu-id="c36fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c36fc-115">Application</span></span> | <span data-ttu-id="c36fc-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36fc-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c36fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c36fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c36fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c36fc-118">Request headers</span></span>

| <span data-ttu-id="c36fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c36fc-119">Name</span></span>       | <span data-ttu-id="c36fc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c36fc-120">Type</span></span> | <span data-ttu-id="c36fc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c36fc-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c36fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c36fc-122">Authorization</span></span>  | <span data-ttu-id="c36fc-123">string</span><span class="sxs-lookup"><span data-stu-id="c36fc-123">string</span></span>  | <span data-ttu-id="c36fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c36fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c36fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c36fc-126">Request body</span></span>

<span data-ttu-id="c36fc-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c36fc-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c36fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c36fc-130">Property</span></span>   | <span data-ttu-id="c36fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c36fc-131">Type</span></span> |<span data-ttu-id="c36fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c36fc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c36fc-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="c36fc-133">allowExternalSenders</span></span>|<span data-ttu-id="c36fc-134">Логический</span><span class="sxs-lookup"><span data-stu-id="c36fc-134">Boolean</span></span>|<span data-ttu-id="c36fc-135">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="c36fc-135">Default is `false`.</span></span> <span data-ttu-id="c36fc-136">Указывает, могут ли внешние люди в организации отправлять сообщения группе.</span><span class="sxs-lookup"><span data-stu-id="c36fc-136">Indicates whether people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="c36fc-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="c36fc-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="c36fc-138">Логический</span><span class="sxs-lookup"><span data-stu-id="c36fc-138">Boolean</span></span>|<span data-ttu-id="c36fc-139">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="c36fc-139">Default is `false`.</span></span> <span data-ttu-id="c36fc-140">Указывает, будут ли новые участники, добавленные в группу, автоматически подписываться на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="c36fc-140">Indicates whether new members added to the group will be auto-subscribed to receive email notifications.</span></span> <span data-ttu-id="c36fc-141">**AutoSubscribeNewMembers** не может быть, если задаваемый `true` для группы **subscriptionEnabled.** `false`</span><span class="sxs-lookup"><span data-stu-id="c36fc-141">**autoSubscribeNewMembers** can't be `true` when **subscriptionEnabled** is set to `false` on the group.</span></span>|
|<span data-ttu-id="c36fc-142">description</span><span class="sxs-lookup"><span data-stu-id="c36fc-142">description</span></span>|<span data-ttu-id="c36fc-143">String</span><span class="sxs-lookup"><span data-stu-id="c36fc-143">String</span></span>|<span data-ttu-id="c36fc-144">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="c36fc-144">An optional description for the group.</span></span>|
|<span data-ttu-id="c36fc-145">description</span><span class="sxs-lookup"><span data-stu-id="c36fc-145">description</span></span>|<span data-ttu-id="c36fc-146">String</span><span class="sxs-lookup"><span data-stu-id="c36fc-146">String</span></span>|<span data-ttu-id="c36fc-147">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="c36fc-147">An optional description for the group.</span></span> |
|<span data-ttu-id="c36fc-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c36fc-148">displayName</span></span>|<span data-ttu-id="c36fc-149">String</span><span class="sxs-lookup"><span data-stu-id="c36fc-149">String</span></span>|<span data-ttu-id="c36fc-p106">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления.</span><span class="sxs-lookup"><span data-stu-id="c36fc-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="c36fc-152">groupTypes</span><span class="sxs-lookup"><span data-stu-id="c36fc-152">groupTypes</span></span>|<span data-ttu-id="c36fc-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c36fc-153">String collection</span></span>|<span data-ttu-id="c36fc-154">Задает тип группы и участие в ней.</span><span class="sxs-lookup"><span data-stu-id="c36fc-154">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="c36fc-155">Если коллекция содержит объект **Unified**, эта группа является группой Microsoft 365. В противном случае она является группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="c36fc-155">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="c36fc-156">Если коллекция включает объект **DynamicMembership**, то в этой группе используется динамическое членство. В противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="c36fc-156">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="c36fc-157">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="c36fc-157">mailEnabled</span></span>|<span data-ttu-id="c36fc-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c36fc-158">Boolean</span></span>|<span data-ttu-id="c36fc-159">Указывает, включена ли для этой группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="c36fc-159">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="c36fc-160">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c36fc-160">mailNickname</span></span>|<span data-ttu-id="c36fc-161">String</span><span class="sxs-lookup"><span data-stu-id="c36fc-161">String</span></span>|<span data-ttu-id="c36fc-162">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="c36fc-162">The mail alias for the group.</span></span> <span data-ttu-id="c36fc-163">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="c36fc-163">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="c36fc-164">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="c36fc-164">securityEnabled</span></span>|<span data-ttu-id="c36fc-165">Логический</span><span class="sxs-lookup"><span data-stu-id="c36fc-165">Boolean</span></span>|<span data-ttu-id="c36fc-166">Указывает, является ли группа группой безопасности, включая группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c36fc-166">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="c36fc-167">visibility</span><span class="sxs-lookup"><span data-stu-id="c36fc-167">visibility</span></span>|<span data-ttu-id="c36fc-168">String</span><span class="sxs-lookup"><span data-stu-id="c36fc-168">String</span></span>|<span data-ttu-id="c36fc-169">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c36fc-169">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="c36fc-170">Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="c36fc-170">Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="c36fc-171">Поскольку **ресурс группы** поддерживает [расширения,](/graph/extensibility-overview)вы можете использовать операцию для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` группы. </span><span class="sxs-lookup"><span data-stu-id="c36fc-171">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="c36fc-172">**Примечание:**</span><span class="sxs-lookup"><span data-stu-id="c36fc-172">**Note:**</span></span>
>
> - <span data-ttu-id="c36fc-173">Вы можете обновить **allowExternalSenders** и **autoSubscribeNewMembers,** указав их в собственном запросе PATCH без указания других свойств в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="c36fc-173">You can update **allowExternalSenders** and **autoSubscribeNewMembers** by specifying them in their own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="c36fc-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](/graph/known-issues#group).</span><span class="sxs-lookup"><span data-stu-id="c36fc-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#group) for examples.</span></span>
> - <span data-ttu-id="c36fc-177">Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="c36fc-177">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="c36fc-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="c36fc-178">Response</span></span>

<span data-ttu-id="c36fc-179">В случае успеха этот метод возвращает код отклика, за исключением кода ответа при обновлении следующих `204 No Content` `200 OK` свойств: **allowExternalSenders,** **autoSubscribeNewMembers,** **hideFromAddressLists,** **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span><span class="sxs-lookup"><span data-stu-id="c36fc-179">If successful, this method returns a `204 No Content` response code—except a `200 OK` response code when updating the following properties: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>

## <a name="examples"></a><span data-ttu-id="c36fc-180">Примеры</span><span class="sxs-lookup"><span data-stu-id="c36fc-180">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="c36fc-181">Пример 1. Обновление имени отображения и описания группы</span><span class="sxs-lookup"><span data-stu-id="c36fc-181">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="c36fc-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="c36fc-182">Request</span></span>

<span data-ttu-id="c36fc-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c36fc-183">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c36fc-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="c36fc-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_1"
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
# <a name="c"></a>[<span data-ttu-id="c36fc-185">C#</span><span class="sxs-lookup"><span data-stu-id="c36fc-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c36fc-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c36fc-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c36fc-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c36fc-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c36fc-188">Java</span><span class="sxs-lookup"><span data-stu-id="c36fc-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c36fc-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="c36fc-189">Response</span></span>

<span data-ttu-id="c36fc-190">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c36fc-190">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="c36fc-191">Пример 2. Применение метки конфиденциальности к группе Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c36fc-191">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="c36fc-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="c36fc-192">Request</span></span>

<span data-ttu-id="c36fc-193">Вы можете получить ID метки, которая будет применяться к группе Microsoft 365 с помощью [метки List.](informationprotectionpolicy-list-labels.md)</span><span class="sxs-lookup"><span data-stu-id="c36fc-193">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="c36fc-194">Затем вы можете обновить свойство [назначенногоLabels](../resources/assignedlabel.md) группы с помощью ID метки.</span><span class="sxs-lookup"><span data-stu-id="c36fc-194">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c36fc-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="c36fc-195">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c36fc-196">C#</span><span class="sxs-lookup"><span data-stu-id="c36fc-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c36fc-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c36fc-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c36fc-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c36fc-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c36fc-199">Java</span><span class="sxs-lookup"><span data-stu-id="c36fc-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c36fc-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="c36fc-200">Response</span></span>

<span data-ttu-id="c36fc-201">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c36fc-201">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="c36fc-202">См. также</span><span class="sxs-lookup"><span data-stu-id="c36fc-202">See also</span></span>

- [<span data-ttu-id="c36fc-203">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c36fc-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c36fc-204">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c36fc-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c36fc-205">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c36fc-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
