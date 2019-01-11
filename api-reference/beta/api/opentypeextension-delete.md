---
title: Удаление открытого расширения
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
localization_priority: Normal
ms.openlocfilehash: 57b496692a976610b458f1452a179dbdb26467ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826952"
---
# <a name="delete-open-extension"></a><span data-ttu-id="334a8-103">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="334a8-103">Delete open extension</span></span>

> <span data-ttu-id="334a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="334a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="334a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="334a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="334a8-106">Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="334a8-106">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="334a8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="334a8-107">Permissions</span></span>

<span data-ttu-id="334a8-108">В зависимости от разрешений и ресурсов, который необходимо удалить данное расширение имени файла из типа (делегированные или приложение) запрошенный, разрешение, указанное в следующей таблице минимальными правами требуется для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="334a8-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="334a8-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="334a8-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="334a8-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="334a8-110">Supported resource</span></span> | <span data-ttu-id="334a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="334a8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="334a8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="334a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="334a8-113">Application</span><span class="sxs-lookup"><span data-stu-id="334a8-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="334a8-114">device</span><span class="sxs-lookup"><span data-stu-id="334a8-114">device</span></span>](../resources/device.md) | <span data-ttu-id="334a8-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="334a8-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="334a8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="334a8-116">Not supported</span></span> | <span data-ttu-id="334a8-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="334a8-118">event</span><span class="sxs-lookup"><span data-stu-id="334a8-118">event</span></span>](../resources/event.md) | <span data-ttu-id="334a8-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="334a8-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="334a8-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="334a8-122">group</span><span class="sxs-lookup"><span data-stu-id="334a8-122">group</span></span>](../resources/group.md) | <span data-ttu-id="334a8-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="334a8-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="334a8-124">Not supported</span></span> | <span data-ttu-id="334a8-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-125">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="334a8-126">[event](../resources/event.md) для групп</span><span class="sxs-lookup"><span data-stu-id="334a8-126">[group event](../resources/event.md)</span></span> | <span data-ttu-id="334a8-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="334a8-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="334a8-128">Not supported</span></span> | <span data-ttu-id="334a8-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="334a8-129">Not supported</span></span> |
| <span data-ttu-id="334a8-130">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="334a8-130">[group post](../resources/post.md)</span></span> | <span data-ttu-id="334a8-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="334a8-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="334a8-132">Not supported</span></span> | <span data-ttu-id="334a8-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="334a8-134">message</span><span class="sxs-lookup"><span data-stu-id="334a8-134">message</span></span>](../resources/message.md) | <span data-ttu-id="334a8-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-135">Mail.ReadWrite</span></span> | <span data-ttu-id="334a8-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-136">Mail.ReadWrite</span></span> | <span data-ttu-id="334a8-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="334a8-138">organization</span><span class="sxs-lookup"><span data-stu-id="334a8-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="334a8-139">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="334a8-139">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="334a8-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="334a8-140">Not supported</span></span> | <span data-ttu-id="334a8-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="334a8-141">Not supported</span></span> |
| <span data-ttu-id="334a8-142">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="334a8-142">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="334a8-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="334a8-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="334a8-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="334a8-146">user</span><span class="sxs-lookup"><span data-stu-id="334a8-146">user</span></span>](../resources/user.md) | <span data-ttu-id="334a8-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-147">User.ReadWrite.All</span></span> | <span data-ttu-id="334a8-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="334a8-148">User.ReadWrite</span></span> | <span data-ttu-id="334a8-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334a8-149">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="334a8-150">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="334a8-150">HTTP request</span></span>

<span data-ttu-id="334a8-151">В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.</span><span class="sxs-lookup"><span data-stu-id="334a8-151">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="334a8-p103">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.</span><span class="sxs-lookup"><span data-stu-id="334a8-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="334a8-154">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="334a8-154">Path parameters</span></span>
|<span data-ttu-id="334a8-155">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="334a8-155">**Parameter**</span></span>|<span data-ttu-id="334a8-156">**Тип**</span><span class="sxs-lookup"><span data-stu-id="334a8-156">**Type**</span></span>|<span data-ttu-id="334a8-157">**Описание**</span><span class="sxs-lookup"><span data-stu-id="334a8-157">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="334a8-158">id</span><span class="sxs-lookup"><span data-stu-id="334a8-158">id</span></span>|<span data-ttu-id="334a8-159">строка</span><span class="sxs-lookup"><span data-stu-id="334a8-159">string</span></span>|<span data-ttu-id="334a8-p104">Уникальный идентификатор экземпляра в соответствующей коллекции. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="334a8-p104">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="334a8-162">extensionId</span><span class="sxs-lookup"><span data-stu-id="334a8-162">extensionId</span></span>|<span data-ttu-id="334a8-163">string</span><span class="sxs-lookup"><span data-stu-id="334a8-163">string</span></span>|<span data-ttu-id="334a8-p105">Этот параметр может быть именем расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полным именем, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве `id` при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="334a8-p105">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="334a8-167">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="334a8-167">Request headers</span></span>
| <span data-ttu-id="334a8-168">Имя</span><span class="sxs-lookup"><span data-stu-id="334a8-168">Name</span></span>       | <span data-ttu-id="334a8-169">Значение</span><span class="sxs-lookup"><span data-stu-id="334a8-169">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="334a8-170">Авторизация</span><span class="sxs-lookup"><span data-stu-id="334a8-170">Authorization</span></span> | <span data-ttu-id="334a8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="334a8-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="334a8-173">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="334a8-173">Request body</span></span>
<span data-ttu-id="334a8-174">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="334a8-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="334a8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="334a8-175">Response</span></span>

<span data-ttu-id="334a8-p107">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="334a8-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="334a8-178">Пример</span><span class="sxs-lookup"><span data-stu-id="334a8-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="334a8-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="334a8-179">Request</span></span>
<span data-ttu-id="334a8-180">В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.</span><span class="sxs-lookup"><span data-stu-id="334a8-180">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="334a8-181">Во втором примере показано, как удалить расширение в событии указанной группы.</span><span class="sxs-lookup"><span data-stu-id="334a8-181">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="334a8-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="334a8-182">Response</span></span>
<span data-ttu-id="334a8-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="334a8-183">Here is an example of the response.</span></span>
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
