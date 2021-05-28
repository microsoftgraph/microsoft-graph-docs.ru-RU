---
title: Обновление группы
description: Обновление свойств объекта group.
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 36b8a21589bdfd1687939eb636bf5de254d37bab
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680740"
---
# <a name="update-group"></a><span data-ttu-id="d98bc-103">Update group</span><span class="sxs-lookup"><span data-stu-id="d98bc-103">Update group</span></span>

<span data-ttu-id="d98bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d98bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d98bc-105">Обновление свойств объекта group.</span><span class="sxs-lookup"><span data-stu-id="d98bc-105">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d98bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d98bc-106">Permissions</span></span>

<span data-ttu-id="d98bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d98bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d98bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d98bc-109">Permission type</span></span>      | <span data-ttu-id="d98bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d98bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d98bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d98bc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d98bc-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d98bc-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="d98bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d98bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d98bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d98bc-114">Not supported.</span></span>    |
|<span data-ttu-id="d98bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d98bc-115">Application</span></span> | <span data-ttu-id="d98bc-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98bc-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d98bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d98bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d98bc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d98bc-118">Request headers</span></span>

| <span data-ttu-id="d98bc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d98bc-119">Name</span></span>       | <span data-ttu-id="d98bc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d98bc-120">Type</span></span> | <span data-ttu-id="d98bc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d98bc-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d98bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d98bc-122">Authorization</span></span>  | <span data-ttu-id="d98bc-123">string</span><span class="sxs-lookup"><span data-stu-id="d98bc-123">string</span></span>  | <span data-ttu-id="d98bc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d98bc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d98bc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d98bc-126">Request body</span></span>

