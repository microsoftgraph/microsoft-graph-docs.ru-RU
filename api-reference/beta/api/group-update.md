---
title: Обновление группы
description: Обновление свойств, принадлежащих объекту группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c60ff8eaf95401c5c3e8eb44017d9a6d37ac0ea4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32501976"
---
# <a name="update-group"></a><span data-ttu-id="9da01-103">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="9da01-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9da01-104">Обновление свойств объекта [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="9da01-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9da01-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9da01-105">Permissions</span></span>

<span data-ttu-id="9da01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9da01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9da01-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9da01-108">Permission type</span></span>      | <span data-ttu-id="9da01-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9da01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9da01-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9da01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9da01-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9da01-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9da01-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9da01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9da01-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9da01-113">Not supported.</span></span>    |
|<span data-ttu-id="9da01-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9da01-114">Application</span></span> | <span data-ttu-id="9da01-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9da01-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9da01-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9da01-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9da01-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9da01-117">Request headers</span></span>

| <span data-ttu-id="9da01-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9da01-118">Name</span></span>       | <span data-ttu-id="9da01-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9da01-119">Type</span></span> | <span data-ttu-id="9da01-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9da01-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9da01-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9da01-121">Authorization</span></span>  | <span data-ttu-id="9da01-122">string</span><span class="sxs-lookup"><span data-stu-id="9da01-122">string</span></span>  | <span data-ttu-id="9da01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9da01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9da01-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9da01-125">Request body</span></span>

<span data-ttu-id="9da01-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9da01-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9da01-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9da01-129">Property</span></span>   | <span data-ttu-id="9da01-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9da01-130">Type</span></span> |<span data-ttu-id="9da01-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9da01-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9da01-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="9da01-132">allowExternalSenders</span></span>|<span data-ttu-id="9da01-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9da01-133">Boolean</span></span>|<span data-ttu-id="9da01-p104">Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="9da01-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="9da01-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="9da01-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="9da01-137">Логический</span><span class="sxs-lookup"><span data-stu-id="9da01-137">Boolean</span></span>|<span data-ttu-id="9da01-p105">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="9da01-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="9da01-140">description</span><span class="sxs-lookup"><span data-stu-id="9da01-140">description</span></span>|<span data-ttu-id="9da01-141">String</span><span class="sxs-lookup"><span data-stu-id="9da01-141">String</span></span>|<span data-ttu-id="9da01-142">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="9da01-142">An optional description for the group.</span></span> |
|<span data-ttu-id="9da01-143">displayName</span><span class="sxs-lookup"><span data-stu-id="9da01-143">displayName</span></span>|<span data-ttu-id="9da01-144">Строка</span><span class="sxs-lookup"><span data-stu-id="9da01-144">String</span></span>|<span data-ttu-id="9da01-p106">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="9da01-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="9da01-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="9da01-148">groupTypes</span></span>|<span data-ttu-id="9da01-149">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9da01-149">String collection</span></span>|<span data-ttu-id="9da01-p107">Указывает тип создаваемой группы. Возможные значения: **Unified** для создания группы Office 365 или **DynamicMembership** для создания динамических групп.  Для остальных типов групп, таких как группы безопасности и поддерживающие почту группы безопасности, это свойство не задается.</span><span class="sxs-lookup"><span data-stu-id="9da01-p107">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="9da01-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="9da01-153">mailEnabled</span></span>|<span data-ttu-id="9da01-154">Логический</span><span class="sxs-lookup"><span data-stu-id="9da01-154">Boolean</span></span>|<span data-ttu-id="9da01-p108">Указывает, включена ли для этой группы поддержка почты. Если для свойства **securityEnabled** также задано значение **true**, это группа безопасности с включенной поддержкой почты. В противном случае это группа рассылки Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="9da01-p108">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="9da01-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="9da01-157">mailNickname</span></span>|<span data-ttu-id="9da01-158">String</span><span class="sxs-lookup"><span data-stu-id="9da01-158">String</span></span>|<span data-ttu-id="9da01-p109">Почтовый псевдоним для группы. Это свойство должно быть указано при создании группы. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="9da01-p109">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="9da01-162">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="9da01-162">securityEnabled</span></span>|<span data-ttu-id="9da01-163">Логическое</span><span class="sxs-lookup"><span data-stu-id="9da01-163">Boolean</span></span>|<span data-ttu-id="9da01-p110">Указывает, является ли эта группа группой безопасности. Если для свойства **mailEnabled** также задано значение true, эта группа является группой безопасности, поддерживающей почту; в противном случае — это группа безопасности. Для групп Office 365 должно быть задано значение **false**. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="9da01-p110">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="9da01-168">visibility</span><span class="sxs-lookup"><span data-stu-id="9da01-168">visibility</span></span>|<span data-ttu-id="9da01-169">String</span><span class="sxs-lookup"><span data-stu-id="9da01-169">String</span></span>|<span data-ttu-id="9da01-p111">Определяет видимость группы Office 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="9da01-p111">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="9da01-172">Так как ресурс **Group** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в настраиваемых свойствах расширения в существующем экземпляре **группы** .</span><span class="sxs-lookup"><span data-stu-id="9da01-172">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="9da01-173">**Примечание:**</span><span class="sxs-lookup"><span data-stu-id="9da01-173">**Note:**</span></span>
>
> - <span data-ttu-id="9da01-174">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="9da01-174">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="9da01-p112">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="9da01-p112">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="9da01-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="9da01-178">Response</span></span>

<span data-ttu-id="9da01-179">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9da01-179">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9da01-180">Пример</span><span class="sxs-lookup"><span data-stu-id="9da01-180">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9da01-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="9da01-181">Request</span></span>

<span data-ttu-id="9da01-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9da01-182">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="9da01-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="9da01-183">Response</span></span>

<span data-ttu-id="9da01-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9da01-184">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="9da01-185">См. также</span><span class="sxs-lookup"><span data-stu-id="9da01-185">See also</span></span>

- [<span data-ttu-id="9da01-186">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="9da01-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9da01-187">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9da01-187">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="9da01-188">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9da01-188">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
    "Error: /api-reference/beta/api/group-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
