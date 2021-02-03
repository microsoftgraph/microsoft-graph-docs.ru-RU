---
title: Удаление открытого расширения
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 01be68fc952fbc57debeb054257813cb34d626a5
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092738"
---
# <a name="delete-open-extension"></a><span data-ttu-id="3a9fa-103">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="3a9fa-103">Delete open extension</span></span>

<span data-ttu-id="3a9fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a9fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a9fa-105">Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

<span data-ttu-id="3a9fa-106">Список ресурсов, [](#permissions) которые поддерживают открытые расширения, см. в таблице в разделе "Разрешения".</span><span class="sxs-lookup"><span data-stu-id="3a9fa-106">See the table in the [Permissions](#permissions) section for the list of resources that support open extensions.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a9fa-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a9fa-107">Permissions</span></span>

<span data-ttu-id="3a9fa-108">В зависимости от ресурса, из который удаляется расширение, и запрашиваемого типа разрешений (делегированная или приложение), разрешение, указанное в следующей таблице, является наименее привилегированным для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3a9fa-109">Чтобы узнать больше, в том [числе](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) с осторожностью перед выбором более привилегированных разрешений, найди следующие разрешения в [разрешениях.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="3a9fa-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a9fa-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="3a9fa-110">Supported resource</span></span> | <span data-ttu-id="3a9fa-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a9fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3a9fa-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a9fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a9fa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a9fa-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3a9fa-114">device</span><span class="sxs-lookup"><span data-stu-id="3a9fa-114">device</span></span>](../resources/device.md) | <span data-ttu-id="3a9fa-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="3a9fa-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a9fa-116">Not supported</span></span> | <span data-ttu-id="3a9fa-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="3a9fa-118">event</span><span class="sxs-lookup"><span data-stu-id="3a9fa-118">event</span></span>](../resources/event.md) | <span data-ttu-id="3a9fa-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="3a9fa-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="3a9fa-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="3a9fa-122">group</span><span class="sxs-lookup"><span data-stu-id="3a9fa-122">group</span></span>](../resources/group.md) | <span data-ttu-id="3a9fa-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="3a9fa-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a9fa-124">Not supported</span></span> | <span data-ttu-id="3a9fa-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-125">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3a9fa-126">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="3a9fa-126">[group event](../resources/event.md)</span></span> | <span data-ttu-id="3a9fa-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="3a9fa-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a9fa-128">Not supported</span></span> | <span data-ttu-id="3a9fa-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a9fa-129">Not supported</span></span> |
| <span data-ttu-id="3a9fa-130">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="3a9fa-130">[group post](../resources/post.md)</span></span> | <span data-ttu-id="3a9fa-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="3a9fa-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a9fa-132">Not supported</span></span> | <span data-ttu-id="3a9fa-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="3a9fa-134">message</span><span class="sxs-lookup"><span data-stu-id="3a9fa-134">message</span></span>](../resources/message.md) | <span data-ttu-id="3a9fa-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-135">Mail.ReadWrite</span></span> | <span data-ttu-id="3a9fa-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-136">Mail.ReadWrite</span></span> | <span data-ttu-id="3a9fa-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="3a9fa-138">organization</span><span class="sxs-lookup"><span data-stu-id="3a9fa-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="3a9fa-139">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-139">Organization.ReadWrite.All</span></span> | <span data-ttu-id="3a9fa-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a9fa-140">Not supported</span></span> | <span data-ttu-id="3a9fa-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-141">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="3a9fa-142">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="3a9fa-142">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="3a9fa-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="3a9fa-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="3a9fa-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="3a9fa-146">user</span><span class="sxs-lookup"><span data-stu-id="3a9fa-146">user</span></span>](../resources/user.md) | <span data-ttu-id="3a9fa-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-147">User.ReadWrite</span></span> | <span data-ttu-id="3a9fa-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-148">User.ReadWrite</span></span> | <span data-ttu-id="3a9fa-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-149">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="3a9fa-150">task</span><span class="sxs-lookup"><span data-stu-id="3a9fa-150">task</span></span>](../resources/todotask.md) | <span data-ttu-id="3a9fa-151">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-151">Tasks.ReadWrite</span></span> | <span data-ttu-id="3a9fa-152">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-152">Tasks.ReadWrite</span></span> | <span data-ttu-id="3a9fa-153">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-153">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="3a9fa-154">tasklist</span><span class="sxs-lookup"><span data-stu-id="3a9fa-154">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="3a9fa-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="3a9fa-156">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a9fa-156">Tasks.ReadWrite</span></span> | <span data-ttu-id="3a9fa-157">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9fa-157">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a9fa-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a9fa-158">HTTP request</span></span>

<span data-ttu-id="3a9fa-159">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-159">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="3a9fa-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="3a9fa-162">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3a9fa-162">Path parameters</span></span>
|<span data-ttu-id="3a9fa-163">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="3a9fa-163">**Parameter**</span></span>|<span data-ttu-id="3a9fa-164">**Тип**</span><span class="sxs-lookup"><span data-stu-id="3a9fa-164">**Type**</span></span>|<span data-ttu-id="3a9fa-165">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3a9fa-165">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3a9fa-166">id</span><span class="sxs-lookup"><span data-stu-id="3a9fa-166">id</span></span>|<span data-ttu-id="3a9fa-167">string</span><span class="sxs-lookup"><span data-stu-id="3a9fa-167">string</span></span>|<span data-ttu-id="3a9fa-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="3a9fa-170">extensionId</span><span class="sxs-lookup"><span data-stu-id="3a9fa-170">extensionId</span></span>|<span data-ttu-id="3a9fa-171">string</span><span class="sxs-lookup"><span data-stu-id="3a9fa-171">string</span></span>|<span data-ttu-id="3a9fa-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3a9fa-175">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a9fa-175">Request headers</span></span>
| <span data-ttu-id="3a9fa-176">Имя</span><span class="sxs-lookup"><span data-stu-id="3a9fa-176">Name</span></span>       | <span data-ttu-id="3a9fa-177">Значение</span><span class="sxs-lookup"><span data-stu-id="3a9fa-177">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3a9fa-178">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a9fa-178">Authorization</span></span> | <span data-ttu-id="3a9fa-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a9fa-181">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a9fa-181">Request body</span></span>
<span data-ttu-id="3a9fa-182">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-182">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a9fa-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9fa-183">Response</span></span>

<span data-ttu-id="3a9fa-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9fa-186">Пример</span><span class="sxs-lookup"><span data-stu-id="3a9fa-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a9fa-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a9fa-187">Request</span></span>
<span data-ttu-id="3a9fa-188">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-188">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a9fa-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a9fa-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[<span data-ttu-id="3a9fa-190">C#</span><span class="sxs-lookup"><span data-stu-id="3a9fa-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a9fa-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a9fa-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a9fa-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a9fa-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a9fa-193">Java</span><span class="sxs-lookup"><span data-stu-id="3a9fa-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3a9fa-194">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-194">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="3a9fa-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9fa-195">Response</span></span>
<span data-ttu-id="3a9fa-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a9fa-196">Here is an example of the response.</span></span>
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


