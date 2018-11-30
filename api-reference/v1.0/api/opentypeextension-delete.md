---
title: Удаление открытого расширения
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
ms.openlocfilehash: 9906b0b68711f1bb78d220252366b0c4a56592fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028325"
---
# <a name="delete-open-extension"></a><span data-ttu-id="a1c5f-103">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="a1c5f-103">Delete open extension</span></span>

<span data-ttu-id="a1c5f-104">Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a1c5f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1c5f-105">Permissions</span></span>

<span data-ttu-id="a1c5f-106">В зависимости от разрешений и ресурсов, который необходимо удалить данное расширение имени файла из типа (делегированные или приложение) запрошенный, разрешение, указанное в следующей таблице минимальными правами требуется для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a1c5f-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1c5f-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1c5f-108">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="a1c5f-108">Supported resource</span></span> | <span data-ttu-id="a1c5f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1c5f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a1c5f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1c5f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1c5f-111">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a1c5f-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="a1c5f-112">device</span><span class="sxs-lookup"><span data-stu-id="a1c5f-112">device</span></span>](../resources/device.md) | <span data-ttu-id="a1c5f-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="a1c5f-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1c5f-114">Not supported</span></span> | <span data-ttu-id="a1c5f-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="a1c5f-116">event</span><span class="sxs-lookup"><span data-stu-id="a1c5f-116">event</span></span>](../resources/event.md) | <span data-ttu-id="a1c5f-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="a1c5f-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="a1c5f-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="a1c5f-120">group</span><span class="sxs-lookup"><span data-stu-id="a1c5f-120">group</span></span>](../resources/group.md) | <span data-ttu-id="a1c5f-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="a1c5f-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1c5f-122">Not supported</span></span> | <span data-ttu-id="a1c5f-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-123">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a1c5f-124">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="a1c5f-124">[group event](../resources/event.md)</span></span> | <span data-ttu-id="a1c5f-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="a1c5f-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1c5f-126">Not supported</span></span> | <span data-ttu-id="a1c5f-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1c5f-127">Not supported</span></span> |
| <span data-ttu-id="a1c5f-128">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="a1c5f-128">[group post](../resources/post.md)</span></span> | <span data-ttu-id="a1c5f-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="a1c5f-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1c5f-130">Not supported</span></span> | <span data-ttu-id="a1c5f-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="a1c5f-132">message</span><span class="sxs-lookup"><span data-stu-id="a1c5f-132">message</span></span>](../resources/message.md) | <span data-ttu-id="a1c5f-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-133">Mail.ReadWrite</span></span> | <span data-ttu-id="a1c5f-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-134">Mail.ReadWrite</span></span> | <span data-ttu-id="a1c5f-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="a1c5f-136">organization</span><span class="sxs-lookup"><span data-stu-id="a1c5f-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="a1c5f-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="a1c5f-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1c5f-138">Not supported</span></span> | <span data-ttu-id="a1c5f-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1c5f-139">Not supported</span></span> |
| <span data-ttu-id="a1c5f-140">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="a1c5f-140">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="a1c5f-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="a1c5f-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="a1c5f-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="a1c5f-144">user</span><span class="sxs-lookup"><span data-stu-id="a1c5f-144">user</span></span>](../resources/user.md) | <span data-ttu-id="a1c5f-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-145">User.ReadWrite.All</span></span> | <span data-ttu-id="a1c5f-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1c5f-146">User.ReadWrite</span></span> | <span data-ttu-id="a1c5f-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1c5f-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1c5f-148">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1c5f-148">HTTP request</span></span>
<span data-ttu-id="a1c5f-149">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="a1c5f-p102">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="a1c5f-152">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="a1c5f-152">Path parameters</span></span>
|<span data-ttu-id="a1c5f-153">Параметр</span><span class="sxs-lookup"><span data-stu-id="a1c5f-153">Parameter</span></span>|<span data-ttu-id="a1c5f-154">Тип</span><span class="sxs-lookup"><span data-stu-id="a1c5f-154">Type</span></span>|<span data-ttu-id="a1c5f-155">Описание</span><span class="sxs-lookup"><span data-stu-id="a1c5f-155">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a1c5f-156">id</span><span class="sxs-lookup"><span data-stu-id="a1c5f-156">id</span></span>|<span data-ttu-id="a1c5f-157">строка</span><span class="sxs-lookup"><span data-stu-id="a1c5f-157">string</span></span>|<span data-ttu-id="a1c5f-p103">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="a1c5f-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="a1c5f-160">extensionId</span></span>|<span data-ttu-id="a1c5f-161">string</span><span class="sxs-lookup"><span data-stu-id="a1c5f-161">string</span></span>|<span data-ttu-id="a1c5f-p104">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a1c5f-165">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1c5f-165">Request headers</span></span>
| <span data-ttu-id="a1c5f-166">Имя</span><span class="sxs-lookup"><span data-stu-id="a1c5f-166">Name</span></span>       | <span data-ttu-id="a1c5f-167">Значение</span><span class="sxs-lookup"><span data-stu-id="a1c5f-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a1c5f-168">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1c5f-168">Authorization</span></span> | <span data-ttu-id="a1c5f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1c5f-171">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1c5f-171">Request body</span></span>
<span data-ttu-id="a1c5f-172">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1c5f-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1c5f-173">Response</span></span>

<span data-ttu-id="a1c5f-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1c5f-176">Пример</span><span class="sxs-lookup"><span data-stu-id="a1c5f-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1c5f-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1c5f-177">Request</span></span>
<span data-ttu-id="a1c5f-178">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="a1c5f-179">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-179">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="a1c5f-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1c5f-180">Response</span></span>
<span data-ttu-id="a1c5f-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1c5f-181">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->