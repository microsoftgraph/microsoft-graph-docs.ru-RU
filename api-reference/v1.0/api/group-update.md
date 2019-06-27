---
title: Обновление группы
description: Обновление свойств объекта group.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 9f6ddca037452003b0192cf7b3cdcd894d2d03f0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263561"
---
# <a name="update-group"></a><span data-ttu-id="b4ab2-103">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="b4ab2-103">Update group</span></span>

<span data-ttu-id="b4ab2-104">Обновление свойств, принадлежащих объекту группы.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-104">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ab2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ab2-105">Permissions</span></span>

<span data-ttu-id="b4ab2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4ab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4ab2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4ab2-108">Permission type</span></span>      | <span data-ttu-id="b4ab2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4ab2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4ab2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4ab2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ab2-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4ab2-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="b4ab2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4ab2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ab2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-113">Not supported.</span></span>    |
|<span data-ttu-id="b4ab2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4ab2-114">Application</span></span> | <span data-ttu-id="b4ab2-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ab2-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ab2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4ab2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4ab2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4ab2-117">Request headers</span></span>

| <span data-ttu-id="b4ab2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b4ab2-118">Name</span></span>       | <span data-ttu-id="b4ab2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b4ab2-119">Type</span></span> | <span data-ttu-id="b4ab2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b4ab2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b4ab2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ab2-121">Authorization</span></span>  | <span data-ttu-id="b4ab2-122">string</span><span class="sxs-lookup"><span data-stu-id="b4ab2-122">string</span></span>  | <span data-ttu-id="b4ab2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ab2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4ab2-125">Request body</span></span>

<span data-ttu-id="b4ab2-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4ab2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4ab2-129">Property</span></span>   | <span data-ttu-id="b4ab2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4ab2-130">Type</span></span> |<span data-ttu-id="b4ab2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4ab2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4ab2-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="b4ab2-132">allowExternalSenders</span></span>|<span data-ttu-id="b4ab2-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="b4ab2-133">Boolean</span></span>|<span data-ttu-id="b4ab2-p104">Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="b4ab2-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="b4ab2-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="b4ab2-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4ab2-137">Boolean</span></span>|<span data-ttu-id="b4ab2-p105">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="b4ab2-140">description</span><span class="sxs-lookup"><span data-stu-id="b4ab2-140">description</span></span>|<span data-ttu-id="b4ab2-141">String</span><span class="sxs-lookup"><span data-stu-id="b4ab2-141">String</span></span>|<span data-ttu-id="b4ab2-142">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-142">An optional description for the group.</span></span> |
|<span data-ttu-id="b4ab2-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b4ab2-143">displayName</span></span>|<span data-ttu-id="b4ab2-144">String</span><span class="sxs-lookup"><span data-stu-id="b4ab2-144">String</span></span>|<span data-ttu-id="b4ab2-p106">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span> |
|<span data-ttu-id="b4ab2-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="b4ab2-147">groupTypes</span></span>|<span data-ttu-id="b4ab2-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b4ab2-148">String collection</span></span>|<span data-ttu-id="b4ab2-149">Задает тип группы и членства в ней.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="b4ab2-150">Если коллекция содержит объект **Unified**, то эта группа является группой Office 365. В противном случае она является группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="b4ab2-151">Если коллекция включает объект **DynamicMembership**, то в этой группе используется динамическое членство. В противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="b4ab2-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="b4ab2-152">mailEnabled</span></span>|<span data-ttu-id="b4ab2-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4ab2-153">Boolean</span></span>|<span data-ttu-id="b4ab2-154">Указывает, включена ли для этой группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-154">Specifies whether the group is a security group.</span></span>|
|<span data-ttu-id="b4ab2-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b4ab2-155">mailNickname</span></span>|<span data-ttu-id="b4ab2-156">String</span><span class="sxs-lookup"><span data-stu-id="b4ab2-156">String</span></span>|<span data-ttu-id="b4ab2-157">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-157">The mail alias for the group.</span></span> <span data-ttu-id="b4ab2-158">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="b4ab2-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="b4ab2-159">securityEnabled</span></span>|<span data-ttu-id="b4ab2-160">Логический</span><span class="sxs-lookup"><span data-stu-id="b4ab2-160">Boolean</span></span>|<span data-ttu-id="b4ab2-161">Указывает, является ли эта группа группой безопасности.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-161">Specifies whether the group is a security group.</span></span> |
|<span data-ttu-id="b4ab2-162">visibility</span><span class="sxs-lookup"><span data-stu-id="b4ab2-162">visibility</span></span>|<span data-ttu-id="b4ab2-163">String</span><span class="sxs-lookup"><span data-stu-id="b4ab2-163">String</span></span>|<span data-ttu-id="b4ab2-164">Определяет видимость группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-164">Specifies the visibility of an Office 365 group.</span></span> <span data-ttu-id="b4ab2-165">Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="b4ab2-165">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="b4ab2-166">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="b4ab2-166">**Note:**</span></span>
>
> - <span data-ttu-id="b4ab2-167">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request,without including the other properties in the table above.</span></span>
> - <span data-ttu-id="b4ab2-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="b4ab2-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="b4ab2-171">Правила обновления групп безопасности, поддерживающих почту, в Microsoft Exchange Server могут быть сложными. Дополнительные сведения см. в статье [Управление группами безопасности с поддержкой электронной почты в Exchange Server](https://docs.microsoft.com/ru-RU/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="b4ab2-171">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>


## <a name="response"></a><span data-ttu-id="b4ab2-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ab2-172">Response</span></span>

<span data-ttu-id="b4ab2-173">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-173">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4ab2-174">Пример</span><span class="sxs-lookup"><span data-stu-id="b4ab2-174">Example</span></span>

<span data-ttu-id="b4ab2-175">В приведенном ниже примере показано, как создать группу.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-175">The following example shows how to create a management scope for a specific group.</span></span>

### <a name="request"></a><span data-ttu-id="b4ab2-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4ab2-176">Request</span></span>

<span data-ttu-id="b4ab2-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-177">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4ab2-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4ab2-178">Response</span></span>

<span data-ttu-id="b4ab2-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b4ab2-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b4ab2-180">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b4ab2-180">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b4ab2-181">C#</span><span class="sxs-lookup"><span data-stu-id="b4ab2-181">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4ab2-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4ab2-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b4ab2-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4ab2-183">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
