---
title: Получение объекта singleValueLegacyExtendedProperty
description: Можно получить экземпляр единственный ресурс, включающим определенное свойство расширенного или коллекцию экземпляров ресурсов
ms.openlocfilehash: 72ae071d2c5c92af02d26af2474c776a5dc1c83c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081280"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="8f9f7-103">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8f9f7-103">Get singleValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="8f9f7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f9f7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f9f7-106">Вы можете получить отдельный экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурсов, включающую расширенные свойства, которые соответствуют фильтру.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-106">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="8f9f7-107">Параметр запроса `$expand` позволяет получить указанный экземпляр ресурса, дополненный определенным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-107">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="8f9f7-108">Используйте операторы `$filter` и `eq` в свойстве **id**, чтобы указать расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-108">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="8f9f7-109">На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-109">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="8f9f7-110">Чтобы получить экземпляры ресурсов, которые содержат определенные расширенные свойства, используйте параметр запроса `$filter` и примените оператор `eq` к свойству **id**.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-110">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="8f9f7-111">Кроме того, для числовых расширенных свойств примените один из следующих операторов к свойству **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-111">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="8f9f7-112">Для расширенных свойств строкового типа примените оператор `contains`, `startswith`, `eq` или `ne` к свойству **value**.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-112">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="8f9f7-113">При фильтрации имени строки (`Name`) в свойстве **id** расширенного свойства учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-113">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="8f9f7-114">При фильтрации свойства **value** расширенного свойства регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-114">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="8f9f7-115">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="8f9f7-115">The following user resources are supported:</span></span>

