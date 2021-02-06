---
title: Получение объекта singleValueLegacyExtendedProperty
description: Можно получить один экземпляр ресурса, расширенный с определенным расширенным свойством, или коллекцию экземпляров ресурсов
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: dedb7eefacd028a837c39b3712ec6f61e0ee032f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134094"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="e3ff4-103">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e3ff4-103">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="e3ff4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3ff4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="e3ff4-105">Вы можете получить отдельный экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурсов, включающую расширенные свойства, которые соответствуют фильтру.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-105">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="e3ff4-106">Параметр запроса `$expand` позволяет получить указанный экземпляр ресурса, дополненный определенным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-106">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="e3ff4-107">Используйте операторы `$filter` и `eq` в свойстве **id**, чтобы указать расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-107">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="e3ff4-108">На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-108">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="e3ff4-109">Чтобы получить экземпляры ресурсов, которые содержат определенные расширенные свойства, используйте параметр запроса `$filter` и примените оператор `eq` к свойству **id**.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-109">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="e3ff4-110">Кроме того, для числовых расширенных свойств примените один из следующих операторов к свойству **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-110">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="e3ff4-111">Для расширенных свойств строкового типа примените оператор `contains`, `startswith`, `eq` или `ne` к свойству **value**.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-111">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="e3ff4-112">При фильтрации имени строки (`Name`) в свойстве **id** расширенного свойства учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-112">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="e3ff4-113">При фильтрации свойства **value** расширенного свойства регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-113">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="e3ff4-114">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-114">The following user resources are supported:</span></span>

