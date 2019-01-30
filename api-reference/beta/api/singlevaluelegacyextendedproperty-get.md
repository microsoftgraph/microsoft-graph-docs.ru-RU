---
title: Получение объекта singleValueLegacyExtendedProperty
description: Можно получить экземпляр единственный ресурс, включающим определенное свойство расширенного или коллекцию экземпляров ресурсов
localization_priority: Normal
ms.openlocfilehash: ead4881737f4431138d444ffe8df131c22c131fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641409"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="de04e-103">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="de04e-103">Get singleValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de04e-104">Вы можете получить отдельный экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурсов, включающую расширенные свойства, которые соответствуют фильтру.</span><span class="sxs-lookup"><span data-stu-id="de04e-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="de04e-105">Параметр запроса `$expand` позволяет получить указанный экземпляр ресурса, дополненный определенным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="de04e-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="de04e-106">Используйте операторы `$filter` и `eq` в свойстве **id**, чтобы указать расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="de04e-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="de04e-107">На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="de04e-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="de04e-108">Чтобы получить экземпляры ресурсов, которые содержат определенные расширенные свойства, используйте параметр запроса `$filter` и примените оператор `eq` к свойству **id**.</span><span class="sxs-lookup"><span data-stu-id="de04e-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="de04e-109">Кроме того, для числовых расширенных свойств примените один из следующих операторов к свойству **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="de04e-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="de04e-110">Для расширенных свойств строкового типа примените оператор `contains`, `startswith`, `eq` или `ne` к свойству **value**.</span><span class="sxs-lookup"><span data-stu-id="de04e-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="de04e-111">При фильтрации имени строки (`Name`) в свойстве **id** расширенного свойства учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="de04e-111">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="de04e-112">При фильтрации свойства **value** расширенного свойства регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="de04e-112">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="de04e-113">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="de04e-113">The following user resources are supported:</span></span>

