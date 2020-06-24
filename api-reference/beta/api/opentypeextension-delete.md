---
title: Удаление открытого расширения
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: bd19d5ca1da444171201c7dbe4cd5c016aad5352
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863385"
---
# <a name="delete-open-extension"></a><span data-ttu-id="04ae1-103">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="04ae1-103">Delete open extension</span></span>

<span data-ttu-id="04ae1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04ae1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04ae1-105">Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="04ae1-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="04ae1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04ae1-106">Permissions</span></span>

<span data-ttu-id="04ae1-107">В зависимости от ресурса, из которого вы удаляете расширение, и запрошенного типа разрешения (делегированного или приложения), разрешение, указанное в следующей таблице, является минимальным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="04ae1-107">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="04ae1-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ae1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04ae1-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="04ae1-109">Supported resource</span></span> | <span data-ttu-id="04ae1-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04ae1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04ae1-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04ae1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04ae1-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04ae1-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="04ae1-113">device</span><span class="sxs-lookup"><span data-stu-id="04ae1-113">device</span></span>](../resources/device.md) | <span data-ttu-id="04ae1-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="04ae1-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04ae1-115">Not supported</span></span> | <span data-ttu-id="04ae1-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="04ae1-117">event</span><span class="sxs-lookup"><span data-stu-id="04ae1-117">event</span></span>](../resources/event.md) | <span data-ttu-id="04ae1-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="04ae1-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="04ae1-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="04ae1-121">group</span><span class="sxs-lookup"><span data-stu-id="04ae1-121">group</span></span>](../resources/group.md) | <span data-ttu-id="04ae1-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="04ae1-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04ae1-123">Not supported</span></span> | <span data-ttu-id="04ae1-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-124">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="04ae1-125">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="04ae1-125">[group event](../resources/event.md)</span></span> | <span data-ttu-id="04ae1-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="04ae1-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04ae1-127">Not supported</span></span> | <span data-ttu-id="04ae1-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04ae1-128">Not supported</span></span> |
| <span data-ttu-id="04ae1-129">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="04ae1-129">[group post](../resources/post.md)</span></span> | <span data-ttu-id="04ae1-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="04ae1-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04ae1-131">Not supported</span></span> | <span data-ttu-id="04ae1-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="04ae1-133">message</span><span class="sxs-lookup"><span data-stu-id="04ae1-133">message</span></span>](../resources/message.md) | <span data-ttu-id="04ae1-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-134">Mail.ReadWrite</span></span> | <span data-ttu-id="04ae1-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-135">Mail.ReadWrite</span></span> | <span data-ttu-id="04ae1-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="04ae1-137">organization</span><span class="sxs-lookup"><span data-stu-id="04ae1-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="04ae1-138">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-138">Organization.ReadWrite.All</span></span> | <span data-ttu-id="04ae1-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="04ae1-139">Not supported</span></span> | <span data-ttu-id="04ae1-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-140">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="04ae1-141">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="04ae1-141">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="04ae1-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="04ae1-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="04ae1-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="04ae1-145">user</span><span class="sxs-lookup"><span data-stu-id="04ae1-145">user</span></span>](../resources/user.md) | <span data-ttu-id="04ae1-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-146">User.ReadWrite</span></span> | <span data-ttu-id="04ae1-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04ae1-147">User.ReadWrite</span></span> | <span data-ttu-id="04ae1-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ae1-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04ae1-149">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04ae1-149">HTTP request</span></span>

<span data-ttu-id="04ae1-150">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="04ae1-150">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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
```

><span data-ttu-id="04ae1-151">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it.</span><span class="sxs-lookup"><span data-stu-id="04ae1-151">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it.</span></span> <span data-ttu-id="04ae1-152">All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span><span class="sxs-lookup"><span data-stu-id="04ae1-152">All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="04ae1-153">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="04ae1-153">Path parameters</span></span>
|<span data-ttu-id="04ae1-154">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="04ae1-154">**Parameter**</span></span>|<span data-ttu-id="04ae1-155">**Тип**</span><span class="sxs-lookup"><span data-stu-id="04ae1-155">**Type**</span></span>|<span data-ttu-id="04ae1-156">**Описание**</span><span class="sxs-lookup"><span data-stu-id="04ae1-156">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="04ae1-157">id</span><span class="sxs-lookup"><span data-stu-id="04ae1-157">id</span></span>|<span data-ttu-id="04ae1-158">строка</span><span class="sxs-lookup"><span data-stu-id="04ae1-158">string</span></span>|<span data-ttu-id="04ae1-159">A unique identifier for an instance in the corresponding collection.</span><span class="sxs-lookup"><span data-stu-id="04ae1-159">A unique identifier for an instance in the corresponding collection.</span></span> <span data-ttu-id="04ae1-160">Required.</span><span class="sxs-lookup"><span data-stu-id="04ae1-160">Required.</span></span>|
|<span data-ttu-id="04ae1-161">extensionId</span><span class="sxs-lookup"><span data-stu-id="04ae1-161">extensionId</span></span>|<span data-ttu-id="04ae1-162">string</span><span class="sxs-lookup"><span data-stu-id="04ae1-162">string</span></span>|<span data-ttu-id="04ae1-163">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span><span class="sxs-lookup"><span data-stu-id="04ae1-163">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span></span> <span data-ttu-id="04ae1-164">The fully qualified name is returned in the `id` property when you create the extension.</span><span class="sxs-lookup"><span data-stu-id="04ae1-164">The fully qualified name is returned in the `id` property when you create the extension.</span></span> <span data-ttu-id="04ae1-165">Required.</span><span class="sxs-lookup"><span data-stu-id="04ae1-165">Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="04ae1-166">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04ae1-166">Request headers</span></span>
| <span data-ttu-id="04ae1-167">Имя</span><span class="sxs-lookup"><span data-stu-id="04ae1-167">Name</span></span>       | <span data-ttu-id="04ae1-168">Значение</span><span class="sxs-lookup"><span data-stu-id="04ae1-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="04ae1-169">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04ae1-169">Authorization</span></span> | <span data-ttu-id="04ae1-170">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="04ae1-170">Bearer {token}.</span></span> <span data-ttu-id="04ae1-171">Required.</span><span class="sxs-lookup"><span data-stu-id="04ae1-171">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04ae1-172">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04ae1-172">Request body</span></span>
<span data-ttu-id="04ae1-173">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04ae1-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04ae1-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ae1-174">Response</span></span>

<span data-ttu-id="04ae1-175">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="04ae1-175">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="04ae1-176">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="04ae1-176">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04ae1-177">Пример</span><span class="sxs-lookup"><span data-stu-id="04ae1-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04ae1-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="04ae1-178">Request</span></span>
<span data-ttu-id="04ae1-179">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="04ae1-179">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="04ae1-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="04ae1-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[<span data-ttu-id="04ae1-181">C#</span><span class="sxs-lookup"><span data-stu-id="04ae1-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04ae1-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04ae1-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04ae1-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04ae1-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="04ae1-184">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="04ae1-184">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="04ae1-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ae1-185">Response</span></span>
<span data-ttu-id="04ae1-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04ae1-186">Here is an example of the response.</span></span>
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
