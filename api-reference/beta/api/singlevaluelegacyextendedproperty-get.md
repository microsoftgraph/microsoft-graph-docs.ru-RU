---
title: Получение объекта singleValueLegacyExtendedProperty
description: Можно получить один экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурса.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c10c8ccb8ee1b4d4fb8fc8bc6af20ead736db777
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991249"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="cbccd-103">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="cbccd-103">Get singleValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbccd-104">Вы можете получить отдельный экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурсов, включающую расширенные свойства, которые соответствуют фильтру.</span><span class="sxs-lookup"><span data-stu-id="cbccd-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="cbccd-105">Параметр запроса `$expand` позволяет получить указанный экземпляр ресурса, дополненный определенным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="cbccd-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="cbccd-106">Используйте операторы `$filter` и `eq` в свойстве **id**, чтобы указать расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="cbccd-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="cbccd-107">На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="cbccd-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="cbccd-108">Чтобы получить экземпляры ресурсов, которые содержат определенные расширенные свойства, используйте параметр запроса `$filter` и примените оператор `eq` к свойству **id**.</span><span class="sxs-lookup"><span data-stu-id="cbccd-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="cbccd-109">Кроме того, для числовых расширенных свойств примените один из следующих операторов к свойству **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="cbccd-110">Для расширенных свойств строкового типа примените оператор `contains`, `startswith`, `eq` или `ne` к свойству **value**.</span><span class="sxs-lookup"><span data-stu-id="cbccd-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="cbccd-111">При фильтрации имени строки (`Name`) в свойстве **id** расширенного свойства учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="cbccd-111">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="cbccd-112">При фильтрации свойства **value** расширенного свойства регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="cbccd-112">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="cbccd-113">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="cbccd-113">The following user resources are supported:</span></span>

