---
title: Создание многозначного расширенного свойства
description: 'Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса. '
ms.openlocfilehash: 17f1bf0a4dd03de3704349fcfd496b768f60d56f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079062"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="03028-103">Создание многозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="03028-103">Create multi-value extended property</span></span>

> <span data-ttu-id="03028-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03028-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03028-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03028-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03028-106">Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="03028-106">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="03028-107">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="03028-107">The following user resources are supported:</span></span>

- <span data-ttu-id="03028-108">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="03028-108">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="03028-109">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="03028-109">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="03028-110">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="03028-110">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="03028-111">событие</span><span class="sxs-lookup"><span data-stu-id="03028-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="03028-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="03028-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="03028-113">message</span><span class="sxs-lookup"><span data-stu-id="03028-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="03028-114">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="03028-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="03028-115">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="03028-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="03028-116">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="03028-116">As well as the following group resources:</span></span>

- <span data-ttu-id="03028-117">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="03028-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="03028-118">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="03028-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="03028-119">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="03028-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="03028-120">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="03028-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="03028-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03028-121">Permissions</span></span>
<span data-ttu-id="03028-122">В зависимости от ресурса при создании расширенные свойства в и введите (делегированные или приложения) вы запроса на разрешение, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="03028-122">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="03028-123">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03028-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03028-124">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="03028-124">Supported resource</span></span> | <span data-ttu-id="03028-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03028-125">Delegated (work or school account)</span></span> | <span data-ttu-id="03028-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03028-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03028-127">Для приложения</span><span class="sxs-lookup"><span data-stu-id="03028-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="03028-128">calendar</span><span class="sxs-lookup"><span data-stu-id="03028-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="03028-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="03028-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-130">Calendars.ReadWrite</span></span> | <span data-ttu-id="03028-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-131">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="03028-132">контакт</span><span class="sxs-lookup"><span data-stu-id="03028-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="03028-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="03028-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="03028-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-135">Contacts.ReadWrite</span></span> |
| <span data-ttu-id="03028-136">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="03028-136">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="03028-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="03028-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-138">Contacts.ReadWrite</span></span> | <span data-ttu-id="03028-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-139">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="03028-140">event</span><span class="sxs-lookup"><span data-stu-id="03028-140">event</span></span>](../resources/event.md) | <span data-ttu-id="03028-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-141">Calendars.ReadWrite</span></span> | <span data-ttu-id="03028-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-142">Calendars.ReadWrite</span></span> |  <span data-ttu-id="03028-143">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-143">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="03028-144">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="03028-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="03028-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03028-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="03028-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-146">Not supported</span></span> | <span data-ttu-id="03028-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-147">Not supported</span></span> |
| <span data-ttu-id="03028-148">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="03028-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="03028-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03028-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="03028-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-150">Not supported</span></span> | <span data-ttu-id="03028-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-151">Not supported</span></span> |
| <span data-ttu-id="03028-152">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="03028-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="03028-153">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03028-153">Group.ReadWrite.All</span></span> | <span data-ttu-id="03028-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-154">Not supported</span></span> | <span data-ttu-id="03028-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-155">Not supported</span></span> |
| [<span data-ttu-id="03028-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="03028-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="03028-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-157">Mail.ReadWrite</span></span> | <span data-ttu-id="03028-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-158">Mail.ReadWrite</span></span> | <span data-ttu-id="03028-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-159">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="03028-160">message</span><span class="sxs-lookup"><span data-stu-id="03028-160">message</span></span>](../resources/message.md) | <span data-ttu-id="03028-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-161">Mail.ReadWrite</span></span> | <span data-ttu-id="03028-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-162">Mail.ReadWrite</span></span> | <span data-ttu-id="03028-163">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-163">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="03028-164">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="03028-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="03028-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="03028-166">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-166">Tasks.ReadWrite</span></span> | <span data-ttu-id="03028-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-167">Not supported</span></span> |
| [<span data-ttu-id="03028-168">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="03028-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="03028-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="03028-170">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03028-170">Tasks.ReadWrite</span></span> | <span data-ttu-id="03028-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="03028-171">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="03028-172">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03028-172">HTTP request</span></span>
<span data-ttu-id="03028-173">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="03028-173">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="03028-174">Создайте один или несколько расширенных свойств в _новый_ экземпляр ресурсов, использование того же запроса REST создания экземпляра и включить свойства нового ресурса экземпляра _и расширенные свойства_ в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="03028-174">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="03028-175">Обратите внимание, что некоторые ресурсы поддержки в несколько способов создания.</span><span class="sxs-lookup"><span data-stu-id="03028-175">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="03028-176">Дополнительные сведения о создании этих экземплярах ресурсов см в соответствующие разделы для создания [сообщения](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [события](../api/user-post-events.md), [календаря](../api/user-post-calendars.md), [контактов](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md) [задач Outlook](../resources/outlooktask.md), [ Папки задач Outlook](../resources/outlooktaskfolder.md), [событие группы](../api/group-post-events.md)и [группы post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="03028-176">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="03028-177">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="03028-177">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
POST /me/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks

POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="03028-178">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="03028-178">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="03028-179">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="03028-179">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /me/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

PATCH /me/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03028-180">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03028-180">Request headers</span></span>
| <span data-ttu-id="03028-181">Имя</span><span class="sxs-lookup"><span data-stu-id="03028-181">Name</span></span>       | <span data-ttu-id="03028-182">Значение</span><span class="sxs-lookup"><span data-stu-id="03028-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="03028-183">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03028-183">Authorization</span></span> | <span data-ttu-id="03028-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03028-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03028-186">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03028-186">Content-Type</span></span> | <span data-ttu-id="03028-187">application/json</span><span class="sxs-lookup"><span data-stu-id="03028-187">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="03028-188">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03028-188">Request body</span></span>

<span data-ttu-id="03028-189">Предоставьте тело в формате JSON для каждого объекта [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) в свойстве коллекции **multiValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="03028-189">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="03028-190">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="03028-190">**Property**</span></span>|<span data-ttu-id="03028-191">**Тип**</span><span class="sxs-lookup"><span data-stu-id="03028-191">**Type**</span></span>|<span data-ttu-id="03028-192">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03028-192">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="03028-193">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="03028-193">multiValueExtendedProperties</span></span>|<span data-ttu-id="03028-194">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="03028-194">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="03028-195">Массив из одного или нескольких многозначных расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="03028-195">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="03028-196">id</span><span class="sxs-lookup"><span data-stu-id="03028-196">id</span></span>|<span data-ttu-id="03028-197">Строка</span><span class="sxs-lookup"><span data-stu-id="03028-197">String</span></span>|<span data-ttu-id="03028-p105">Чтобы идентифицировать свойства в коллекции **multiValueExtendedProperties**, укажите этот параметр для каждого из них. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="03028-p105">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="03028-202">значение</span><span class="sxs-lookup"><span data-stu-id="03028-202">value</span></span>|<span data-ttu-id="03028-203">строка</span><span class="sxs-lookup"><span data-stu-id="03028-203">string</span></span>|<span data-ttu-id="03028-p106">Укажите значение для каждого свойства в коллекции **multiValueExtendedProperties**. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="03028-p106">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="03028-206">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **multiValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03028-206">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="03028-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="03028-207">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="03028-208">Код отклика</span><span class="sxs-lookup"><span data-stu-id="03028-208">Response code</span></span>
<span data-ttu-id="03028-209">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="03028-209">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="03028-210">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="03028-210">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="03028-211">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="03028-211">Response body</span></span>

<span data-ttu-id="03028-p107">При создании расширенного свойства в поддерживаемом ресурсе, отличном от [post для групп](../resources/post.md), отклик включает только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы просмотреть только что созданное расширенное свойство, [разверните экземпляр с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="03028-p107">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="03028-p108">При создании расширенного свойства в _новом_ экземпляре post для групп отклик включает только код отклика и не содержит ни новой записи, ни расширенного свойства. Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="03028-p108">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="03028-216">Пример</span><span class="sxs-lookup"><span data-stu-id="03028-216">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="03028-217">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="03028-217">Request 1</span></span>

<span data-ttu-id="03028-p109">В первом примере в новом экземпляре event создается многозначное расширенное свойство с помощью одной операции POST. Помимо свойств, которые обычно указываются для нового события, тело запроса включает коллекцию **multiValueExtendedProperties**, которая содержит одно расширенное свойство. Тело запроса включает следующие данные для многозначного расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="03028-p109">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="03028-221">**id**. Задает свойство в виде массива строк с заданным идентификатором GUID и именем `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="03028-221">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="03028-222">**value**. Задает `Recreation` в виде массива из 3 строковых значений, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="03028-222">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="03028-223">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="03028-223">Response 1</span></span>

<span data-ttu-id="03028-p110">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="03028-p110">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="03028-226">Чтобы просмотреть новое расширенное свойство, [разверните event с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="03028-226">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="03028-227">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="03028-227">Request 2</span></span>

<span data-ttu-id="03028-p111">Во втором примере создается многозначное расширенное свойство для указанного сообщения. Это расширенное свойство — единственный элемент в коллекции **multiValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="03028-p111">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="03028-231">**id**. Задает свойство в виде массива строк с указанным идентификатором GUID и именем `Palette`.</span><span class="sxs-lookup"><span data-stu-id="03028-231">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="03028-232">**value**. Задает `Palette` в виде массива 3 строковых значений, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="03028-232">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="03028-233">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="03028-233">Response 2</span></span>

<span data-ttu-id="03028-p112">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="03028-p112">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="03028-236">Чтобы просмотреть новое расширенное свойство, [разверните message с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="03028-236">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->




