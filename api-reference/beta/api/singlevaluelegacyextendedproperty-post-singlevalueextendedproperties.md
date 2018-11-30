---
title: Создание расширенного свойства с одним значением
description: 'Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса. '
ms.openlocfilehash: c55ab01ecde214feb38857e8d77f83eb3bfbabc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076775"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="12b7e-103">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="12b7e-103">Create single-value extended property</span></span>

> <span data-ttu-id="12b7e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12b7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12b7e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12b7e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12b7e-106">Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="12b7e-106">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="12b7e-107">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="12b7e-107">The following user resources are supported:</span></span>

- <span data-ttu-id="12b7e-108">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="12b7e-108">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="12b7e-109">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="12b7e-109">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="12b7e-110">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="12b7e-110">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="12b7e-111">событие</span><span class="sxs-lookup"><span data-stu-id="12b7e-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="12b7e-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="12b7e-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="12b7e-113">message</span><span class="sxs-lookup"><span data-stu-id="12b7e-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="12b7e-114">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="12b7e-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="12b7e-115">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="12b7e-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="12b7e-116">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="12b7e-116">As well as the following group resources:</span></span>

- <span data-ttu-id="12b7e-117">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="12b7e-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="12b7e-118">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="12b7e-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="12b7e-119">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="12b7e-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="12b7e-120">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="12b7e-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="12b7e-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12b7e-121">Permissions</span></span>
<span data-ttu-id="12b7e-122">В зависимости от ресурса при создании расширенные свойства в и введите (делегированные или приложения) вы запроса на разрешение, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="12b7e-122">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="12b7e-123">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12b7e-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12b7e-124">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="12b7e-124">Supported resource</span></span> | <span data-ttu-id="12b7e-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12b7e-125">Delegated (work or school account)</span></span> | <span data-ttu-id="12b7e-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12b7e-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12b7e-127">Для приложения</span><span class="sxs-lookup"><span data-stu-id="12b7e-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="12b7e-128">calendar</span><span class="sxs-lookup"><span data-stu-id="12b7e-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="12b7e-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="12b7e-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-130">Calendars.ReadWrite</span></span> | <span data-ttu-id="12b7e-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-131">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="12b7e-132">контакт</span><span class="sxs-lookup"><span data-stu-id="12b7e-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="12b7e-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b7e-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b7e-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-135">Contacts.ReadWrite</span></span> |
| <span data-ttu-id="12b7e-136">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="12b7e-136">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="12b7e-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b7e-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-138">Contacts.ReadWrite</span></span> | <span data-ttu-id="12b7e-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-139">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="12b7e-140">event</span><span class="sxs-lookup"><span data-stu-id="12b7e-140">event</span></span>](../resources/event.md) | <span data-ttu-id="12b7e-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-141">Calendars.ReadWrite</span></span> | <span data-ttu-id="12b7e-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-142">Calendars.ReadWrite</span></span> |  <span data-ttu-id="12b7e-143">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-143">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="12b7e-144">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="12b7e-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="12b7e-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b7e-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="12b7e-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-146">Not supported</span></span> | <span data-ttu-id="12b7e-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-147">Not supported</span></span> |
| <span data-ttu-id="12b7e-148">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="12b7e-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="12b7e-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b7e-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="12b7e-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-150">Not supported</span></span> | <span data-ttu-id="12b7e-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-151">Not supported</span></span> |
| <span data-ttu-id="12b7e-152">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="12b7e-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="12b7e-153">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b7e-153">Group.ReadWrite.All</span></span> | <span data-ttu-id="12b7e-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-154">Not supported</span></span> | <span data-ttu-id="12b7e-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-155">Not supported</span></span> |
| [<span data-ttu-id="12b7e-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="12b7e-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="12b7e-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-157">Mail.ReadWrite</span></span> | <span data-ttu-id="12b7e-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-158">Mail.ReadWrite</span></span> | <span data-ttu-id="12b7e-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-159">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="12b7e-160">message</span><span class="sxs-lookup"><span data-stu-id="12b7e-160">message</span></span>](../resources/message.md) | <span data-ttu-id="12b7e-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-161">Mail.ReadWrite</span></span> | <span data-ttu-id="12b7e-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-162">Mail.ReadWrite</span></span> | <span data-ttu-id="12b7e-163">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-163">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="12b7e-164">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="12b7e-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="12b7e-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b7e-166">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-166">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b7e-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-167">Not supported</span></span> |
| [<span data-ttu-id="12b7e-168">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="12b7e-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="12b7e-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b7e-170">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12b7e-170">Tasks.ReadWrite</span></span> | <span data-ttu-id="12b7e-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12b7e-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="12b7e-172">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12b7e-172">HTTP request</span></span>
<span data-ttu-id="12b7e-173">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="12b7e-173">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="12b7e-174">Создайте один или несколько расширенных свойств в _новый_ экземпляр ресурсов, использование того же запроса REST создания экземпляра и включить свойства нового ресурса экземпляра _и расширенные свойства_ в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="12b7e-174">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="12b7e-175">Обратите внимание, что некоторые ресурсы поддержки в несколько способов создания.</span><span class="sxs-lookup"><span data-stu-id="12b7e-175">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="12b7e-176">Дополнительные сведения о создании этих экземплярах ресурсов см в соответствующие разделы для создания [сообщения](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [события](../api/user-post-events.md), [календаря](../api/user-post-calendars.md), [контактов](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md) [задач Outlook](../resources/outlooktask.md), [ Папки задач Outlook](../resources/outlooktaskfolder.md), [событие группы](../api/group-post-events.md)и [группы post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="12b7e-176">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="12b7e-177">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="12b7e-177">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="12b7e-178">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="12b7e-178">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="12b7e-179">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="12b7e-179">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="12b7e-180">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12b7e-180">Request headers</span></span>
| <span data-ttu-id="12b7e-181">Имя</span><span class="sxs-lookup"><span data-stu-id="12b7e-181">Name</span></span>       | <span data-ttu-id="12b7e-182">Значение</span><span class="sxs-lookup"><span data-stu-id="12b7e-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="12b7e-183">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12b7e-183">Authorization</span></span> | <span data-ttu-id="12b7e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12b7e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12b7e-186">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12b7e-186">Content-Type</span></span> | <span data-ttu-id="12b7e-187">application/json</span><span class="sxs-lookup"><span data-stu-id="12b7e-187">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="12b7e-188">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12b7e-188">Request body</span></span>

<span data-ttu-id="12b7e-189">Предоставьте тело JSON каждого объекта [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) в свойстве коллекции **singleValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="12b7e-189">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="12b7e-190">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="12b7e-190">**Property**</span></span>|<span data-ttu-id="12b7e-191">**Тип**</span><span class="sxs-lookup"><span data-stu-id="12b7e-191">**Type**</span></span>|<span data-ttu-id="12b7e-192">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12b7e-192">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="12b7e-193">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="12b7e-193">singleValueExtendedProperties</span></span>|<span data-ttu-id="12b7e-194">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="12b7e-194">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="12b7e-195">Массив из одного или нескольких расширенных свойств с одним значением.</span><span class="sxs-lookup"><span data-stu-id="12b7e-195">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="12b7e-196">id</span><span class="sxs-lookup"><span data-stu-id="12b7e-196">id</span></span>|<span data-ttu-id="12b7e-197">Строка</span><span class="sxs-lookup"><span data-stu-id="12b7e-197">String</span></span>|<span data-ttu-id="12b7e-p105">Чтобы идентифицировать свойства в коллекции **singleValueExtendedProperties**, для каждого из них укажите этот параметр. Свойство должно быть одного из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="12b7e-p105">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="12b7e-202">значение</span><span class="sxs-lookup"><span data-stu-id="12b7e-202">value</span></span>|<span data-ttu-id="12b7e-203">строка</span><span class="sxs-lookup"><span data-stu-id="12b7e-203">string</span></span>|<span data-ttu-id="12b7e-p106">Для каждого свойства из коллекции **singleValueExtendedProperties** следует указать значение. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="12b7e-p106">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="12b7e-206">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **singleValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12b7e-206">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="12b7e-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="12b7e-207">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="12b7e-208">Код отклика</span><span class="sxs-lookup"><span data-stu-id="12b7e-208">Response code</span></span>
<span data-ttu-id="12b7e-209">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="12b7e-209">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="12b7e-210">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="12b7e-210">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="12b7e-211">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="12b7e-211">Response body</span></span>

<span data-ttu-id="12b7e-p107">При создании расширенного свойства отклик будет включать только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы отобразить только что созданное расширенное свойство, [примените к экземпляру, содержащему это расширенное свойство, параметр $expand](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="12b7e-p107">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="12b7e-214">Когда вы создаете расширенное свойство в _новом_ экземпляре [group post](../resources/post.md) при ответе на беседу или публикацию, отклик будет включать только код отклика, но не новую публикацию или расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="12b7e-214">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="12b7e-215">Пример</span><span class="sxs-lookup"><span data-stu-id="12b7e-215">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="12b7e-216">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="12b7e-216">Request 1</span></span>

<span data-ttu-id="12b7e-p108">Первый пример показывает создание нового события и расширенного свойства с одним значением с помощью одной и той же операции POST. Помимо свойств, которые вы обычно указываете для нового события, тело запроса включает коллекцию **singleValueExtendedProperties**, которая содержит одно расширенное свойство с одним значением, и следующие данные для этого свойства:</span><span class="sxs-lookup"><span data-stu-id="12b7e-p108">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="12b7e-219">**id** (указывает тип свойства как `String`), GUID и свойство `Fun`.</span><span class="sxs-lookup"><span data-stu-id="12b7e-219">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="12b7e-220">**value** (указывает `Food` как значение свойства `Fun`).</span><span class="sxs-lookup"><span data-stu-id="12b7e-220">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="12b7e-221">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="12b7e-221">Response 1</span></span>

<span data-ttu-id="12b7e-p109">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="12b7e-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="12b7e-224">Чтобы просмотреть новое расширенное свойство, [разверните event с этим свойством](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="12b7e-224">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="12b7e-225">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="12b7e-225">Request 2</span></span>

<span data-ttu-id="12b7e-p110">Второй пример показывает создание расширенного свойства с одним значением для указанного существующего сообщения. Это расширенное свойство — единственный элемент в массиве **singleValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="12b7e-p110">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="12b7e-229">**id** (указывает тип свойства как `String`), GUID и свойство `Color`.</span><span class="sxs-lookup"><span data-stu-id="12b7e-229">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="12b7e-230">**value** (указывает `Green` как значение свойства `Color`).</span><span class="sxs-lookup"><span data-stu-id="12b7e-230">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="12b7e-231">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="12b7e-231">Response 2</span></span>

<span data-ttu-id="12b7e-p111">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="12b7e-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="12b7e-234">Чтобы просмотреть новое расширенное свойство, [разверните message с этим свойством](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="12b7e-234">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

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