- <span data-ttu-id="8f9f7-116">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="8f9f7-116">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="8f9f7-117">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="8f9f7-117">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="8f9f7-118">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-118">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="8f9f7-119">событие</span><span class="sxs-lookup"><span data-stu-id="8f9f7-119">event</span></span>](../resources/event.md)
- [<span data-ttu-id="8f9f7-120">mailFolder</span><span class="sxs-lookup"><span data-stu-id="8f9f7-120">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="8f9f7-121">message</span><span class="sxs-lookup"><span data-stu-id="8f9f7-121">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="8f9f7-122">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="8f9f7-122">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="8f9f7-123">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="8f9f7-123">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="8f9f7-124">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="8f9f7-124">As well as the following group resources:</span></span>

- <span data-ttu-id="8f9f7-125">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="8f9f7-125">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="8f9f7-126">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="8f9f7-126">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="8f9f7-127">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-127">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="8f9f7-128">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-128">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f9f7-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f9f7-129">Permissions</span></span>
<span data-ttu-id="8f9f7-130">В зависимости от ресурса они будут расширенные свойства из и разрешение введите (делегированные или приложения) вы запроса, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-130">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="8f9f7-131">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-131">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f9f7-132">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="8f9f7-132">Supported resource</span></span> | <span data-ttu-id="8f9f7-133">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f9f7-133">Delegated (work or school account)</span></span> | <span data-ttu-id="8f9f7-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f9f7-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f9f7-135">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8f9f7-135">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="8f9f7-136">calendar</span><span class="sxs-lookup"><span data-stu-id="8f9f7-136">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="8f9f7-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-137">Calendars.Read</span></span> | <span data-ttu-id="8f9f7-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-138">Calendars.Read</span></span> | <span data-ttu-id="8f9f7-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-139">Calendars.Read</span></span> |
| [<span data-ttu-id="8f9f7-140">контакт</span><span class="sxs-lookup"><span data-stu-id="8f9f7-140">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8f9f7-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-141">Contacts.Read</span></span> | <span data-ttu-id="8f9f7-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-142">Contacts.Read</span></span> | <span data-ttu-id="8f9f7-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-143">Contacts.Read</span></span> |
| <span data-ttu-id="8f9f7-144">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-144">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="8f9f7-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-145">Contacts.Read</span></span> | <span data-ttu-id="8f9f7-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-146">Contacts.Read</span></span> | <span data-ttu-id="8f9f7-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-147">Contacts.Read</span></span> |
| [<span data-ttu-id="8f9f7-148">событие</span><span class="sxs-lookup"><span data-stu-id="8f9f7-148">event</span></span>](../resources/event.md) | <span data-ttu-id="8f9f7-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-149">Calendars.Read</span></span> | <span data-ttu-id="8f9f7-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-150">Calendars.Read</span></span> |  <span data-ttu-id="8f9f7-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-151">Calendars.Read</span></span>|
| <span data-ttu-id="8f9f7-152">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="8f9f7-152">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="8f9f7-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f9f7-153">Group.Read.All</span></span> | <span data-ttu-id="8f9f7-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f9f7-154">Not supported</span></span> | <span data-ttu-id="8f9f7-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f9f7-155">Not supported</span></span> |
| <span data-ttu-id="8f9f7-156">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="8f9f7-156">group [event](../resources/event.md)</span></span> | <span data-ttu-id="8f9f7-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f9f7-157">Group.Read.All</span></span> | <span data-ttu-id="8f9f7-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f9f7-158">Not supported</span></span> | <span data-ttu-id="8f9f7-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f9f7-159">Not supported</span></span> |
| <span data-ttu-id="8f9f7-160">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-160">group [post](../resources/post.md)</span></span> | <span data-ttu-id="8f9f7-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f9f7-161">Group.Read.All</span></span> | <span data-ttu-id="8f9f7-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f9f7-162">Not supported</span></span> | <span data-ttu-id="8f9f7-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f9f7-163">Group.Read.All</span></span> |
| [<span data-ttu-id="8f9f7-164">mailFolder</span><span class="sxs-lookup"><span data-stu-id="8f9f7-164">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="8f9f7-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-165">Mail.Read</span></span> | <span data-ttu-id="8f9f7-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-166">Mail.Read</span></span> | <span data-ttu-id="8f9f7-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-167">Mail.Read</span></span> |
| [<span data-ttu-id="8f9f7-168">message</span><span class="sxs-lookup"><span data-stu-id="8f9f7-168">message</span></span>](../resources/message.md) | <span data-ttu-id="8f9f7-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-169">Mail.Read</span></span> | <span data-ttu-id="8f9f7-170">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-170">Mail.Read</span></span> | <span data-ttu-id="8f9f7-171">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-171">Mail.Read</span></span> |
| [<span data-ttu-id="8f9f7-172">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="8f9f7-172">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="8f9f7-173">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-173">Tasks.Read</span></span> | <span data-ttu-id="8f9f7-174">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-174">Tasks.Read</span></span> | <span data-ttu-id="8f9f7-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f9f7-175">Not supported</span></span> |
| [<span data-ttu-id="8f9f7-176">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="8f9f7-176">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="8f9f7-177">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-177">Tasks.Read</span></span> | <span data-ttu-id="8f9f7-178">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8f9f7-178">Tasks.Read</span></span> | <span data-ttu-id="8f9f7-179">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f9f7-179">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="8f9f7-180">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f9f7-180">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="8f9f7-181">Получение экземпляра ресурса, дополненного расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="8f9f7-181">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="8f9f7-p106">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-p106">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="8f9f7-184">Получение экземпляра **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-184">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f9f7-185">Получение экземпляра **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-185">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="8f9f7-186">Получение экземпляра **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-186">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f9f7-187">Получение экземпляра **календаря** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-187">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="8f9f7-188">Получение экземпляра **контактов** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-188">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f9f7-189">Получение экземпляра **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-189">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="8f9f7-190">Получение экземпляра **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-190">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="8f9f7-191">Получение экземпляра **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-191">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="8f9f7-192">Получение экземпляра **события** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-192">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="8f9f7-193">Получение экземпляра **публиковать** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-193">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="8f9f7-194">Получение экземпляров ресурсов с числовыми расширенными свойствами, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="8f9f7-194">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="8f9f7-195">Получите экземпляры поддерживаемого ресурса с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-195">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="8f9f7-196">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-196">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="8f9f7-197">Убедитесь, что применение сделать что применения [Кодировка URL-адрес](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра - двоеточие, косая черта и пространства.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-197">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="8f9f7-198">В приведенных ниже строках синтаксиса показан фильтр, в случае которого один оператор `eq` используется для свойства id, а другой оператор `eq` — для свойства value.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-198">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="8f9f7-199">Вы можете заменить оператор `eq` для свойства **value** любым из других операторов (`ne`, `ge`, `gt`, `le` или `lt`), которые применяются к числовым значениям.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-199">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="8f9f7-200">Получение экземпляров **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-200">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f9f7-201">Получение экземпляров **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-201">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="8f9f7-202">Получение экземпляров **события** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-202">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f9f7-203">Получение экземпляров **календаря** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-203">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f9f7-204">Получение экземпляров **контактов** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-204">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f9f7-205">Получение экземпляров **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-205">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="8f9f7-206">Получение экземпляра **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-206">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="8f9f7-207">Получение экземпляра **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-207">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="8f9f7-208">Получение экземпляров группы **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-208">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="8f9f7-209">Получение экземпляров **публикации** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-209">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="8f9f7-210">Получение экземпляров ресурсов с расширенными свойствами строкового типа, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="8f9f7-210">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="8f9f7-211">Получите экземпляры ресурса **message** или **event**, которые включают расширенное свойство строкового типа, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-211">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="8f9f7-212">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `contains`, `startswith`, `eq` или `ne`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-212">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="8f9f7-213">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-213">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="8f9f7-214">Получение экземпляров **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-214">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="8f9f7-215">Получение экземпляров **события** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-215">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="8f9f7-216">Получение экземпляров группы **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8f9f7-216">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="8f9f7-217">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="8f9f7-217">Path parameters</span></span>
|<span data-ttu-id="8f9f7-218">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="8f9f7-218">**Parameter**</span></span>|<span data-ttu-id="8f9f7-219">**Тип**</span><span class="sxs-lookup"><span data-stu-id="8f9f7-219">**Type**</span></span>|<span data-ttu-id="8f9f7-220">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8f9f7-220">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8f9f7-221">id_value</span><span class="sxs-lookup"><span data-stu-id="8f9f7-221">id_value</span></span>|<span data-ttu-id="8f9f7-222">String</span><span class="sxs-lookup"><span data-stu-id="8f9f7-222">String</span></span>|<span data-ttu-id="8f9f7-p110">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-p110">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="8f9f7-227">property_value</span><span class="sxs-lookup"><span data-stu-id="8f9f7-227">property_value</span></span> |<span data-ttu-id="8f9f7-228">String</span><span class="sxs-lookup"><span data-stu-id="8f9f7-228">String</span></span>|<span data-ttu-id="8f9f7-229">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-229">The value of the extended property to match.</span></span> <span data-ttu-id="8f9f7-230">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-230">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="8f9f7-231">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-231">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="8f9f7-232">Примеры см. в разделе [Запрос 4](#request-4).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-232">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8f9f7-233">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f9f7-233">Request headers</span></span>
| <span data-ttu-id="8f9f7-234">Имя</span><span class="sxs-lookup"><span data-stu-id="8f9f7-234">Name</span></span>      |<span data-ttu-id="8f9f7-235">Описание</span><span class="sxs-lookup"><span data-stu-id="8f9f7-235">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f9f7-236">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f9f7-236">Authorization</span></span>  | <span data-ttu-id="8f9f7-p112">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f9f7-239">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f9f7-239">Request body</span></span>
<span data-ttu-id="8f9f7-240">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-240">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f9f7-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f9f7-241">Response</span></span>

<span data-ttu-id="8f9f7-242">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-242">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="8f9f7-243">Запрос GET на получение экземпляра ресурса с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="8f9f7-243">GET resource instance using `$expand`</span></span>
<span data-ttu-id="8f9f7-244">Тело отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-244">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="8f9f7-245">Получение экземпляров ресурсов с расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="8f9f7-245">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="8f9f7-246">Тело отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-246">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="8f9f7-247">Тело отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-247">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="8f9f7-248">Пример</span><span class="sxs-lookup"><span data-stu-id="8f9f7-248">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="8f9f7-249">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="8f9f7-249">Request 1</span></span>

<span data-ttu-id="8f9f7-p114">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-p114">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="8f9f7-252">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="8f9f7-252">Response 1</span></span>
<span data-ttu-id="8f9f7-253">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-253">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="8f9f7-p115">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-p115">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="8f9f7-256">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="8f9f7-256">Request 2</span></span>

<span data-ttu-id="8f9f7-257">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-257">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="8f9f7-258">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="8f9f7-258">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="8f9f7-259">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="8f9f7-259">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="8f9f7-260">его свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-260">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="8f9f7-261">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="8f9f7-261">Response 2</span></span>

<span data-ttu-id="8f9f7-p117">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user-list-messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-p117">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="8f9f7-265">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="8f9f7-265">Request 3</span></span>

<span data-ttu-id="8f9f7-266">В третьем примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством строкового типа.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-266">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="8f9f7-267">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="8f9f7-267">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="8f9f7-268">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="8f9f7-268">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="8f9f7-269">его свойство **value** включает строку `green`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-269">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="8f9f7-270">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="8f9f7-270">Response 3</span></span>

<span data-ttu-id="8f9f7-271">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а тело отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-271">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="8f9f7-272">Например, сообщение, которое содержит однозначное расширенное свойство со свойством **id**, равным строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, и свойством **value**, равным строке `Light green`, будет соответствовать фильтру и включено в отклик.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-272">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="8f9f7-273">Тело отклика такое же, как при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-273">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="8f9f7-274">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-274">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="8f9f7-275">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="8f9f7-275">Request 4</span></span>

<span data-ttu-id="8f9f7-276">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от строкового.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-276">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="8f9f7-277">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-277">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="8f9f7-278">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="8f9f7-278">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="8f9f7-279">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-279">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="8f9f7-280">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-280">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="8f9f7-281">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-281">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="8f9f7-282">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="8f9f7-282">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="8f9f7-283">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-283">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="8f9f7-284">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-284">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="8f9f7-285">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-285">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="8f9f7-286">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="8f9f7-286">Response 4</span></span>

<span data-ttu-id="8f9f7-287">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-287">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="8f9f7-288">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="8f9f7-288">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="8f9f7-289">Ответ не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="8f9f7-289">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->