- <span data-ttu-id="e3ff4-115">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="e3ff4-115">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e3ff4-116">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="e3ff4-116">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="e3ff4-117">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e3ff4-117">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="e3ff4-118">event</span><span class="sxs-lookup"><span data-stu-id="e3ff4-118">event</span></span>](../resources/event.md)
- [<span data-ttu-id="e3ff4-119">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e3ff4-119">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="e3ff4-120">message</span><span class="sxs-lookup"><span data-stu-id="e3ff4-120">message</span></span>](../resources/message.md)
- [<span data-ttu-id="e3ff4-121">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="e3ff4-121">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="e3ff4-122">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="e3ff4-122">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="e3ff4-123">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-123">As well as the following group resources:</span></span>

- <span data-ttu-id="e3ff4-124">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="e3ff4-124">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e3ff4-125">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="e3ff4-125">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="e3ff4-126">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-126">group [post](../resources/post.md)</span></span>

<span data-ttu-id="e3ff4-127">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e3ff4-127">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3ff4-128">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3ff4-128">Permissions</span></span>
<span data-ttu-id="e3ff4-129">В зависимости от ресурса, из которых вы получаете расширенное свойство, и типа запрашиваемого разрешения (делегирования или приложения), разрешение, указанное в следующей таблице, является минимальным требованием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-129">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="e3ff4-130">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3ff4-130">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3ff4-131">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="e3ff4-131">Supported resource</span></span> | <span data-ttu-id="e3ff4-132">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3ff4-132">Delegated (work or school account)</span></span> | <span data-ttu-id="e3ff4-133">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3ff4-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3ff4-134">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3ff4-134">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="e3ff4-135">calendar</span><span class="sxs-lookup"><span data-stu-id="e3ff4-135">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="e3ff4-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-136">Calendars.Read</span></span> | <span data-ttu-id="e3ff4-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-137">Calendars.Read</span></span> | <span data-ttu-id="e3ff4-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-138">Calendars.Read</span></span> |
| [<span data-ttu-id="e3ff4-139">contact</span><span class="sxs-lookup"><span data-stu-id="e3ff4-139">contact</span></span>](../resources/contact.md) | <span data-ttu-id="e3ff4-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-140">Contacts.Read</span></span> | <span data-ttu-id="e3ff4-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-141">Contacts.Read</span></span> | <span data-ttu-id="e3ff4-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-142">Contacts.Read</span></span> |
| [<span data-ttu-id="e3ff4-143">contactFolder</span><span class="sxs-lookup"><span data-stu-id="e3ff4-143">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="e3ff4-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-144">Contacts.Read</span></span> | <span data-ttu-id="e3ff4-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-145">Contacts.Read</span></span> | <span data-ttu-id="e3ff4-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-146">Contacts.Read</span></span> |
| [<span data-ttu-id="e3ff4-147">event</span><span class="sxs-lookup"><span data-stu-id="e3ff4-147">event</span></span>](../resources/event.md) | <span data-ttu-id="e3ff4-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-148">Calendars.Read</span></span> | <span data-ttu-id="e3ff4-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-149">Calendars.Read</span></span> |  <span data-ttu-id="e3ff4-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-150">Calendars.Read</span></span>|
| <span data-ttu-id="e3ff4-151">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="e3ff4-151">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="e3ff4-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3ff4-152">Group.Read.All</span></span> | <span data-ttu-id="e3ff4-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3ff4-153">Not supported</span></span> | <span data-ttu-id="e3ff4-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3ff4-154">Not supported</span></span> |
| <span data-ttu-id="e3ff4-155">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="e3ff4-155">group [event](../resources/event.md)</span></span> | <span data-ttu-id="e3ff4-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3ff4-156">Group.Read.All</span></span> | <span data-ttu-id="e3ff4-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3ff4-157">Not supported</span></span> | <span data-ttu-id="e3ff4-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3ff4-158">Not supported</span></span> |
| <span data-ttu-id="e3ff4-159">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-159">group [post](../resources/post.md)</span></span> | <span data-ttu-id="e3ff4-160">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3ff4-160">Group.Read.All</span></span> | <span data-ttu-id="e3ff4-161">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3ff4-161">Not supported</span></span> | <span data-ttu-id="e3ff4-162">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3ff4-162">Group.Read.All</span></span> |
| [<span data-ttu-id="e3ff4-163">mailFolder</span><span class="sxs-lookup"><span data-stu-id="e3ff4-163">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="e3ff4-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-164">Mail.Read</span></span> | <span data-ttu-id="e3ff4-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-165">Mail.Read</span></span> | <span data-ttu-id="e3ff4-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-166">Mail.Read</span></span> |
| [<span data-ttu-id="e3ff4-167">message</span><span class="sxs-lookup"><span data-stu-id="e3ff4-167">message</span></span>](../resources/message.md) | <span data-ttu-id="e3ff4-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-168">Mail.Read</span></span> | <span data-ttu-id="e3ff4-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-169">Mail.Read</span></span> | <span data-ttu-id="e3ff4-170">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-170">Mail.Read</span></span> |
| [<span data-ttu-id="e3ff4-171">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="e3ff4-171">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="e3ff4-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-172">Tasks.Read</span></span> | <span data-ttu-id="e3ff4-173">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-173">Tasks.Read</span></span> | <span data-ttu-id="e3ff4-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3ff4-174">Not supported</span></span> |
| [<span data-ttu-id="e3ff4-175">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="e3ff4-175">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="e3ff4-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-176">Tasks.Read</span></span> | <span data-ttu-id="e3ff4-177">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e3ff4-177">Tasks.Read</span></span> | <span data-ttu-id="e3ff4-178">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3ff4-178">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="e3ff4-179">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3ff4-179">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="e3ff4-180">Получение экземпляра ресурса, дополненного расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="e3ff4-180">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="e3ff4-p105">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="e3ff4-183">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-183">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e3ff4-184">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-184">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="e3ff4-185">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-185">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e3ff4-186">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-186">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="e3ff4-187">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-187">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e3ff4-188">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-188">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="e3ff4-189">Получите экземпляр **outlookTask:**</span><span class="sxs-lookup"><span data-stu-id="e3ff4-189">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="e3ff4-190">Получите экземпляр **outlookTaskFolder:**</span><span class="sxs-lookup"><span data-stu-id="e3ff4-190">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="e3ff4-191">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-191">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="e3ff4-192">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-192">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="e3ff4-193">Получение экземпляров ресурсов с числовыми расширенными свойствами, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="e3ff4-193">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="e3ff4-194">Получите экземпляры поддерживаемого ресурса с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-194">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="e3ff4-195">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-195">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span>
<span data-ttu-id="e3ff4-196">Убедитесь, что вы [](https://www.w3schools.com/tags/ref_urlencode.asp) применяли кодику URL-адресов к следующим символам в строке фильтра — двоеточию, косой черте и пробелу.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-196">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="e3ff4-197">В приведенных ниже строках синтаксиса показан фильтр, в случае которого один оператор `eq` используется для свойства id, а другой оператор `eq` — для свойства value.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-197">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="e3ff4-198">Вы можете заменить оператор `eq` для свойства **value** любым из других операторов (`ne`, `ge`, `gt`, `le` или `lt`), которые применяются к числовым значениям.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-198">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="e3ff4-199">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-199">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e3ff4-200">Получение экземпляров объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-200">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="e3ff4-201">Список экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-201">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e3ff4-202">Получение экземпляров объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-202">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e3ff4-203">Получение экземпляров объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-203">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e3ff4-204">Получение экземпляров объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-204">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="e3ff4-205">Получите экземпляр **outlookTask:**</span><span class="sxs-lookup"><span data-stu-id="e3ff4-205">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="e3ff4-206">Получите экземпляр **outlookTaskFolder:**</span><span class="sxs-lookup"><span data-stu-id="e3ff4-206">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="e3ff4-207">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-207">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="e3ff4-208">Получение экземпляров объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-208">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="e3ff4-209">Получение экземпляров ресурсов с расширенными свойствами строкового типа, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="e3ff4-209">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="e3ff4-210">Получите экземпляры ресурса **message** или **event**, которые включают расширенное свойство строкового типа, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-210">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="e3ff4-211">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `contains`, `startswith`, `eq` или `ne`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-211">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="e3ff4-212">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-212">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="e3ff4-213">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-213">Get **message** instances:</span></span>
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

<span data-ttu-id="e3ff4-214">Получение экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-214">Get **event** instances:</span></span>
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

<span data-ttu-id="e3ff4-215">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-215">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="e3ff4-216">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e3ff4-216">Path parameters</span></span>
|<span data-ttu-id="e3ff4-217">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="e3ff4-217">**Parameter**</span></span>|<span data-ttu-id="e3ff4-218">**Тип**</span><span class="sxs-lookup"><span data-stu-id="e3ff4-218">**Type**</span></span>|<span data-ttu-id="e3ff4-219">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e3ff4-219">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e3ff4-220">id_value</span><span class="sxs-lookup"><span data-stu-id="e3ff4-220">id_value</span></span>|<span data-ttu-id="e3ff4-221">String</span><span class="sxs-lookup"><span data-stu-id="e3ff4-221">String</span></span>|<span data-ttu-id="e3ff4-p109">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="e3ff4-226">property_value</span><span class="sxs-lookup"><span data-stu-id="e3ff4-226">property_value</span></span> |<span data-ttu-id="e3ff4-227">String</span><span class="sxs-lookup"><span data-stu-id="e3ff4-227">String</span></span>|<span data-ttu-id="e3ff4-228">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-228">The value of the extended property to match.</span></span> <span data-ttu-id="e3ff4-229">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-229">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="e3ff4-230">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-230">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="e3ff4-231">Примеры см. в разделе [Запрос 4](#request-4).</span><span class="sxs-lookup"><span data-stu-id="e3ff4-231">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e3ff4-232">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3ff4-232">Request headers</span></span>
| <span data-ttu-id="e3ff4-233">Имя</span><span class="sxs-lookup"><span data-stu-id="e3ff4-233">Name</span></span>      |<span data-ttu-id="e3ff4-234">Описание</span><span class="sxs-lookup"><span data-stu-id="e3ff4-234">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3ff4-235">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3ff4-235">Authorization</span></span>  | <span data-ttu-id="e3ff4-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3ff4-238">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3ff4-238">Request body</span></span>
<span data-ttu-id="e3ff4-239">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-239">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3ff4-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3ff4-240">Response</span></span>

<span data-ttu-id="e3ff4-241">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-241">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="e3ff4-242">Запрос GET на получение экземпляра ресурса с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="e3ff4-242">GET resource instance using `$expand`</span></span>
<span data-ttu-id="e3ff4-243">Тело отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="e3ff4-243">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>

#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="e3ff4-244">Получение экземпляров ресурсов с расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="e3ff4-244">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="e3ff4-245">Тело отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-245">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="e3ff4-246">Тело отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-246">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="e3ff4-247">Пример</span><span class="sxs-lookup"><span data-stu-id="e3ff4-247">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e3ff4-248">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="e3ff4-248">Request 1</span></span>

<span data-ttu-id="e3ff4-p113">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="e3ff4-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>


# <a name="http"></a>[<span data-ttu-id="e3ff4-251">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3ff4-251">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
# <a name="c"></a>[<span data-ttu-id="e3ff4-252">C#</span><span class="sxs-lookup"><span data-stu-id="e3ff4-252">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-singlevaluelegacyextendedproperty-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3ff4-253">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3ff4-253">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-singlevaluelegacyextendedproperty-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3ff4-254">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3ff4-254">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-singlevaluelegacyextendedproperty-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3ff4-255">Java</span><span class="sxs-lookup"><span data-stu-id="e3ff4-255">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-singlevaluelegacyextendedproperty-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-1"></a><span data-ttu-id="e3ff4-256">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="e3ff4-256">Response 1</span></span>
<span data-ttu-id="e3ff4-257">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-257">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="e3ff4-p114">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="e3ff4-260">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="e3ff4-260">Request 2</span></span>

<span data-ttu-id="e3ff4-261">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-261">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="e3ff4-262">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-262">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="e3ff4-263">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="e3ff4-263">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="e3ff4-264">его свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-264">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="e3ff4-265">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="e3ff4-265">Response 2</span></span>

<span data-ttu-id="e3ff4-p116">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user-list-messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="e3ff4-269">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="e3ff4-269">Request 3</span></span>

<span data-ttu-id="e3ff4-270">В третьем примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством строкового типа.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-270">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="e3ff4-271">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-271">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="e3ff4-272">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="e3ff4-272">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="e3ff4-273">его свойство **value** включает строку `green`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-273">Its **value** containing the string `green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="e3ff4-274">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="e3ff4-274">Response 3</span></span>

<span data-ttu-id="e3ff4-275">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а тело отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-275">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="e3ff4-276">Например, сообщение, которое содержит однозначное расширенное свойство со свойством **id**, равным строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, и свойством **value**, равным строке `Light green`, будет соответствовать фильтру и включено в отклик.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-276">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="e3ff4-277">Тело отклика такое же, как при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="e3ff4-277">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="e3ff4-278">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-278">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="e3ff4-279">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="e3ff4-279">Request 4</span></span>

<span data-ttu-id="e3ff4-280">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от строкового.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-280">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="e3ff4-281">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-281">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="e3ff4-282">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-282">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="e3ff4-283">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-283">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="e3ff4-284">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-284">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="e3ff4-285">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-285">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="e3ff4-286">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="e3ff4-286">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="e3ff4-287">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-287">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="e3ff4-288">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-288">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="e3ff4-289">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-289">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="e3ff4-290">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="e3ff4-290">Response 4</span></span>

<span data-ttu-id="e3ff4-291">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-291">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="e3ff4-292">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="e3ff4-292">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="e3ff4-293">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="e3ff4-293">The response does not include the matching extended property.</span></span>


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


