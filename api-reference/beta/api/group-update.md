---
title: Обновление группы
description: Обновление свойств, принадлежащих объекту группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f1f86067771a4732c8839f48bc02dd3edd15c19b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915237"
---
# <a name="update-group"></a><span data-ttu-id="228ee-103">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="228ee-103">Update group</span></span>

> <span data-ttu-id="228ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="228ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="228ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="228ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="228ee-106">Обновляет свойства объекта [группы](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="228ee-106">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="228ee-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="228ee-107">Permissions</span></span>

<span data-ttu-id="228ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="228ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="228ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="228ee-110">Permission type</span></span>      | <span data-ttu-id="228ee-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="228ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="228ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="228ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="228ee-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228ee-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="228ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="228ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="228ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="228ee-115">Not supported.</span></span>    |
|<span data-ttu-id="228ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="228ee-116">Application</span></span> | <span data-ttu-id="228ee-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228ee-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="228ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="228ee-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="228ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="228ee-119">Request headers</span></span>

| <span data-ttu-id="228ee-120">Имя</span><span class="sxs-lookup"><span data-stu-id="228ee-120">Name</span></span>       | <span data-ttu-id="228ee-121">Тип</span><span class="sxs-lookup"><span data-stu-id="228ee-121">Type</span></span> | <span data-ttu-id="228ee-122">Описание</span><span class="sxs-lookup"><span data-stu-id="228ee-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="228ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="228ee-123">Authorization</span></span>  | <span data-ttu-id="228ee-124">строка</span><span class="sxs-lookup"><span data-stu-id="228ee-124">string</span></span>  | <span data-ttu-id="228ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="228ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="228ee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="228ee-127">Request body</span></span>

<span data-ttu-id="228ee-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="228ee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="228ee-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="228ee-131">Property</span></span>   | <span data-ttu-id="228ee-132">Тип</span><span class="sxs-lookup"><span data-stu-id="228ee-132">Type</span></span> |<span data-ttu-id="228ee-133">Описание</span><span class="sxs-lookup"><span data-stu-id="228ee-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="228ee-134">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="228ee-134">allowExternalSenders</span></span>|<span data-ttu-id="228ee-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="228ee-135">Boolean</span></span>|<span data-ttu-id="228ee-p105">Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.</span><span class="sxs-lookup"><span data-stu-id="228ee-p105">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="228ee-138">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="228ee-138">autoSubscribeNewMembers</span></span>|<span data-ttu-id="228ee-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="228ee-139">Boolean</span></span>|<span data-ttu-id="228ee-p106">Значение, используемое по умолчанию: **false**. Указывает, будут ли новые участники группы автоматически подписаны на получение уведомлений по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="228ee-p106">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="228ee-142">описание</span><span class="sxs-lookup"><span data-stu-id="228ee-142">description</span></span>|<span data-ttu-id="228ee-143">String</span><span class="sxs-lookup"><span data-stu-id="228ee-143">String</span></span>|<span data-ttu-id="228ee-144">Необязательное описание для группы.</span><span class="sxs-lookup"><span data-stu-id="228ee-144">An optional description for the group.</span></span> |
|<span data-ttu-id="228ee-145">displayName</span><span class="sxs-lookup"><span data-stu-id="228ee-145">displayName</span></span>|<span data-ttu-id="228ee-146">String</span><span class="sxs-lookup"><span data-stu-id="228ee-146">String</span></span>|<span data-ttu-id="228ee-p107">Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.</span><span class="sxs-lookup"><span data-stu-id="228ee-p107">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="228ee-150">groupTypes</span><span class="sxs-lookup"><span data-stu-id="228ee-150">groupTypes</span></span>|<span data-ttu-id="228ee-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="228ee-151">String collection</span></span>|<span data-ttu-id="228ee-p108">Указывает тип создаваемой группы. Возможные значения: **Unified** для создания группы Office 365 или **DynamicMembership** для создания динамических групп.  Для остальных типов групп, таких как группы безопасности и поддерживающие почту группы безопасности, это свойство не задается.</span><span class="sxs-lookup"><span data-stu-id="228ee-p108">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="228ee-155">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="228ee-155">mailEnabled</span></span>|<span data-ttu-id="228ee-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="228ee-156">Boolean</span></span>|<span data-ttu-id="228ee-p109">Указывает, включена ли для этой группы поддержка почты. Если для свойства **securityEnabled** также задано значение **true**, это группа безопасности с включенной поддержкой почты. В противном случае это группа рассылки Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="228ee-p109">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="228ee-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="228ee-159">mailNickname</span></span>|<span data-ttu-id="228ee-160">String</span><span class="sxs-lookup"><span data-stu-id="228ee-160">String</span></span>|<span data-ttu-id="228ee-p110">Почтовый псевдоним для группы. Это свойство должно быть указано при создании группы. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="228ee-p110">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="228ee-164">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="228ee-164">securityEnabled</span></span>|<span data-ttu-id="228ee-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="228ee-165">Boolean</span></span>|<span data-ttu-id="228ee-p111">Указывает, является ли эта группа группой безопасности. Если для свойства **mailEnabled** также задано значение true, эта группа является группой безопасности, поддерживающей почту; в противном случае — это группа безопасности. Для групп Office 365 должно быть задано значение **false**. Поддерживает параметр $filter.</span><span class="sxs-lookup"><span data-stu-id="228ee-p111">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="228ee-170">visibility</span><span class="sxs-lookup"><span data-stu-id="228ee-170">visibility</span></span>|<span data-ttu-id="228ee-171">String</span><span class="sxs-lookup"><span data-stu-id="228ee-171">String</span></span>|<span data-ttu-id="228ee-p112">Определяет видимость группы Office 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).</span><span class="sxs-lookup"><span data-stu-id="228ee-p112">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="228ee-174">Поскольку **группы** ресурсов поддерживает [расширения](/graph/extensibility-overview), можно использовать `PATCH` операции для добавления, обновления или удаления данных конкретного приложения в настраиваемых свойств расширения в существующий экземпляр **группы** .</span><span class="sxs-lookup"><span data-stu-id="228ee-174">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="228ee-175">**Примечания:**</span><span class="sxs-lookup"><span data-stu-id="228ee-175">**Note:**</span></span>
>
> - <span data-ttu-id="228ee-176">Свойство **autoSubscribeNewMembers** можно обновить, указав его в его собственном запросе PATCH, не включая при этом другие свойства, описанные в таблице выше.</span><span class="sxs-lookup"><span data-stu-id="228ee-176">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="228ee-p113">Только некоторые элементы API групп, относящиеся к основным операциям администрирования групп и управления ими, поддерживают разрешения для приложений и делегированные разрешения. Все остальные элементы API групп, включая обновление **autoSubscribeNewMembers**, поддерживают только делегированные разрешения. Примеры см. в разделе [Известные проблемы](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="228ee-p113">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="228ee-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="228ee-180">Response</span></span>

<span data-ttu-id="228ee-181">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="228ee-181">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="228ee-182">Пример</span><span class="sxs-lookup"><span data-stu-id="228ee-182">Example</span></span>

#### <a name="request"></a><span data-ttu-id="228ee-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="228ee-183">Request</span></span>

<span data-ttu-id="228ee-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="228ee-184">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="228ee-185">Ответ</span><span class="sxs-lookup"><span data-stu-id="228ee-185">Response</span></span>

<span data-ttu-id="228ee-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="228ee-186">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="228ee-187">См. также</span><span class="sxs-lookup"><span data-stu-id="228ee-187">See also</span></span>

- [<span data-ttu-id="228ee-188">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="228ee-188">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="228ee-189">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="228ee-189">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="228ee-190">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="228ee-190">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
