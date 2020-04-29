---
title: Удаление открытого расширения
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78de314eb75a1950c062ca34eaa66409abffd7d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511266"
---
# <a name="delete-open-extension"></a><span data-ttu-id="73c8f-103">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="73c8f-103">Delete open extension</span></span>

<span data-ttu-id="73c8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73c8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73c8f-105">Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="73c8f-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="73c8f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73c8f-106">Permissions</span></span>

<span data-ttu-id="73c8f-107">В зависимости от ресурса, из которого вы удаляете расширение, и запрошенного типа разрешения (делегированного или приложения), разрешение, указанное в следующей таблице, является минимальным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="73c8f-107">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="73c8f-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73c8f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73c8f-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="73c8f-109">Supported resource</span></span> | <span data-ttu-id="73c8f-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73c8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73c8f-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73c8f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73c8f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73c8f-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="73c8f-113">device</span><span class="sxs-lookup"><span data-stu-id="73c8f-113">device</span></span>](../resources/device.md) | <span data-ttu-id="73c8f-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="73c8f-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73c8f-115">Not supported</span></span> | <span data-ttu-id="73c8f-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="73c8f-117">event</span><span class="sxs-lookup"><span data-stu-id="73c8f-117">event</span></span>](../resources/event.md) | <span data-ttu-id="73c8f-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="73c8f-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="73c8f-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="73c8f-121">group</span><span class="sxs-lookup"><span data-stu-id="73c8f-121">group</span></span>](../resources/group.md) | <span data-ttu-id="73c8f-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="73c8f-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73c8f-123">Not supported</span></span> | <span data-ttu-id="73c8f-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-124">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="73c8f-125">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="73c8f-125">[group event](../resources/event.md)</span></span> | <span data-ttu-id="73c8f-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="73c8f-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73c8f-127">Not supported</span></span> | <span data-ttu-id="73c8f-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73c8f-128">Not supported</span></span> |
| <span data-ttu-id="73c8f-129">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="73c8f-129">[group post](../resources/post.md)</span></span> | <span data-ttu-id="73c8f-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="73c8f-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73c8f-131">Not supported</span></span> | <span data-ttu-id="73c8f-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="73c8f-133">message</span><span class="sxs-lookup"><span data-stu-id="73c8f-133">message</span></span>](../resources/message.md) | <span data-ttu-id="73c8f-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-134">Mail.ReadWrite</span></span> | <span data-ttu-id="73c8f-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-135">Mail.ReadWrite</span></span> | <span data-ttu-id="73c8f-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="73c8f-137">organization</span><span class="sxs-lookup"><span data-stu-id="73c8f-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="73c8f-138">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-138">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="73c8f-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73c8f-139">Not supported</span></span> | <span data-ttu-id="73c8f-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73c8f-140">Not supported</span></span> |
| <span data-ttu-id="73c8f-141">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="73c8f-141">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="73c8f-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="73c8f-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="73c8f-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="73c8f-145">user</span><span class="sxs-lookup"><span data-stu-id="73c8f-145">user</span></span>](../resources/user.md) | <span data-ttu-id="73c8f-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-146">User.ReadWrite.All</span></span> | <span data-ttu-id="73c8f-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73c8f-147">User.ReadWrite</span></span> | <span data-ttu-id="73c8f-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73c8f-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73c8f-149">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73c8f-149">HTTP request</span></span>
<span data-ttu-id="73c8f-150">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="73c8f-150">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
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

><span data-ttu-id="73c8f-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="73c8f-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="73c8f-153">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="73c8f-153">Path parameters</span></span>
|<span data-ttu-id="73c8f-154">Параметр</span><span class="sxs-lookup"><span data-stu-id="73c8f-154">Parameter</span></span>|<span data-ttu-id="73c8f-155">Тип</span><span class="sxs-lookup"><span data-stu-id="73c8f-155">Type</span></span>|<span data-ttu-id="73c8f-156">Описание</span><span class="sxs-lookup"><span data-stu-id="73c8f-156">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73c8f-157">id</span><span class="sxs-lookup"><span data-stu-id="73c8f-157">id</span></span>|<span data-ttu-id="73c8f-158">строка</span><span class="sxs-lookup"><span data-stu-id="73c8f-158">string</span></span>|<span data-ttu-id="73c8f-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73c8f-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="73c8f-161">extensionId</span><span class="sxs-lookup"><span data-stu-id="73c8f-161">extensionId</span></span>|<span data-ttu-id="73c8f-162">string</span><span class="sxs-lookup"><span data-stu-id="73c8f-162">string</span></span>|<span data-ttu-id="73c8f-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73c8f-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="73c8f-166">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73c8f-166">Request headers</span></span>
| <span data-ttu-id="73c8f-167">Имя</span><span class="sxs-lookup"><span data-stu-id="73c8f-167">Name</span></span>       | <span data-ttu-id="73c8f-168">Значение</span><span class="sxs-lookup"><span data-stu-id="73c8f-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="73c8f-169">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73c8f-169">Authorization</span></span> | <span data-ttu-id="73c8f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73c8f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73c8f-172">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73c8f-172">Request body</span></span>
<span data-ttu-id="73c8f-173">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73c8f-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73c8f-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="73c8f-174">Response</span></span>

<span data-ttu-id="73c8f-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="73c8f-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73c8f-177">Пример</span><span class="sxs-lookup"><span data-stu-id="73c8f-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73c8f-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="73c8f-178">Request</span></span>
<span data-ttu-id="73c8f-179">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="73c8f-179">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="73c8f-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="73c8f-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="73c8f-181">C#</span><span class="sxs-lookup"><span data-stu-id="73c8f-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73c8f-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73c8f-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73c8f-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73c8f-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73c8f-184">Java</span><span class="sxs-lookup"><span data-stu-id="73c8f-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="73c8f-185">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="73c8f-185">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="73c8f-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="73c8f-186">Response</span></span>
<span data-ttu-id="73c8f-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73c8f-187">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
