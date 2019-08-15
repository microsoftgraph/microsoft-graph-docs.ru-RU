---
title: Обновление группы
description: Обновление свойств объекта [Group](../resources/group.md) .
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 39ab782ff74564f59d43f504afae459a9108b440
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420030"
---
# <a name="update-group"></a><span data-ttu-id="9ed1f-103">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="9ed1f-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed1f-104">Обновление свойств объекта [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="9ed1f-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed1f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed1f-105">Permissions</span></span>

<span data-ttu-id="9ed1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ed1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed1f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed1f-108">Permission type</span></span>      | <span data-ttu-id="9ed1f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ed1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ed1f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ed1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ed1f-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ed1f-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="9ed1f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ed1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed1f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-113">Not supported.</span></span>    |
|<span data-ttu-id="9ed1f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ed1f-114">Application</span></span> | <span data-ttu-id="9ed1f-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed1f-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ed1f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ed1f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9ed1f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ed1f-117">Request headers</span></span>

| <span data-ttu-id="9ed1f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9ed1f-118">Name</span></span>       | <span data-ttu-id="9ed1f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9ed1f-119">Type</span></span> | <span data-ttu-id="9ed1f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ed1f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9ed1f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed1f-121">Authorization</span></span>  | <span data-ttu-id="9ed1f-122">string</span><span class="sxs-lookup"><span data-stu-id="9ed1f-122">string</span></span>  | <span data-ttu-id="9ed1f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ed1f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ed1f-125">Request body</span></span>

<span data-ttu-id="9ed1f-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9ed1f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ed1f-129">Property</span></span>   | <span data-ttu-id="9ed1f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9ed1f-130">Type</span></span> |<span data-ttu-id="9ed1f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9ed1f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ed1f-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="9ed1f-132">allowExternalSenders</span></span>|<span data-ttu-id="9ed1f-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="9ed1f-133">Boolean</span></span>|<span data-ttu-id="9ed1f-p104">Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="9ed1f-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="9ed1f-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="9ed1f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed1f-137">Boolean</span></span>|<span data-ttu-id="9ed1f-p105">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="9ed1f-140">description</span><span class="sxs-lookup"><span data-stu-id="9ed1f-140">description</span></span>|<span data-ttu-id="9ed1f-141">String</span><span class="sxs-lookup"><span data-stu-id="9ed1f-141">String</span></span>|<span data-ttu-id="9ed1f-142">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-142">An optional description for the group.</span></span> |
|<span data-ttu-id="9ed1f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="9ed1f-143">displayName</span></span>|<span data-ttu-id="9ed1f-144">String</span><span class="sxs-lookup"><span data-stu-id="9ed1f-144">String</span></span>|<span data-ttu-id="9ed1f-145">Отображаемое имя для группы.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-145">The display name for the group.</span></span> <span data-ttu-id="9ed1f-146">Это свойство является обязательным при создании группы и не может быть очищено во время обновлений.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-146">This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="9ed1f-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="9ed1f-147">groupTypes</span></span>|<span data-ttu-id="9ed1f-148">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9ed1f-148">String collection</span></span>|<span data-ttu-id="9ed1f-149">Указывает тип группы и ее принадлежность.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="9ed1f-150">Если коллекция содержит **Unified** , то эта группа является группой Office 365; в противном случае это группа безопасности.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="9ed1f-151">Если коллекция включает **включить динамическое членство**, Группа имеет динамическое членство; в противном случае членство является статическим.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="9ed1f-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="9ed1f-152">mailEnabled</span></span>|<span data-ttu-id="9ed1f-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed1f-153">Boolean</span></span>|<span data-ttu-id="9ed1f-154">Указывает, включена ли для группы поддержка почты.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-154">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="9ed1f-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9ed1f-155">mailNickname</span></span>|<span data-ttu-id="9ed1f-156">String</span><span class="sxs-lookup"><span data-stu-id="9ed1f-156">String</span></span>|<span data-ttu-id="9ed1f-157">Почтовый псевдоним для группы.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-157">The mail alias for the group.</span></span> <span data-ttu-id="9ed1f-158">Это свойство должно быть указано при создании группы.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="9ed1f-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="9ed1f-159">securityEnabled</span></span>|<span data-ttu-id="9ed1f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ed1f-160">Boolean</span></span>|<span data-ttu-id="9ed1f-161">Указывает, является ли группа группой безопасности, в том числе группами Office 365.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-161">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="9ed1f-162">visibility</span><span class="sxs-lookup"><span data-stu-id="9ed1f-162">visibility</span></span>|<span data-ttu-id="9ed1f-163">String</span><span class="sxs-lookup"><span data-stu-id="9ed1f-163">String</span></span>|<span data-ttu-id="9ed1f-p108">Определяет видимость группы Office 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="9ed1f-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="9ed1f-166">Так как ресурс **Group** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в настраиваемых свойствах расширения в существующем экземпляре **группы** .</span><span class="sxs-lookup"><span data-stu-id="9ed1f-166">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="9ed1f-167">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="9ed1f-167">**Note:**</span></span>
>
> - <span data-ttu-id="9ed1f-168">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-168">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="9ed1f-p109">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="9ed1f-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="9ed1f-172">Правила обновления групп безопасности с включенной поддержкой почты в Microsoft Exchange Server могут быть сложными; Дополнительные сведения см. [в статье Управление группами безопасности с поддержкой почты в Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="9ed1f-172">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>
 


## <a name="response"></a><span data-ttu-id="9ed1f-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ed1f-173">Response</span></span>

<span data-ttu-id="9ed1f-174">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-174">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9ed1f-175">Пример</span><span class="sxs-lookup"><span data-stu-id="9ed1f-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9ed1f-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ed1f-176">Request</span></span>

<span data-ttu-id="9ed1f-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-177">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ed1f-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed1f-178">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ed1f-179">C#</span><span class="sxs-lookup"><span data-stu-id="9ed1f-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ed1f-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed1f-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ed1f-181">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9ed1f-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ed1f-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ed1f-182">Response</span></span>

<span data-ttu-id="9ed1f-183">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9ed1f-183">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="9ed1f-184">См. также</span><span class="sxs-lookup"><span data-stu-id="9ed1f-184">See also</span></span>

- [<span data-ttu-id="9ed1f-185">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9ed1f-185">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9ed1f-186">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9ed1f-186">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9ed1f-187">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9ed1f-187">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
