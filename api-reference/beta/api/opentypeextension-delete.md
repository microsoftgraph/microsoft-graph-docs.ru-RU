---
title: Удаление открытого расширения
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 06c94c94d28af9e23c9b323e19a38c703231fa87
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976291"
---
# <a name="delete-open-extension"></a><span data-ttu-id="a07dc-103">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="a07dc-103">Delete open extension</span></span>

<span data-ttu-id="a07dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a07dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a07dc-105">Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="a07dc-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a07dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a07dc-106">Permissions</span></span>

<span data-ttu-id="a07dc-107">В зависимости от ресурса, из которого вы удаляете расширение, и запрошенного типа разрешения (делегированного или приложения), разрешение, указанное в следующей таблице, является минимальным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a07dc-107">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a07dc-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a07dc-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a07dc-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="a07dc-109">Supported resource</span></span> | <span data-ttu-id="a07dc-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a07dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a07dc-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a07dc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a07dc-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a07dc-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="a07dc-113">device</span><span class="sxs-lookup"><span data-stu-id="a07dc-113">device</span></span>](../resources/device.md) | <span data-ttu-id="a07dc-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="a07dc-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a07dc-115">Not supported</span></span> | <span data-ttu-id="a07dc-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="a07dc-117">event</span><span class="sxs-lookup"><span data-stu-id="a07dc-117">event</span></span>](../resources/event.md) | <span data-ttu-id="a07dc-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="a07dc-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="a07dc-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="a07dc-121">group</span><span class="sxs-lookup"><span data-stu-id="a07dc-121">group</span></span>](../resources/group.md) | <span data-ttu-id="a07dc-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="a07dc-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a07dc-123">Not supported</span></span> | <span data-ttu-id="a07dc-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-124">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a07dc-125">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="a07dc-125">[group event](../resources/event.md)</span></span> | <span data-ttu-id="a07dc-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="a07dc-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a07dc-127">Not supported</span></span> | <span data-ttu-id="a07dc-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a07dc-128">Not supported</span></span> |
| <span data-ttu-id="a07dc-129">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="a07dc-129">[group post](../resources/post.md)</span></span> | <span data-ttu-id="a07dc-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="a07dc-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a07dc-131">Not supported</span></span> | <span data-ttu-id="a07dc-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="a07dc-133">message</span><span class="sxs-lookup"><span data-stu-id="a07dc-133">message</span></span>](../resources/message.md) | <span data-ttu-id="a07dc-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-134">Mail.ReadWrite</span></span> | <span data-ttu-id="a07dc-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-135">Mail.ReadWrite</span></span> | <span data-ttu-id="a07dc-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="a07dc-137">organization</span><span class="sxs-lookup"><span data-stu-id="a07dc-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="a07dc-138">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-138">Organization.ReadWrite.All</span></span> | <span data-ttu-id="a07dc-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a07dc-139">Not supported</span></span> | <span data-ttu-id="a07dc-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-140">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="a07dc-141">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="a07dc-141">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="a07dc-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="a07dc-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="a07dc-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="a07dc-145">user</span><span class="sxs-lookup"><span data-stu-id="a07dc-145">user</span></span>](../resources/user.md) | <span data-ttu-id="a07dc-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-146">User.ReadWrite</span></span> | <span data-ttu-id="a07dc-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-147">User.ReadWrite</span></span> | <span data-ttu-id="a07dc-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-148">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="a07dc-149">task</span><span class="sxs-lookup"><span data-stu-id="a07dc-149">task</span></span>](../resources/todotask.md) | <span data-ttu-id="a07dc-150">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-150">Tasks.ReadWrite</span></span> | <span data-ttu-id="a07dc-151">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-151">Tasks.ReadWrite</span></span> | <span data-ttu-id="a07dc-152">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-152">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="a07dc-153">tasklist</span><span class="sxs-lookup"><span data-stu-id="a07dc-153">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="a07dc-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-154">Tasks.ReadWrite</span></span> | <span data-ttu-id="a07dc-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a07dc-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="a07dc-156">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a07dc-156">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a07dc-157">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a07dc-157">HTTP request</span></span>

<span data-ttu-id="a07dc-158">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="a07dc-158">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{Id}/extensions/{extensionId}
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
DELETE /users/me/todo/lists/{todoTaskListId}/extensions/{extensionId}
DELETE /users/me/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
```

><span data-ttu-id="a07dc-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="a07dc-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="a07dc-161">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="a07dc-161">Path parameters</span></span>
|<span data-ttu-id="a07dc-162">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="a07dc-162">**Parameter**</span></span>|<span data-ttu-id="a07dc-163">**Тип**</span><span class="sxs-lookup"><span data-stu-id="a07dc-163">**Type**</span></span>|<span data-ttu-id="a07dc-164">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a07dc-164">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a07dc-165">id</span><span class="sxs-lookup"><span data-stu-id="a07dc-165">id</span></span>|<span data-ttu-id="a07dc-166">string</span><span class="sxs-lookup"><span data-stu-id="a07dc-166">string</span></span>|<span data-ttu-id="a07dc-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a07dc-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="a07dc-169">extensionId</span><span class="sxs-lookup"><span data-stu-id="a07dc-169">extensionId</span></span>|<span data-ttu-id="a07dc-170">string</span><span class="sxs-lookup"><span data-stu-id="a07dc-170">string</span></span>|<span data-ttu-id="a07dc-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a07dc-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a07dc-174">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a07dc-174">Request headers</span></span>
| <span data-ttu-id="a07dc-175">Имя</span><span class="sxs-lookup"><span data-stu-id="a07dc-175">Name</span></span>       | <span data-ttu-id="a07dc-176">Значение</span><span class="sxs-lookup"><span data-stu-id="a07dc-176">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a07dc-177">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a07dc-177">Authorization</span></span> | <span data-ttu-id="a07dc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a07dc-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a07dc-180">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a07dc-180">Request body</span></span>
<span data-ttu-id="a07dc-181">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a07dc-181">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a07dc-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="a07dc-182">Response</span></span>

<span data-ttu-id="a07dc-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a07dc-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a07dc-185">Пример</span><span class="sxs-lookup"><span data-stu-id="a07dc-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a07dc-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="a07dc-186">Request</span></span>
<span data-ttu-id="a07dc-187">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="a07dc-187">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="a07dc-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="a07dc-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[<span data-ttu-id="a07dc-189">C#</span><span class="sxs-lookup"><span data-stu-id="a07dc-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a07dc-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a07dc-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a07dc-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a07dc-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a07dc-192">Java</span><span class="sxs-lookup"><span data-stu-id="a07dc-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a07dc-193">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="a07dc-193">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="a07dc-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="a07dc-194">Response</span></span>
<span data-ttu-id="a07dc-195">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a07dc-195">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


