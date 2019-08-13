---
title: Удаление открытого расширения
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 507672f99022751c82a3b1ea4efd9b0bd2c4b4f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342542"
---
# <a name="delete-open-extension"></a><span data-ttu-id="c5474-103">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="c5474-103">Delete open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5474-104">Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5474-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c5474-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5474-105">Permissions</span></span>

<span data-ttu-id="c5474-106">В зависимости от ресурса, из которого вы удаляете расширение, и запрошенного типа разрешения (делегированного или приложения), разрешение, указанное в следующей таблице, является минимальным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c5474-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c5474-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5474-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5474-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="c5474-108">Supported resource</span></span> | <span data-ttu-id="c5474-109">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5474-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c5474-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5474-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5474-111">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5474-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="c5474-112">device</span><span class="sxs-lookup"><span data-stu-id="c5474-112">device</span></span>](../resources/device.md) | <span data-ttu-id="c5474-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5474-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="c5474-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5474-114">Not supported</span></span> | <span data-ttu-id="c5474-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="c5474-116">event</span><span class="sxs-lookup"><span data-stu-id="c5474-116">event</span></span>](../resources/event.md) | <span data-ttu-id="c5474-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="c5474-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="c5474-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="c5474-120">group</span><span class="sxs-lookup"><span data-stu-id="c5474-120">group</span></span>](../resources/group.md) | <span data-ttu-id="c5474-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="c5474-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5474-122">Not supported</span></span> | <span data-ttu-id="c5474-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-123">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c5474-124">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="c5474-124">[group event](../resources/event.md)</span></span> | <span data-ttu-id="c5474-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="c5474-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5474-126">Not supported</span></span> | <span data-ttu-id="c5474-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5474-127">Not supported</span></span> |
| <span data-ttu-id="c5474-128">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="c5474-128">[group post](../resources/post.md)</span></span> | <span data-ttu-id="c5474-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="c5474-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5474-130">Not supported</span></span> | <span data-ttu-id="c5474-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="c5474-132">message</span><span class="sxs-lookup"><span data-stu-id="c5474-132">message</span></span>](../resources/message.md) | <span data-ttu-id="c5474-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-133">Mail.ReadWrite</span></span> | <span data-ttu-id="c5474-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-134">Mail.ReadWrite</span></span> | <span data-ttu-id="c5474-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="c5474-136">organization</span><span class="sxs-lookup"><span data-stu-id="c5474-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="c5474-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5474-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="c5474-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5474-138">Not supported</span></span> | <span data-ttu-id="c5474-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c5474-139">Not supported</span></span> |
| <span data-ttu-id="c5474-140">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="c5474-140">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="c5474-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="c5474-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="c5474-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="c5474-144">user</span><span class="sxs-lookup"><span data-stu-id="c5474-144">user</span></span>](../resources/user.md) | <span data-ttu-id="c5474-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-145">User.ReadWrite.All</span></span> | <span data-ttu-id="c5474-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5474-146">User.ReadWrite</span></span> | <span data-ttu-id="c5474-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5474-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5474-148">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5474-148">HTTP request</span></span>

<span data-ttu-id="c5474-149">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="c5474-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="c5474-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="c5474-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="c5474-152">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c5474-152">Path parameters</span></span>
|<span data-ttu-id="c5474-153">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="c5474-153">**Parameter**</span></span>|<span data-ttu-id="c5474-154">**Тип**</span><span class="sxs-lookup"><span data-stu-id="c5474-154">**Type**</span></span>|<span data-ttu-id="c5474-155">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5474-155">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c5474-156">id</span><span class="sxs-lookup"><span data-stu-id="c5474-156">id</span></span>|<span data-ttu-id="c5474-157">string</span><span class="sxs-lookup"><span data-stu-id="c5474-157">string</span></span>|<span data-ttu-id="c5474-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5474-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="c5474-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="c5474-160">extensionId</span></span>|<span data-ttu-id="c5474-161">string</span><span class="sxs-lookup"><span data-stu-id="c5474-161">string</span></span>|<span data-ttu-id="c5474-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5474-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c5474-165">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5474-165">Request headers</span></span>
| <span data-ttu-id="c5474-166">Имя</span><span class="sxs-lookup"><span data-stu-id="c5474-166">Name</span></span>       | <span data-ttu-id="c5474-167">Значение</span><span class="sxs-lookup"><span data-stu-id="c5474-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c5474-168">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5474-168">Authorization</span></span> | <span data-ttu-id="c5474-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5474-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5474-171">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5474-171">Request body</span></span>
<span data-ttu-id="c5474-172">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5474-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5474-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5474-173">Response</span></span>

<span data-ttu-id="c5474-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c5474-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5474-176">Пример</span><span class="sxs-lookup"><span data-stu-id="c5474-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5474-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5474-177">Request</span></span>
<span data-ttu-id="c5474-178">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="c5474-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c5474-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5474-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c5474-180">C#</span><span class="sxs-lookup"><span data-stu-id="c5474-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5474-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5474-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c5474-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c5474-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c5474-183">Java</span><span class="sxs-lookup"><span data-stu-id="c5474-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c5474-184">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="c5474-184">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="c5474-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5474-185">Response</span></span>
<span data-ttu-id="c5474-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5474-186">Here is an example of the response.</span></span>
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
