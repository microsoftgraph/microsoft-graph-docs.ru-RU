---
title: Обновление группы
description: Обновление свойств объекта group.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0cb114173db81ca8f4f2042b74ff7126b66b5953
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401595"
---
# <a name="update-group"></a><span data-ttu-id="4499d-103">Update group</span><span class="sxs-lookup"><span data-stu-id="4499d-103">Update group</span></span>

<span data-ttu-id="4499d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4499d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4499d-105">Обновление свойств объекта group.</span><span class="sxs-lookup"><span data-stu-id="4499d-105">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4499d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4499d-106">Permissions</span></span>

<span data-ttu-id="4499d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4499d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4499d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4499d-109">Permission type</span></span>      | <span data-ttu-id="4499d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4499d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4499d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4499d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4499d-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4499d-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="4499d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4499d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4499d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4499d-114">Not supported.</span></span>    |
|<span data-ttu-id="4499d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4499d-115">Application</span></span> | <span data-ttu-id="4499d-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4499d-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4499d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4499d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4499d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4499d-118">Request headers</span></span>

| <span data-ttu-id="4499d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4499d-119">Name</span></span>       | <span data-ttu-id="4499d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4499d-120">Type</span></span> | <span data-ttu-id="4499d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4499d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4499d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4499d-122">Authorization</span></span>  | <span data-ttu-id="4499d-123">string</span><span class="sxs-lookup"><span data-stu-id="4499d-123">string</span></span>  | <span data-ttu-id="4499d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4499d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4499d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4499d-126">Request body</span></span>

<span data-ttu-id="4499d-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4499d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4499d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4499d-130">Property</span></span>   | <span data-ttu-id="4499d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4499d-131">Type</span></span> |<span data-ttu-id="4499d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4499d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4499d-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="4499d-133">allowExternalSenders</span></span>|<span data-ttu-id="4499d-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="4499d-134">Boolean</span></span>|<span data-ttu-id="4499d-p104">Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="4499d-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="4499d-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="4499d-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="4499d-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="4499d-138">Boolean</span></span>|<span data-ttu-id="4499d-p105">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="4499d-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="4499d-141">description</span><span class="sxs-lookup"><span data-stu-id="4499d-141">description</span></span>|<span data-ttu-id="4499d-142">String</span><span class="sxs-lookup"><span data-stu-id="4499d-142">String</span></span>|<span data-ttu-id="4499d-143">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="4499d-143">An optional description for the group.</span></span> |
|<span data-ttu-id="4499d-144">displayName</span><span class="sxs-lookup"><span data-stu-id="4499d-144">displayName</span></span>|<span data-ttu-id="4499d-145">String</span><span class="sxs-lookup"><span data-stu-id="4499d-145">String</span></span>|<span data-ttu-id="4499d-p106">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления.</span><span class="sxs-lookup"><span data-stu-id="4499d-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="4499d-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="4499d-148">groupTypes</span></span>|<span data-ttu-id="4499d-149">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4499d-149">String collection</span></span>|<span data-ttu-id="4499d-150">Задает тип группы и участие в ней.</span><span class="sxs-lookup"><span data-stu-id="4499d-150">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="4499d-151">Если коллекция содержит объект **Unified**, эта группа является группой Microsoft 365. В противном случае она является группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="4499d-151">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="4499d-152">Если коллекция включает объект **DynamicMembership**, то в этой группе используется динамическое членство. В противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="4499d-152">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="4499d-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4499d-153">mailEnabled</span></span>|<span data-ttu-id="4499d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4499d-154">Boolean</span></span>|<span data-ttu-id="4499d-155">Указывает, включена ли для этой группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="4499d-155">Specifies whether the group is mail-enabled.</span></span>|
|<span data-ttu-id="4499d-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4499d-156">mailNickname</span></span>|<span data-ttu-id="4499d-157">String</span><span class="sxs-lookup"><span data-stu-id="4499d-157">String</span></span>|<span data-ttu-id="4499d-158">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="4499d-158">The mail alias for the group.</span></span> <span data-ttu-id="4499d-159">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="4499d-159">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="4499d-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4499d-160">securityEnabled</span></span>|<span data-ttu-id="4499d-161">Логический</span><span class="sxs-lookup"><span data-stu-id="4499d-161">Boolean</span></span>|<span data-ttu-id="4499d-162">Указывает, является ли эта группа группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="4499d-162">Specifies whether the group is a security group.</span></span> |
|<span data-ttu-id="4499d-163">visibility</span><span class="sxs-lookup"><span data-stu-id="4499d-163">visibility</span></span>|<span data-ttu-id="4499d-164">String</span><span class="sxs-lookup"><span data-stu-id="4499d-164">String</span></span>|<span data-ttu-id="4499d-165">Определяет видимость группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4499d-165">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="4499d-166">Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="4499d-166">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="4499d-167">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="4499d-167">**Note:**</span></span>
>
> - <span data-ttu-id="4499d-168">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="4499d-168">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request,without including the other properties in the table above.</span></span>
> - <span data-ttu-id="4499d-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](/graph/known-issues#groups).</span><span class="sxs-lookup"><span data-stu-id="4499d-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#groups) for examples.</span></span>
> - <span data-ttu-id="4499d-172">Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="4499d-172">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>


## <a name="response"></a><span data-ttu-id="4499d-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="4499d-173">Response</span></span>

<span data-ttu-id="4499d-174">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4499d-174">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4499d-175">Пример</span><span class="sxs-lookup"><span data-stu-id="4499d-175">Example</span></span>

<span data-ttu-id="4499d-176">В примере ниже показано, как обновить группу.</span><span class="sxs-lookup"><span data-stu-id="4499d-176">The following example shows how to update a group.</span></span>

### <a name="request"></a><span data-ttu-id="4499d-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="4499d-177">Request</span></span>

<span data-ttu-id="4499d-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4499d-178">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4499d-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="4499d-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4499d-180">C#</span><span class="sxs-lookup"><span data-stu-id="4499d-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4499d-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4499d-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4499d-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4499d-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4499d-183">Java</span><span class="sxs-lookup"><span data-stu-id="4499d-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4499d-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="4499d-184">Response</span></span>

<span data-ttu-id="4499d-185">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4499d-185">The following is an example of the response.</span></span>

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
