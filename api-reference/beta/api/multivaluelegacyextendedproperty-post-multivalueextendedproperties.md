---
title: Создание расширенного свойства с несколькими значениями
description: 'Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: fd6986161e84aecc17c908c3118bbd813d92f0ef
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131014"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="c7dea-103">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="c7dea-103">Create multi-value extended property</span></span>

<span data-ttu-id="c7dea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7dea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="c7dea-105">Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7dea-105">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="c7dea-106">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="c7dea-106">The following user resources are supported:</span></span>

- <span data-ttu-id="c7dea-107">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="c7dea-107">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="c7dea-108">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="c7dea-108">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="c7dea-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c7dea-109">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="c7dea-110">event</span><span class="sxs-lookup"><span data-stu-id="c7dea-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="c7dea-111">mailFolder</span><span class="sxs-lookup"><span data-stu-id="c7dea-111">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="c7dea-112">message</span><span class="sxs-lookup"><span data-stu-id="c7dea-112">message</span></span>](../resources/message.md)
- [<span data-ttu-id="c7dea-113">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="c7dea-113">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="c7dea-114">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="c7dea-114">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="c7dea-115">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="c7dea-115">As well as the following group resources:</span></span>

- <span data-ttu-id="c7dea-116">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="c7dea-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="c7dea-117">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="c7dea-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="c7dea-118">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="c7dea-118">group [post](../resources/post.md)</span></span>

<span data-ttu-id="c7dea-119">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c7dea-119">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7dea-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7dea-120">Permissions</span></span>
<span data-ttu-id="c7dea-121">В зависимости от ресурса, в который вы создаете расширенное свойство, и типа запрашиваемого разрешения (делегирования или приложения), разрешение, указанное в следующей таблице, является минимальным, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c7dea-121">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="c7dea-122">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7dea-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7dea-123">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="c7dea-123">Supported resource</span></span> | <span data-ttu-id="c7dea-124">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7dea-124">Delegated (work or school account)</span></span> | <span data-ttu-id="c7dea-125">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7dea-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7dea-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7dea-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="c7dea-127">calendar</span><span class="sxs-lookup"><span data-stu-id="c7dea-127">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="c7dea-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="c7dea-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="c7dea-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-130">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="c7dea-131">контакт</span><span class="sxs-lookup"><span data-stu-id="c7dea-131">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c7dea-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="c7dea-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="c7dea-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-134">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="c7dea-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c7dea-135">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="c7dea-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="c7dea-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="c7dea-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-138">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="c7dea-139">event</span><span class="sxs-lookup"><span data-stu-id="c7dea-139">event</span></span>](../resources/event.md) | <span data-ttu-id="c7dea-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-140">Calendars.ReadWrite</span></span> | <span data-ttu-id="c7dea-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-141">Calendars.ReadWrite</span></span> |  <span data-ttu-id="c7dea-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-142">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="c7dea-143">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="c7dea-143">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="c7dea-144">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7dea-144">Group.ReadWrite.All</span></span> | <span data-ttu-id="c7dea-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-145">Not supported</span></span> | <span data-ttu-id="c7dea-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-146">Not supported</span></span> |
| <span data-ttu-id="c7dea-147">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="c7dea-147">group [event](../resources/event.md)</span></span> | <span data-ttu-id="c7dea-148">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7dea-148">Group.ReadWrite.All</span></span> | <span data-ttu-id="c7dea-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-149">Not supported</span></span> | <span data-ttu-id="c7dea-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-150">Not supported</span></span> |
| <span data-ttu-id="c7dea-151">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="c7dea-151">group [post](../resources/post.md)</span></span> | <span data-ttu-id="c7dea-152">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7dea-152">Group.ReadWrite.All</span></span> | <span data-ttu-id="c7dea-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-153">Not supported</span></span> | <span data-ttu-id="c7dea-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-154">Not supported</span></span> |
| [<span data-ttu-id="c7dea-155">mailFolder</span><span class="sxs-lookup"><span data-stu-id="c7dea-155">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="c7dea-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-156">Mail.ReadWrite</span></span> | <span data-ttu-id="c7dea-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-157">Mail.ReadWrite</span></span> | <span data-ttu-id="c7dea-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-158">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="c7dea-159">message</span><span class="sxs-lookup"><span data-stu-id="c7dea-159">message</span></span>](../resources/message.md) | <span data-ttu-id="c7dea-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-160">Mail.ReadWrite</span></span> | <span data-ttu-id="c7dea-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-161">Mail.ReadWrite</span></span> | <span data-ttu-id="c7dea-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-162">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="c7dea-163">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="c7dea-163">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="c7dea-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="c7dea-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="c7dea-166">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-166">Not supported</span></span> |
| [<span data-ttu-id="c7dea-167">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="c7dea-167">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="c7dea-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="c7dea-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7dea-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="c7dea-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c7dea-170">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7dea-171">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7dea-171">HTTP request</span></span>
<span data-ttu-id="c7dea-172">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7dea-172">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="c7dea-173">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_.</span><span class="sxs-lookup"><span data-stu-id="c7dea-173">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="c7dea-174">Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания.</span><span class="sxs-lookup"><span data-stu-id="c7dea-174">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="c7dea-175">Дополнительные сведения о создании этих экземпляров ресурсов см. в соответствующих [](../api/group-post-events.md)темах для создания сообщения, [mailFolder,](../api/user-post-mailfolders.md) [события](../api/user-post-events.md) [,](../api/user-post-calendars.md)календаря, контакта , [contactFolder](../api/user-post-contactfolders.md), [задачи Outlook,](../resources/outlooktask.md)папки задач [Outlook,](../resources/outlooktaskfolder.md)события группы и публикации группы [.](../resources/post.md) [](../resources/message.md) [](../api/user-post-contacts.md)</span><span class="sxs-lookup"><span data-stu-id="c7dea-175">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span>

<span data-ttu-id="c7dea-176">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="c7dea-176">The following is the syntax of the requests.</span></span>

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

<span data-ttu-id="c7dea-177">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="c7dea-177">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="c7dea-178">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="c7dea-178">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="c7dea-179">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7dea-179">Request headers</span></span>
| <span data-ttu-id="c7dea-180">Имя</span><span class="sxs-lookup"><span data-stu-id="c7dea-180">Name</span></span>       | <span data-ttu-id="c7dea-181">Значение</span><span class="sxs-lookup"><span data-stu-id="c7dea-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c7dea-182">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7dea-182">Authorization</span></span> | <span data-ttu-id="c7dea-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7dea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7dea-185">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7dea-185">Content-Type</span></span> | <span data-ttu-id="c7dea-186">application/json</span><span class="sxs-lookup"><span data-stu-id="c7dea-186">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7dea-187">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7dea-187">Request body</span></span>

<span data-ttu-id="c7dea-188">Предоставьте тело в формате JSON для каждого объекта [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) в свойстве коллекции **multiValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="c7dea-188">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="c7dea-189">**Property**</span><span class="sxs-lookup"><span data-stu-id="c7dea-189">**Property**</span></span>|<span data-ttu-id="c7dea-190">**Тип**</span><span class="sxs-lookup"><span data-stu-id="c7dea-190">**Type**</span></span>|<span data-ttu-id="c7dea-191">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7dea-191">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c7dea-192">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c7dea-192">multiValueExtendedProperties</span></span>|<span data-ttu-id="c7dea-193">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c7dea-193">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c7dea-194">Массив из одного или нескольких многозначных расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="c7dea-194">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="c7dea-195">id</span><span class="sxs-lookup"><span data-stu-id="c7dea-195">id</span></span>|<span data-ttu-id="c7dea-196">Строка</span><span class="sxs-lookup"><span data-stu-id="c7dea-196">String</span></span>|<span data-ttu-id="c7dea-p104">Чтобы идентифицировать свойства в коллекции **multiValueExtendedProperties**, укажите этот параметр для каждого из них. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c7dea-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="c7dea-201">значение</span><span class="sxs-lookup"><span data-stu-id="c7dea-201">value</span></span>|<span data-ttu-id="c7dea-202">string</span><span class="sxs-lookup"><span data-stu-id="c7dea-202">string</span></span>|<span data-ttu-id="c7dea-p105">Укажите значение для каждого свойства в коллекции **multiValueExtendedProperties**. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c7dea-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="c7dea-205">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **multiValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7dea-205">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="c7dea-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7dea-206">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="c7dea-207">Код ответа</span><span class="sxs-lookup"><span data-stu-id="c7dea-207">Response code</span></span>
<span data-ttu-id="c7dea-208">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="c7dea-208">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="c7dea-209">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c7dea-209">In an existing resource instance, a successful create operation returns `200 OK`.</span></span>


#### <a name="response-body"></a><span data-ttu-id="c7dea-210">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="c7dea-210">Response body</span></span>

<span data-ttu-id="c7dea-p106">При создании расширенного свойства в поддерживаемом ресурсе, отличном от [post для групп](../resources/post.md), отклик включает только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы просмотреть только что созданное расширенное свойство, [разверните экземпляр с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="c7dea-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="c7dea-p107">При создании расширенного свойства в _новом_ экземпляре post для групп отклик включает только код отклика и не содержит ни новой записи, ни расширенного свойства. Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="c7dea-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="c7dea-215">Пример</span><span class="sxs-lookup"><span data-stu-id="c7dea-215">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c7dea-216">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="c7dea-216">Request 1</span></span>

<span data-ttu-id="c7dea-p108">В первом примере в новом экземпляре event создается многозначное расширенное свойство с помощью одной операции POST. Помимо свойств, которые обычно указываются для нового события, тело запроса включает коллекцию **multiValueExtendedProperties**, которая содержит одно расширенное свойство. Тело запроса включает следующие данные для многозначного расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="c7dea-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="c7dea-220">**id**. Задает свойство в виде массива строк с заданным идентификатором GUID и именем `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="c7dea-220">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span>
- <span data-ttu-id="c7dea-221">**value**. Задает `Recreation` в виде массива из 3 строковых значений, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="c7dea-221">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>


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

##### <a name="response-1"></a><span data-ttu-id="c7dea-222">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="c7dea-222">Response 1</span></span>

<span data-ttu-id="c7dea-p109">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="c7dea-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="c7dea-225">Чтобы отобразить только что созданное расширенное свойство, [примените к событию, к которому относится это свойство, параметр $expand](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="c7dea-225">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="c7dea-226">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="c7dea-226">Request 2</span></span>

<span data-ttu-id="c7dea-p110">Во втором примере создается многозначное расширенное свойство для указанного сообщения. Это расширенное свойство — единственный элемент в коллекции **multiValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="c7dea-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="c7dea-230">**id**. Задает свойство в виде массива строк с указанным идентификатором GUID и именем `Palette`.</span><span class="sxs-lookup"><span data-stu-id="c7dea-230">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="c7dea-231">**value**. Задает `Palette` в виде массива 3 строковых значений, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="c7dea-231">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="c7dea-232">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="c7dea-232">Response 2</span></span>

<span data-ttu-id="c7dea-p111">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="c7dea-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="c7dea-235">Чтобы отобразить только что созданное расширенное свойство, [примените к сообщению, к которому относится это свойство, параметр $expand](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="c7dea-235">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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
  "suppressions": []
}
-->






