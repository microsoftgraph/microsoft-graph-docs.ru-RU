---
title: Обновление группы
description: Обновление свойств объекта [Group](../resources/group.md) .
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d559fa5f4dead2601d14b6b708b5ce095b7b5055
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34036341"
---
# <a name="update-group"></a><span data-ttu-id="cd528-103">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="cd528-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd528-104">Обновление свойств объекта [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="cd528-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd528-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd528-105">Permissions</span></span>

<span data-ttu-id="cd528-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd528-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd528-108">Permission type</span></span>      | <span data-ttu-id="cd528-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd528-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd528-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd528-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd528-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd528-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd528-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd528-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd528-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd528-113">Not supported.</span></span>    |
|<span data-ttu-id="cd528-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd528-114">Application</span></span> | <span data-ttu-id="cd528-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd528-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd528-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd528-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cd528-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd528-117">Request headers</span></span>

| <span data-ttu-id="cd528-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cd528-118">Name</span></span>       | <span data-ttu-id="cd528-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cd528-119">Type</span></span> | <span data-ttu-id="cd528-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cd528-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cd528-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd528-121">Authorization</span></span>  | <span data-ttu-id="cd528-122">string</span><span class="sxs-lookup"><span data-stu-id="cd528-122">string</span></span>  | <span data-ttu-id="cd528-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd528-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd528-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd528-125">Request body</span></span>

<span data-ttu-id="cd528-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cd528-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cd528-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd528-129">Property</span></span>   | <span data-ttu-id="cd528-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd528-130">Type</span></span> |<span data-ttu-id="cd528-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd528-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd528-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="cd528-132">allowExternalSenders</span></span>|<span data-ttu-id="cd528-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="cd528-133">Boolean</span></span>|<span data-ttu-id="cd528-p104">Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="cd528-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="cd528-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="cd528-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="cd528-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd528-137">Boolean</span></span>|<span data-ttu-id="cd528-p105">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="cd528-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="cd528-140">description</span><span class="sxs-lookup"><span data-stu-id="cd528-140">description</span></span>|<span data-ttu-id="cd528-141">String</span><span class="sxs-lookup"><span data-stu-id="cd528-141">String</span></span>|<span data-ttu-id="cd528-142">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="cd528-142">An optional description for the group.</span></span> |
|<span data-ttu-id="cd528-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cd528-143">displayName</span></span>|<span data-ttu-id="cd528-144">String</span><span class="sxs-lookup"><span data-stu-id="cd528-144">String</span></span>|<span data-ttu-id="cd528-145">Отображаемое имя для группы.</span><span class="sxs-lookup"><span data-stu-id="cd528-145">The display name for the group.</span></span> <span data-ttu-id="cd528-146">Это свойство является обязательным при создании группы и не может быть очищено во время обновлений.</span><span class="sxs-lookup"><span data-stu-id="cd528-146">This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="cd528-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="cd528-147">groupTypes</span></span>|<span data-ttu-id="cd528-148">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd528-148">String collection</span></span>|<span data-ttu-id="cd528-149">Указывает тип группы и ее принадлежность.</span><span class="sxs-lookup"><span data-stu-id="cd528-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="cd528-150">Если коллекция содержит **Unified** , то эта группа является группой Office 365; в противном случае это группа безопасности.</span><span class="sxs-lookup"><span data-stu-id="cd528-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="cd528-151">Если коллекция включает **включить динамическое членство**, Группа имеет динамическое членство; в противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="cd528-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="cd528-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="cd528-152">mailEnabled</span></span>|<span data-ttu-id="cd528-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd528-153">Boolean</span></span>|<span data-ttu-id="cd528-154">Указывает, включена ли для группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="cd528-154">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="cd528-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cd528-155">mailNickname</span></span>|<span data-ttu-id="cd528-156">String</span><span class="sxs-lookup"><span data-stu-id="cd528-156">String</span></span>|<span data-ttu-id="cd528-157">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="cd528-157">The mail alias for the group.</span></span> <span data-ttu-id="cd528-158">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="cd528-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="cd528-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="cd528-159">securityEnabled</span></span>|<span data-ttu-id="cd528-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd528-160">Boolean</span></span>|<span data-ttu-id="cd528-161">Указывает, является ли группа группой безопасности, в том числе группами Office 365.</span><span class="sxs-lookup"><span data-stu-id="cd528-161">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="cd528-162">visibility</span><span class="sxs-lookup"><span data-stu-id="cd528-162">visibility</span></span>|<span data-ttu-id="cd528-163">String</span><span class="sxs-lookup"><span data-stu-id="cd528-163">String</span></span>|<span data-ttu-id="cd528-p108">Определяет видимость группы Office 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="cd528-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="cd528-166">Так как ресурс **Group** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в настраиваемых свойствах расширения в существующем экземпляре **группы** .</span><span class="sxs-lookup"><span data-stu-id="cd528-166">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="cd528-167">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="cd528-167">**Note:**</span></span>
>
> - <span data-ttu-id="cd528-168">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="cd528-168">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="cd528-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="cd528-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="cd528-172">Правила обновления групп безопасности с включенной поддержкой почты в Microsoft Exchange Server могут быть сложными; Дополнительные сведения см. [в статье Управление группами безопасности с поддержкой почты в Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="cd528-172">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>
 


## <a name="response"></a><span data-ttu-id="cd528-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd528-173">Response</span></span>

<span data-ttu-id="cd528-174">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cd528-174">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd528-175">Пример</span><span class="sxs-lookup"><span data-stu-id="cd528-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cd528-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd528-176">Request</span></span>

<span data-ttu-id="cd528-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd528-177">The following is an example of the request.</span></span>
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
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```

#### <a name="response"></a><span data-ttu-id="cd528-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd528-178">Response</span></span>

<span data-ttu-id="cd528-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd528-179">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cd528-180">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="cd528-180">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cd528-181">C#</span><span class="sxs-lookup"><span data-stu-id="cd528-181">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd528-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd528-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="cd528-183">См. также</span><span class="sxs-lookup"><span data-stu-id="cd528-183">See also</span></span>

- [<span data-ttu-id="cd528-184">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="cd528-184">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cd528-185">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cd528-185">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cd528-186">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cd528-186">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/group-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