<span data-ttu-id="d98bc-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d98bc-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d98bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d98bc-130">Property</span></span>   | <span data-ttu-id="d98bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d98bc-131">Type</span></span> |<span data-ttu-id="d98bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d98bc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d98bc-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="d98bc-133">allowExternalSenders</span></span>|<span data-ttu-id="d98bc-134">Логический</span><span class="sxs-lookup"><span data-stu-id="d98bc-134">Boolean</span></span>|<span data-ttu-id="d98bc-135">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="d98bc-135">Default is `false`.</span></span> <span data-ttu-id="d98bc-136">Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="d98bc-136">Indicates whether people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="d98bc-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="d98bc-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="d98bc-138">Логический</span><span class="sxs-lookup"><span data-stu-id="d98bc-138">Boolean</span></span>|<span data-ttu-id="d98bc-139">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="d98bc-139">Default is `false`.</span></span> <span data-ttu-id="d98bc-140">Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="d98bc-140">Indicates whether new members added to the group will be auto-subscribed to receive email notifications.</span></span> <span data-ttu-id="d98bc-141">**AutoSubscribeNewMembers** не может быть `true`, если в группе установлено `false` для **subscriptionEnabled**.</span><span class="sxs-lookup"><span data-stu-id="d98bc-141">**autoSubscribeNewMembers** can't be `true` when **subscriptionEnabled** is set to `false` on the group.</span></span>|
|<span data-ttu-id="d98bc-142">description</span><span class="sxs-lookup"><span data-stu-id="d98bc-142">description</span></span>|<span data-ttu-id="d98bc-143">String</span><span class="sxs-lookup"><span data-stu-id="d98bc-143">String</span></span>|<span data-ttu-id="d98bc-144">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="d98bc-144">An optional description for the group.</span></span> |
|<span data-ttu-id="d98bc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d98bc-145">displayName</span></span>|<span data-ttu-id="d98bc-146">String</span><span class="sxs-lookup"><span data-stu-id="d98bc-146">String</span></span>|<span data-ttu-id="d98bc-p106">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления.</span><span class="sxs-lookup"><span data-stu-id="d98bc-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="d98bc-149">groupTypes</span><span class="sxs-lookup"><span data-stu-id="d98bc-149">groupTypes</span></span>|<span data-ttu-id="d98bc-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d98bc-150">String collection</span></span>|<span data-ttu-id="d98bc-151">Задает тип группы и участие в ней.</span><span class="sxs-lookup"><span data-stu-id="d98bc-151">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="d98bc-152">Если коллекция содержит объект **Unified**, эта группа является группой Microsoft 365. В противном случае она является группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="d98bc-152">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="d98bc-153">Если коллекция включает объект **DynamicMembership**, то в этой группе используется динамическое членство. В противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="d98bc-153">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="d98bc-154">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="d98bc-154">mailEnabled</span></span>|<span data-ttu-id="d98bc-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="d98bc-155">Boolean</span></span>|<span data-ttu-id="d98bc-156">Указывает, включена ли для этой группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="d98bc-156">Specifies whether the group is mail-enabled.</span></span>|
|<span data-ttu-id="d98bc-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d98bc-157">mailNickname</span></span>|<span data-ttu-id="d98bc-158">String</span><span class="sxs-lookup"><span data-stu-id="d98bc-158">String</span></span>|<span data-ttu-id="d98bc-p107">Почтовый псевдоним для группы. Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="d98bc-p107">The mail alias for the group. This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="d98bc-161">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="d98bc-161">securityEnabled</span></span>|<span data-ttu-id="d98bc-162">Логический</span><span class="sxs-lookup"><span data-stu-id="d98bc-162">Boolean</span></span>|<span data-ttu-id="d98bc-163">Указывает, является ли эта группа группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="d98bc-163">Specifies whether the group is a security group.</span></span> |
|<span data-ttu-id="d98bc-164">visibility</span><span class="sxs-lookup"><span data-stu-id="d98bc-164">visibility</span></span>|<span data-ttu-id="d98bc-165">String</span><span class="sxs-lookup"><span data-stu-id="d98bc-165">String</span></span>|<span data-ttu-id="d98bc-166">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d98bc-166">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="d98bc-167">Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="d98bc-167">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="d98bc-168">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="d98bc-168">**Note:**</span></span>
>
> - <span data-ttu-id="d98bc-169">Свойства **allowExternalSenders** и **autoSubscribeNewMembers** можно изменить, указав их в отдельном запросе PATCH, не затрагивающем другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="d98bc-169">You can update **allowExternalSenders** and **autoSubscribeNewMembers** by specifying them in their own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="d98bc-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](/graph/known-issues#groups).</span><span class="sxs-lookup"><span data-stu-id="d98bc-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#groups) for examples.</span></span>
> - <span data-ttu-id="d98bc-173">Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="d98bc-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>

## <a name="response"></a><span data-ttu-id="d98bc-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="d98bc-174">Response</span></span>

<span data-ttu-id="d98bc-175">В случае успеха этот метод возвращает код отклика `204 No Content`, за исключением кода отклика `200 OK` при обновлении следующих свойств: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span><span class="sxs-lookup"><span data-stu-id="d98bc-175">If successful, this method returns a `204 No Content` response code—except a `200 OK` response code when updating the following properties: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>

## <a name="example"></a><span data-ttu-id="d98bc-176">Пример</span><span class="sxs-lookup"><span data-stu-id="d98bc-176">Example</span></span>

<span data-ttu-id="d98bc-177">В примере ниже показано, как обновить группу.</span><span class="sxs-lookup"><span data-stu-id="d98bc-177">The following example shows how to update a group.</span></span>

### <a name="request"></a><span data-ttu-id="d98bc-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="d98bc-178">Request</span></span>

<span data-ttu-id="d98bc-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d98bc-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d98bc-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="d98bc-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d98bc-181">C#</span><span class="sxs-lookup"><span data-stu-id="d98bc-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d98bc-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d98bc-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d98bc-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d98bc-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d98bc-184">Java</span><span class="sxs-lookup"><span data-stu-id="d98bc-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d98bc-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="d98bc-185">Response</span></span>

<span data-ttu-id="d98bc-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d98bc-186">The following is an example of the response.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