- <span data-ttu-id="cbccd-114">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="cbccd-114">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="cbccd-115">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="cbccd-115">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="cbccd-116">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="cbccd-116">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="cbccd-117">event</span><span class="sxs-lookup"><span data-stu-id="cbccd-117">event</span></span>](../resources/event.md)
- [<span data-ttu-id="cbccd-118">mailFolder</span><span class="sxs-lookup"><span data-stu-id="cbccd-118">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="cbccd-119">message</span><span class="sxs-lookup"><span data-stu-id="cbccd-119">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="cbccd-120">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="cbccd-120">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="cbccd-121">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="cbccd-121">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="cbccd-122">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="cbccd-122">As well as the following group resources:</span></span>

- <span data-ttu-id="cbccd-123">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="cbccd-123">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="cbccd-124">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="cbccd-124">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="cbccd-125">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="cbccd-125">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="cbccd-126">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="cbccd-126">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbccd-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbccd-127">Permissions</span></span>
<span data-ttu-id="cbccd-128">В зависимости от ресурса, из которого вы получаете расширенное свойство, а также от запрашиваемого типа разрешения (делегированного или приложения), для вызова этого API требуется минимум разрешение, указанное в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="cbccd-128">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="cbccd-129">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbccd-129">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbccd-130">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="cbccd-130">Supported resource</span></span> | <span data-ttu-id="cbccd-131">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbccd-131">Delegated (work or school account)</span></span> | <span data-ttu-id="cbccd-132">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbccd-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbccd-133">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbccd-133">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="cbccd-134">calendar</span><span class="sxs-lookup"><span data-stu-id="cbccd-134">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="cbccd-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-135">Calendars.Read</span></span> | <span data-ttu-id="cbccd-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-136">Calendars.Read</span></span> | <span data-ttu-id="cbccd-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-137">Calendars.Read</span></span> |
| [<span data-ttu-id="cbccd-138">contact</span><span class="sxs-lookup"><span data-stu-id="cbccd-138">contact</span></span>](../resources/contact.md) | <span data-ttu-id="cbccd-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-139">Contacts.Read</span></span> | <span data-ttu-id="cbccd-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-140">Contacts.Read</span></span> | <span data-ttu-id="cbccd-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-141">Contacts.Read</span></span> |
| <span data-ttu-id="cbccd-142">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="cbccd-142">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="cbccd-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-143">Contacts.Read</span></span> | <span data-ttu-id="cbccd-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-144">Contacts.Read</span></span> | <span data-ttu-id="cbccd-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-145">Contacts.Read</span></span> |
| [<span data-ttu-id="cbccd-146">event</span><span class="sxs-lookup"><span data-stu-id="cbccd-146">event</span></span>](../resources/event.md) | <span data-ttu-id="cbccd-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-147">Calendars.Read</span></span> | <span data-ttu-id="cbccd-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-148">Calendars.Read</span></span> |  <span data-ttu-id="cbccd-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-149">Calendars.Read</span></span>|
| <span data-ttu-id="cbccd-150">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="cbccd-150">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="cbccd-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbccd-151">Group.Read.All</span></span> | <span data-ttu-id="cbccd-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbccd-152">Not supported</span></span> | <span data-ttu-id="cbccd-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbccd-153">Not supported</span></span> |
| <span data-ttu-id="cbccd-154">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="cbccd-154">group [event](../resources/event.md)</span></span> | <span data-ttu-id="cbccd-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbccd-155">Group.Read.All</span></span> | <span data-ttu-id="cbccd-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbccd-156">Not supported</span></span> | <span data-ttu-id="cbccd-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbccd-157">Not supported</span></span> |
| <span data-ttu-id="cbccd-158">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="cbccd-158">group [post](../resources/post.md)</span></span> | <span data-ttu-id="cbccd-159">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbccd-159">Group.Read.All</span></span> | <span data-ttu-id="cbccd-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbccd-160">Not supported</span></span> | <span data-ttu-id="cbccd-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbccd-161">Group.Read.All</span></span> |
| [<span data-ttu-id="cbccd-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="cbccd-162">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="cbccd-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-163">Mail.Read</span></span> | <span data-ttu-id="cbccd-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-164">Mail.Read</span></span> | <span data-ttu-id="cbccd-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-165">Mail.Read</span></span> |
| [<span data-ttu-id="cbccd-166">message</span><span class="sxs-lookup"><span data-stu-id="cbccd-166">message</span></span>](../resources/message.md) | <span data-ttu-id="cbccd-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-167">Mail.Read</span></span> | <span data-ttu-id="cbccd-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-168">Mail.Read</span></span> | <span data-ttu-id="cbccd-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-169">Mail.Read</span></span> |
| [<span data-ttu-id="cbccd-170">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="cbccd-170">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="cbccd-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-171">Tasks.Read</span></span> | <span data-ttu-id="cbccd-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-172">Tasks.Read</span></span> | <span data-ttu-id="cbccd-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbccd-173">Not supported</span></span> |
| [<span data-ttu-id="cbccd-174">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="cbccd-174">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="cbccd-175">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-175">Tasks.Read</span></span> | <span data-ttu-id="cbccd-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cbccd-176">Tasks.Read</span></span> | <span data-ttu-id="cbccd-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbccd-177">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="cbccd-178">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbccd-178">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="cbccd-179">Получение экземпляра ресурса, дополненного расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="cbccd-179">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="cbccd-p105">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="cbccd-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="cbccd-182">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-182">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="cbccd-183">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-183">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="cbccd-184">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-184">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="cbccd-185">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-185">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="cbccd-186">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-186">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="cbccd-187">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-187">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="cbccd-188">Получение экземпляра **outlookTask** :</span><span class="sxs-lookup"><span data-stu-id="cbccd-188">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="cbccd-189">Получение экземпляра **outlookTaskFolder** :</span><span class="sxs-lookup"><span data-stu-id="cbccd-189">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="cbccd-190">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="cbccd-190">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="cbccd-191">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="cbccd-191">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="cbccd-192">Получение экземпляров ресурсов с числовыми расширенными свойствами, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="cbccd-192">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="cbccd-193">Получите экземпляры поддерживаемого ресурса с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="cbccd-193">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="cbccd-194">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-194">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="cbccd-195">Убедитесь, что вы применяете [кодировку URL-адреса](https://www.w3schools.com/tags/ref_urlencode.asp) к следующим символам в строке фильтра — двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="cbccd-195">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="cbccd-196">В приведенных ниже строках синтаксиса показан фильтр, в случае которого один оператор `eq` используется для свойства id, а другой оператор `eq` — для свойства value.</span><span class="sxs-lookup"><span data-stu-id="cbccd-196">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="cbccd-197">Вы можете заменить оператор `eq` для свойства **value** любым из других операторов (`ne`, `ge`, `gt`, `le` или `lt`), которые применяются к числовым значениям.</span><span class="sxs-lookup"><span data-stu-id="cbccd-197">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="cbccd-198">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-198">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="cbccd-199">Получение экземпляров объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-199">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="cbccd-200">Список экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-200">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="cbccd-201">Получение экземпляров объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-201">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="cbccd-202">Получение экземпляров объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-202">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="cbccd-203">Получение экземпляров объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-203">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="cbccd-204">Получение экземпляра **outlookTask** :</span><span class="sxs-lookup"><span data-stu-id="cbccd-204">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="cbccd-205">Получение экземпляра **outlookTaskFolder** :</span><span class="sxs-lookup"><span data-stu-id="cbccd-205">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="cbccd-206">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="cbccd-206">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="cbccd-207">Получение экземпляров объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="cbccd-207">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="cbccd-208">Получение экземпляров ресурсов с расширенными свойствами строкового типа, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="cbccd-208">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="cbccd-209">Получите экземпляры ресурса **message** или **event**, которые включают расширенное свойство строкового типа, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="cbccd-209">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="cbccd-210">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `contains`, `startswith`, `eq` или `ne`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-210">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="cbccd-211">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="cbccd-211">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="cbccd-212">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-212">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="cbccd-213">Получение экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="cbccd-213">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="cbccd-214">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="cbccd-214">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="cbccd-215">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="cbccd-215">Path parameters</span></span>
|<span data-ttu-id="cbccd-216">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="cbccd-216">**Parameter**</span></span>|<span data-ttu-id="cbccd-217">**Тип**</span><span class="sxs-lookup"><span data-stu-id="cbccd-217">**Type**</span></span>|<span data-ttu-id="cbccd-218">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cbccd-218">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cbccd-219">id_value</span><span class="sxs-lookup"><span data-stu-id="cbccd-219">id_value</span></span>|<span data-ttu-id="cbccd-220">String</span><span class="sxs-lookup"><span data-stu-id="cbccd-220">String</span></span>|<span data-ttu-id="cbccd-p109">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbccd-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="cbccd-225">property_value</span><span class="sxs-lookup"><span data-stu-id="cbccd-225">property_value</span></span> |<span data-ttu-id="cbccd-226">String</span><span class="sxs-lookup"><span data-stu-id="cbccd-226">String</span></span>|<span data-ttu-id="cbccd-227">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="cbccd-227">The value of the extended property to match.</span></span> <span data-ttu-id="cbccd-228">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="cbccd-228">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="cbccd-229">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="cbccd-229">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="cbccd-230">Примеры см. в разделе [Запрос 4](#request-4).</span><span class="sxs-lookup"><span data-stu-id="cbccd-230">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cbccd-231">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbccd-231">Request headers</span></span>
| <span data-ttu-id="cbccd-232">Имя</span><span class="sxs-lookup"><span data-stu-id="cbccd-232">Name</span></span>      |<span data-ttu-id="cbccd-233">Описание</span><span class="sxs-lookup"><span data-stu-id="cbccd-233">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cbccd-234">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbccd-234">Authorization</span></span>  | <span data-ttu-id="cbccd-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbccd-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbccd-237">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cbccd-237">Request body</span></span>
<span data-ttu-id="cbccd-238">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbccd-238">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbccd-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbccd-239">Response</span></span>

<span data-ttu-id="cbccd-240">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-240">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="cbccd-241">Запрос GET на получение экземпляра ресурса с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="cbccd-241">GET resource instance using `$expand`</span></span>
<span data-ttu-id="cbccd-242">Тело отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="cbccd-242">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="cbccd-243">Получение экземпляров ресурсов с расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="cbccd-243">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="cbccd-244">Тело отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="cbccd-244">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="cbccd-245">Тело отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="cbccd-245">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="cbccd-246">Пример</span><span class="sxs-lookup"><span data-stu-id="cbccd-246">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="cbccd-247">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="cbccd-247">Request 1</span></span>

<span data-ttu-id="cbccd-p113">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="cbccd-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cbccd-250">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbccd-250">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cbccd-251">C#</span><span class="sxs-lookup"><span data-stu-id="cbccd-251">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-singlevaluelegacyextendedproperty-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbccd-252">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbccd-252">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-singlevaluelegacyextendedproperty-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cbccd-253">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cbccd-253">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-singlevaluelegacyextendedproperty-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cbccd-254">Java</span><span class="sxs-lookup"><span data-stu-id="cbccd-254">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-singlevaluelegacyextendedproperty-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-1"></a><span data-ttu-id="cbccd-255">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="cbccd-255">Response 1</span></span>
<span data-ttu-id="cbccd-256">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="cbccd-256">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="cbccd-p114">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbccd-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="cbccd-259">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="cbccd-259">Request 2</span></span>

<span data-ttu-id="cbccd-260">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="cbccd-260">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="cbccd-261">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="cbccd-261">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="cbccd-262">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="cbccd-262">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="cbccd-263">его свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-263">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="cbccd-264">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="cbccd-264">Response 2</span></span>

<span data-ttu-id="cbccd-p116">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user-list-messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="cbccd-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="cbccd-268">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="cbccd-268">Request 3</span></span>

<span data-ttu-id="cbccd-269">В третьем примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством строкового типа.</span><span class="sxs-lookup"><span data-stu-id="cbccd-269">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="cbccd-270">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="cbccd-270">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="cbccd-271">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="cbccd-271">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="cbccd-272">его свойство **value** включает строку `green`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-272">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="cbccd-273">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="cbccd-273">Response 3</span></span>

<span data-ttu-id="cbccd-274">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а тело отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="cbccd-274">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="cbccd-275">Например, сообщение, которое содержит однозначное расширенное свойство со свойством **id**, равным строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, и свойством **value**, равным строке `Light green`, будет соответствовать фильтру и включено в отклик.</span><span class="sxs-lookup"><span data-stu-id="cbccd-275">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="cbccd-276">Тело отклика такое же, как при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="cbccd-276">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="cbccd-277">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="cbccd-277">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="cbccd-278">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="cbccd-278">Request 4</span></span>

<span data-ttu-id="cbccd-279">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от строкового.</span><span class="sxs-lookup"><span data-stu-id="cbccd-279">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="cbccd-280">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="cbccd-280">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="cbccd-281">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="cbccd-281">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="cbccd-282">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-282">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="cbccd-283">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-283">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="cbccd-284">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-284">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="cbccd-285">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="cbccd-285">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="cbccd-286">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-286">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="cbccd-287">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="cbccd-287">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="cbccd-288">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="cbccd-288">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="cbccd-289">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="cbccd-289">Response 4</span></span>

<span data-ttu-id="cbccd-290">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="cbccd-290">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="cbccd-291">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="cbccd-291">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="cbccd-292">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="cbccd-292">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
