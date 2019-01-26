---
title: Создание многозначного расширенного свойства
description: 'Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса. '
localization_priority: Normal
ms.openlocfilehash: 4ed9af6fda2117fee7ef1ac50c69c4f006abd45d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576264"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="228b0-103">Создание многозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="228b0-103">Create multi-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="228b0-104">Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="228b0-104">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="228b0-105">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="228b0-105">The following user resources are supported:</span></span>

- <span data-ttu-id="228b0-106">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="228b0-106">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="228b0-107">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="228b0-107">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="228b0-108">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="228b0-108">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="228b0-109">event</span><span class="sxs-lookup"><span data-stu-id="228b0-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="228b0-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="228b0-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="228b0-111">message</span><span class="sxs-lookup"><span data-stu-id="228b0-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="228b0-112">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="228b0-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="228b0-113">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="228b0-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="228b0-114">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="228b0-114">As well as the following group resources:</span></span>

- <span data-ttu-id="228b0-115">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="228b0-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="228b0-116">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="228b0-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="228b0-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="228b0-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="228b0-118">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="228b0-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="228b0-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="228b0-119">Permissions</span></span>
<span data-ttu-id="228b0-120">В зависимости от ресурса при создании расширенные свойства в и введите (делегированные или приложения) вы запроса на разрешение, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="228b0-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="228b0-121">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="228b0-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="228b0-122">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="228b0-122">Supported resource</span></span> | <span data-ttu-id="228b0-123">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="228b0-123">Delegated (work or school account)</span></span> | <span data-ttu-id="228b0-124">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="228b0-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="228b0-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="228b0-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="228b0-126">calendar</span><span class="sxs-lookup"><span data-stu-id="228b0-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="228b0-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="228b0-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="228b0-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="228b0-130">contact</span><span class="sxs-lookup"><span data-stu-id="228b0-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="228b0-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="228b0-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="228b0-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-133">Contacts.ReadWrite</span></span> |
| <span data-ttu-id="228b0-134">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="228b0-134">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="228b0-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="228b0-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="228b0-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="228b0-138">event</span><span class="sxs-lookup"><span data-stu-id="228b0-138">event</span></span>](../resources/event.md) | <span data-ttu-id="228b0-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="228b0-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="228b0-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="228b0-142">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="228b0-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="228b0-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228b0-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="228b0-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-144">Not supported</span></span> | <span data-ttu-id="228b0-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-145">Not supported</span></span> |
| <span data-ttu-id="228b0-146">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="228b0-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="228b0-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228b0-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="228b0-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-148">Not supported</span></span> | <span data-ttu-id="228b0-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-149">Not supported</span></span> |
| <span data-ttu-id="228b0-150">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="228b0-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="228b0-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228b0-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="228b0-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-152">Not supported</span></span> | <span data-ttu-id="228b0-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-153">Not supported</span></span> |
| [<span data-ttu-id="228b0-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="228b0-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="228b0-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-155">Mail.ReadWrite</span></span> | <span data-ttu-id="228b0-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-156">Mail.ReadWrite</span></span> | <span data-ttu-id="228b0-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="228b0-158">message</span><span class="sxs-lookup"><span data-stu-id="228b0-158">message</span></span>](../resources/message.md) | <span data-ttu-id="228b0-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-159">Mail.ReadWrite</span></span> | <span data-ttu-id="228b0-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-160">Mail.ReadWrite</span></span> | <span data-ttu-id="228b0-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="228b0-162">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="228b0-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="228b0-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="228b0-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="228b0-165">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-165">Not supported</span></span> |
| [<span data-ttu-id="228b0-166">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="228b0-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="228b0-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="228b0-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228b0-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="228b0-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="228b0-169">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="228b0-170">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="228b0-170">HTTP request</span></span>
<span data-ttu-id="228b0-171">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="228b0-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="228b0-172">Создайте один или несколько расширенных свойств в _новый_ экземпляр ресурсов, использование того же запроса REST создания экземпляра и включить свойства нового ресурса экземпляра _и расширенные свойства_ в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="228b0-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="228b0-173">Обратите внимание, что некоторые ресурсы поддержки в несколько способов создания.</span><span class="sxs-lookup"><span data-stu-id="228b0-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="228b0-174">Дополнительные сведения о создании этих экземплярах ресурсов см в соответствующие разделы для создания [сообщения](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [события](../api/user-post-events.md), [календаря](../api/user-post-calendars.md), [контактов](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md) [задач Outlook](../resources/outlooktask.md), [ Папки задач Outlook](../resources/outlooktaskfolder.md), [событие группы](../api/group-post-events.md)и [группы post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="228b0-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="228b0-175">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="228b0-175">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="228b0-176">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="228b0-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="228b0-177">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="228b0-177">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="228b0-178">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="228b0-178">Request headers</span></span>
| <span data-ttu-id="228b0-179">Имя</span><span class="sxs-lookup"><span data-stu-id="228b0-179">Name</span></span>       | <span data-ttu-id="228b0-180">Значение</span><span class="sxs-lookup"><span data-stu-id="228b0-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="228b0-181">Авторизация</span><span class="sxs-lookup"><span data-stu-id="228b0-181">Authorization</span></span> | <span data-ttu-id="228b0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="228b0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="228b0-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="228b0-184">Content-Type</span></span> | <span data-ttu-id="228b0-185">application/json</span><span class="sxs-lookup"><span data-stu-id="228b0-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="228b0-186">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="228b0-186">Request body</span></span>

<span data-ttu-id="228b0-187">Предоставление текста JSON каждого объекта [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) в свойства коллекции **multiValueLegacyExtendedProperty** экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="228b0-187">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueLegacyExtendedProperty** collection property of the resource instance.</span></span>

|<span data-ttu-id="228b0-188">**Свойство**</span><span class="sxs-lookup"><span data-stu-id="228b0-188">**Property**</span></span>|<span data-ttu-id="228b0-189">**Тип**</span><span class="sxs-lookup"><span data-stu-id="228b0-189">**Type**</span></span>|<span data-ttu-id="228b0-190">**Описание**</span><span class="sxs-lookup"><span data-stu-id="228b0-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="228b0-191">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="228b0-191">multiValueLegacyExtendedProperty</span></span>|<span data-ttu-id="228b0-192">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="228b0-192">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="228b0-193">Массив из одного или нескольких многозначных расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="228b0-193">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="228b0-194">id</span><span class="sxs-lookup"><span data-stu-id="228b0-194">id</span></span>|<span data-ttu-id="228b0-195">Строка</span><span class="sxs-lookup"><span data-stu-id="228b0-195">String</span></span>|<span data-ttu-id="228b0-196">Для каждого свойства в коллекции **multiValueLegacyExtendedProperty** укажите это для идентификации свойство.</span><span class="sxs-lookup"><span data-stu-id="228b0-196">For each property in the **multiValueLegacyExtendedProperty** collection, specify this to identify the property.</span></span> <span data-ttu-id="228b0-197">Его необходимо выполнить один из поддерживаемых форматов.</span><span class="sxs-lookup"><span data-stu-id="228b0-197">It must follow one of the supported formats.</span></span> <span data-ttu-id="228b0-198">Для получения дополнительных сведений в разделе [Общие сведения о свойствах расширенные Outlook](../resources/extended-properties-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="228b0-198">See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information.</span></span> <span data-ttu-id="228b0-199">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="228b0-199">Required.</span></span>|
|<span data-ttu-id="228b0-200">value</span><span class="sxs-lookup"><span data-stu-id="228b0-200">value</span></span>|<span data-ttu-id="228b0-201">строка</span><span class="sxs-lookup"><span data-stu-id="228b0-201">string</span></span>|<span data-ttu-id="228b0-202">Для каждого свойства в коллекции **multiValueLegacyExtendedProperty** укажите значение свойства.</span><span class="sxs-lookup"><span data-stu-id="228b0-202">For each property in the **multiValueLegacyExtendedProperty** collection, specify the property value.</span></span> <span data-ttu-id="228b0-203">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="228b0-203">Required.</span></span>|

<span data-ttu-id="228b0-204">При создании расширенных свойств в _новый_ экземпляр ресурсов, в дополнение к новой коллекции **multiValueLegacyExtendedProperty** , для представления JSON этого экземпляра ресурсов (то есть, [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md) [событие](../resources/event.md), и т.д.)</span><span class="sxs-lookup"><span data-stu-id="228b0-204">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueLegacyExtendedProperty** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="228b0-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="228b0-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="228b0-206">Код отклика</span><span class="sxs-lookup"><span data-stu-id="228b0-206">Response code</span></span>
<span data-ttu-id="228b0-207">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="228b0-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="228b0-208">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="228b0-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="228b0-209">Тело отклика</span><span class="sxs-lookup"><span data-stu-id="228b0-209">Response body</span></span>

<span data-ttu-id="228b0-p106">При создании расширенного свойства в поддерживаемом ресурсе, отличном от [post для групп](../resources/post.md), отклик включает только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы просмотреть только что созданное расширенное свойство, [разверните экземпляр с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="228b0-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="228b0-p107">При создании расширенного свойства в _новом_ экземпляре post для групп отклик включает только код отклика и не содержит ни новой записи, ни расширенного свойства. Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="228b0-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="228b0-214">Пример</span><span class="sxs-lookup"><span data-stu-id="228b0-214">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="228b0-215">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="228b0-215">Request 1</span></span>

<span data-ttu-id="228b0-216">В первом примере создается Многозначный расширенные свойства в новое событие в одной и той же операции POST.</span><span class="sxs-lookup"><span data-stu-id="228b0-216">The first example creates a multi-value extended property in a new event all in the same POST operation.</span></span> <span data-ttu-id="228b0-217">За исключением свойства, которое обычно содержит новые события текст запроса включает в себя коллекцию **multiValueLegacyExtendedProperty** , которая содержит один расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="228b0-217">Apart from the properties you'd normally include for a new event, the request body includes the **multiValueLegacyExtendedProperty** collection which contains one extended property.</span></span> <span data-ttu-id="228b0-218">Текст запроса включает в себя следующие параметры для многозначного свойства расширенного:</span><span class="sxs-lookup"><span data-stu-id="228b0-218">The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="228b0-219">**id**. Задает свойство в виде массива строк с заданным идентификатором GUID и именем `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="228b0-219">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="228b0-220">**value**. Задает `Recreation` в виде массива из 3 строковых значений, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="228b0-220">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

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
  "multiValueLegacyExtendedProperty": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="228b0-221">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="228b0-221">Response 1</span></span>

<span data-ttu-id="228b0-p109">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="228b0-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="228b0-224">Чтобы просмотреть новое расширенное свойство, [разверните event с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="228b0-224">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="228b0-225">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="228b0-225">Request 2</span></span>

<span data-ttu-id="228b0-226">Во втором примере создает один Многозначный расширенные свойства для указанного сообщения.</span><span class="sxs-lookup"><span data-stu-id="228b0-226">The second example creates one multi-value extended property for the specified message.</span></span> <span data-ttu-id="228b0-227">Расширенные свойства это единственный элемент коллекции **multiValueLegacyExtendedProperty** .</span><span class="sxs-lookup"><span data-stu-id="228b0-227">That extended property is the only element in the **multiValueLegacyExtendedProperty** collection.</span></span> <span data-ttu-id="228b0-228">Текст запроса включает в себя следующие параметры для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="228b0-228">The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="228b0-229">**id**. Задает свойство в виде массива строк с указанным идентификатором GUID и именем `Palette`.</span><span class="sxs-lookup"><span data-stu-id="228b0-229">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="228b0-230">**value**. Задает `Palette` в виде массива 3 строковых значений, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="228b0-230">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueLegacyExtendedProperty": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="228b0-231">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="228b0-231">Response 2</span></span>

<span data-ttu-id="228b0-p111">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="228b0-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="228b0-234">Чтобы просмотреть новое расширенное свойство, [разверните message с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="228b0-234">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->