- <span data-ttu-id="de04e-114">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="de04e-114">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="de04e-115">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="de04e-115">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="de04e-116">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="de04e-116">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="de04e-117">event</span><span class="sxs-lookup"><span data-stu-id="de04e-117">event</span></span>](../resources/event.md)
- [<span data-ttu-id="de04e-118">mailFolder</span><span class="sxs-lookup"><span data-stu-id="de04e-118">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="de04e-119">message</span><span class="sxs-lookup"><span data-stu-id="de04e-119">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="de04e-120">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="de04e-120">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="de04e-121">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="de04e-121">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="de04e-122">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="de04e-122">As well as the following group resources:</span></span>

- <span data-ttu-id="de04e-123">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="de04e-123">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="de04e-124">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="de04e-124">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="de04e-125">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="de04e-125">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="de04e-126">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="de04e-126">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="de04e-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de04e-127">Permissions</span></span>
<span data-ttu-id="de04e-128">В зависимости от ресурса они будут расширенные свойства из и разрешение введите (делегированные или приложения) вы запроса, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="de04e-128">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="de04e-129">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de04e-129">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de04e-130">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="de04e-130">Supported resource</span></span> | <span data-ttu-id="de04e-131">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de04e-131">Delegated (work or school account)</span></span> | <span data-ttu-id="de04e-132">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de04e-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de04e-133">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de04e-133">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="de04e-134">calendar</span><span class="sxs-lookup"><span data-stu-id="de04e-134">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="de04e-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-135">Calendars.Read</span></span> | <span data-ttu-id="de04e-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-136">Calendars.Read</span></span> | <span data-ttu-id="de04e-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-137">Calendars.Read</span></span> |
| [<span data-ttu-id="de04e-138">contact</span><span class="sxs-lookup"><span data-stu-id="de04e-138">contact</span></span>](../resources/contact.md) | <span data-ttu-id="de04e-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-139">Contacts.Read</span></span> | <span data-ttu-id="de04e-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-140">Contacts.Read</span></span> | <span data-ttu-id="de04e-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-141">Contacts.Read</span></span> |
| <span data-ttu-id="de04e-142">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="de04e-142">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="de04e-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-143">Contacts.Read</span></span> | <span data-ttu-id="de04e-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-144">Contacts.Read</span></span> | <span data-ttu-id="de04e-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-145">Contacts.Read</span></span> |
| [<span data-ttu-id="de04e-146">event</span><span class="sxs-lookup"><span data-stu-id="de04e-146">event</span></span>](../resources/event.md) | <span data-ttu-id="de04e-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-147">Calendars.Read</span></span> | <span data-ttu-id="de04e-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-148">Calendars.Read</span></span> |  <span data-ttu-id="de04e-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-149">Calendars.Read</span></span>|
| <span data-ttu-id="de04e-150">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="de04e-150">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="de04e-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="de04e-151">Group.Read.All</span></span> | <span data-ttu-id="de04e-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de04e-152">Not supported</span></span> | <span data-ttu-id="de04e-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de04e-153">Not supported</span></span> |
| <span data-ttu-id="de04e-154">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="de04e-154">group [event](../resources/event.md)</span></span> | <span data-ttu-id="de04e-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="de04e-155">Group.Read.All</span></span> | <span data-ttu-id="de04e-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de04e-156">Not supported</span></span> | <span data-ttu-id="de04e-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de04e-157">Not supported</span></span> |
| <span data-ttu-id="de04e-158">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="de04e-158">group [post](../resources/post.md)</span></span> | <span data-ttu-id="de04e-159">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="de04e-159">Group.Read.All</span></span> | <span data-ttu-id="de04e-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de04e-160">Not supported</span></span> | <span data-ttu-id="de04e-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="de04e-161">Group.Read.All</span></span> |
| [<span data-ttu-id="de04e-162">mailFolder</span><span class="sxs-lookup"><span data-stu-id="de04e-162">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="de04e-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-163">Mail.Read</span></span> | <span data-ttu-id="de04e-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-164">Mail.Read</span></span> | <span data-ttu-id="de04e-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-165">Mail.Read</span></span> |
| [<span data-ttu-id="de04e-166">message</span><span class="sxs-lookup"><span data-stu-id="de04e-166">message</span></span>](../resources/message.md) | <span data-ttu-id="de04e-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-167">Mail.Read</span></span> | <span data-ttu-id="de04e-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-168">Mail.Read</span></span> | <span data-ttu-id="de04e-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-169">Mail.Read</span></span> |
| [<span data-ttu-id="de04e-170">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="de04e-170">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="de04e-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-171">Tasks.Read</span></span> | <span data-ttu-id="de04e-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-172">Tasks.Read</span></span> | <span data-ttu-id="de04e-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de04e-173">Not supported</span></span> |
| [<span data-ttu-id="de04e-174">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="de04e-174">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="de04e-175">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-175">Tasks.Read</span></span> | <span data-ttu-id="de04e-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="de04e-176">Tasks.Read</span></span> | <span data-ttu-id="de04e-177">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de04e-177">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="de04e-178">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de04e-178">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="de04e-179">Получение экземпляра ресурса, дополненного расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="de04e-179">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="de04e-p105">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="de04e-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="de04e-182">Получение экземпляра **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-182">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="de04e-183">Получение экземпляра **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-183">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="de04e-184">Получение экземпляра **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-184">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="de04e-185">Получение экземпляра **календаря** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-185">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="de04e-186">Получение экземпляра **контактов** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-186">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="de04e-187">Получение экземпляра **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-187">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="de04e-188">Получение экземпляра **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-188">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="de04e-189">Получение экземпляра **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-189">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="de04e-190">Получение экземпляра **события** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-190">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="de04e-191">Получение экземпляра **публиковать** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-191">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="de04e-192">Получение экземпляров ресурсов с числовыми расширенными свойствами, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="de04e-192">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="de04e-193">Получите экземпляры поддерживаемого ресурса с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="de04e-193">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="de04e-194">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="de04e-194">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="de04e-195">Убедитесь, что применение сделать что применения [Кодировка URL-адрес](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра - двоеточие, косая черта и пространства.</span><span class="sxs-lookup"><span data-stu-id="de04e-195">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="de04e-196">В приведенных ниже строках синтаксиса показан фильтр, в случае которого один оператор `eq` используется для свойства id, а другой оператор `eq` — для свойства value.</span><span class="sxs-lookup"><span data-stu-id="de04e-196">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="de04e-197">Вы можете заменить оператор `eq` для свойства **value** любым из других операторов (`ne`, `ge`, `gt`, `le` или `lt`), которые применяются к числовым значениям.</span><span class="sxs-lookup"><span data-stu-id="de04e-197">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="de04e-198">Получение экземпляров **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-198">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="de04e-199">Получение экземпляров **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-199">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="de04e-200">Получение экземпляров **события** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-200">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="de04e-201">Получение экземпляров **календаря** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-201">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="de04e-202">Получение экземпляров **контактов** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-202">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="de04e-203">Получение экземпляров **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-203">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="de04e-204">Получение экземпляра **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-204">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="de04e-205">Получение экземпляра **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-205">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="de04e-206">Получение экземпляров группы **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-206">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="de04e-207">Получение экземпляров **публикации** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-207">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="de04e-208">Получение экземпляров ресурсов с расширенными свойствами строкового типа, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="de04e-208">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="de04e-209">Получите экземпляры ресурса **message** или **event**, которые включают расширенное свойство строкового типа, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="de04e-209">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="de04e-210">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `contains`, `startswith`, `eq` или `ne`.</span><span class="sxs-lookup"><span data-stu-id="de04e-210">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="de04e-211">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="de04e-211">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="de04e-212">Получение экземпляров **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-212">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="de04e-213">Получение экземпляров **события** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-213">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="de04e-214">Получение экземпляров группы **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="de04e-214">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="de04e-215">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="de04e-215">Path parameters</span></span>
|<span data-ttu-id="de04e-216">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="de04e-216">**Parameter**</span></span>|<span data-ttu-id="de04e-217">**Тип**</span><span class="sxs-lookup"><span data-stu-id="de04e-217">**Type**</span></span>|<span data-ttu-id="de04e-218">**Описание**</span><span class="sxs-lookup"><span data-stu-id="de04e-218">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="de04e-219">id_value</span><span class="sxs-lookup"><span data-stu-id="de04e-219">id_value</span></span>|<span data-ttu-id="de04e-220">String</span><span class="sxs-lookup"><span data-stu-id="de04e-220">String</span></span>|<span data-ttu-id="de04e-p109">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de04e-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="de04e-225">property_value</span><span class="sxs-lookup"><span data-stu-id="de04e-225">property_value</span></span> |<span data-ttu-id="de04e-226">String</span><span class="sxs-lookup"><span data-stu-id="de04e-226">String</span></span>|<span data-ttu-id="de04e-227">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="de04e-227">The value of the extended property to match.</span></span> <span data-ttu-id="de04e-228">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="de04e-228">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="de04e-229">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="de04e-229">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="de04e-230">Примеры см. в разделе [Запрос 4](#request-4).</span><span class="sxs-lookup"><span data-stu-id="de04e-230">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="de04e-231">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de04e-231">Request headers</span></span>
| <span data-ttu-id="de04e-232">Имя</span><span class="sxs-lookup"><span data-stu-id="de04e-232">Name</span></span>      |<span data-ttu-id="de04e-233">Описание</span><span class="sxs-lookup"><span data-stu-id="de04e-233">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="de04e-234">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de04e-234">Authorization</span></span>  | <span data-ttu-id="de04e-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de04e-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de04e-237">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de04e-237">Request body</span></span>
<span data-ttu-id="de04e-238">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de04e-238">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de04e-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="de04e-239">Response</span></span>

<span data-ttu-id="de04e-240">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="de04e-240">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="de04e-241">Запрос GET на получение экземпляра ресурса с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="de04e-241">GET resource instance using `$expand`</span></span>
<span data-ttu-id="de04e-242">Тело отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="de04e-242">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="de04e-243">Получение экземпляров ресурсов с расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="de04e-243">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="de04e-244">Тело отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="de04e-244">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="de04e-245">Тело отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="de04e-245">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="de04e-246">Пример</span><span class="sxs-lookup"><span data-stu-id="de04e-246">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="de04e-247">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="de04e-247">Request 1</span></span>

<span data-ttu-id="de04e-p113">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="de04e-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="de04e-250">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="de04e-250">Response 1</span></span>
<span data-ttu-id="de04e-251">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="de04e-251">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="de04e-p114">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de04e-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="de04e-254">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="de04e-254">Request 2</span></span>

<span data-ttu-id="de04e-255">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="de04e-255">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="de04e-256">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="de04e-256">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="de04e-257">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="de04e-257">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="de04e-258">его свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="de04e-258">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="de04e-259">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="de04e-259">Response 2</span></span>

<span data-ttu-id="de04e-p116">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user-list-messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="de04e-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="de04e-263">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="de04e-263">Request 3</span></span>

<span data-ttu-id="de04e-264">В третьем примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством строкового типа.</span><span class="sxs-lookup"><span data-stu-id="de04e-264">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="de04e-265">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="de04e-265">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="de04e-266">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="de04e-266">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="de04e-267">его свойство **value** включает строку `green`.</span><span class="sxs-lookup"><span data-stu-id="de04e-267">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="de04e-268">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="de04e-268">Response 3</span></span>

<span data-ttu-id="de04e-269">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а тело отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="de04e-269">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="de04e-270">Например, сообщение, которое содержит однозначное расширенное свойство со свойством **id**, равным строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, и свойством **value**, равным строке `Light green`, будет соответствовать фильтру и включено в отклик.</span><span class="sxs-lookup"><span data-stu-id="de04e-270">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="de04e-271">Тело отклика такое же, как при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="de04e-271">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="de04e-272">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="de04e-272">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="de04e-273">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="de04e-273">Request 4</span></span>

<span data-ttu-id="de04e-274">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от строкового.</span><span class="sxs-lookup"><span data-stu-id="de04e-274">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="de04e-275">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="de04e-275">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="de04e-276">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="de04e-276">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="de04e-277">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="de04e-277">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="de04e-278">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="de04e-278">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="de04e-279">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="de04e-279">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="de04e-280">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="de04e-280">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="de04e-281">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="de04e-281">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="de04e-282">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="de04e-282">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="de04e-283">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="de04e-283">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="de04e-284">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="de04e-284">Response 4</span></span>

<span data-ttu-id="de04e-285">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="de04e-285">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="de04e-286">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="de04e-286">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="de04e-287">Ответ не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="de04e-287">The response does not include the matching extended property.</span></span>


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
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
