---
title: Создание расширенного свойства с одним значением
description: 'Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: f5cfd9e123c63a8b629dfddb38d93b78c219cfe4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132099"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="73628-103">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="73628-103">Create single-value extended property</span></span>

<span data-ttu-id="73628-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73628-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="73628-105">Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="73628-105">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="73628-106">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="73628-106">The following user resources are supported:</span></span>

- <span data-ttu-id="73628-107">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="73628-107">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="73628-108">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="73628-108">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="73628-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="73628-109">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="73628-110">event</span><span class="sxs-lookup"><span data-stu-id="73628-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="73628-111">mailFolder</span><span class="sxs-lookup"><span data-stu-id="73628-111">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="73628-112">message</span><span class="sxs-lookup"><span data-stu-id="73628-112">message</span></span>](../resources/message.md)
- [<span data-ttu-id="73628-113">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="73628-113">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="73628-114">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="73628-114">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="73628-115">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="73628-115">As well as the following group resources:</span></span>

- <span data-ttu-id="73628-116">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="73628-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="73628-117">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="73628-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="73628-118">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="73628-118">group [post](../resources/post.md)</span></span>

<span data-ttu-id="73628-119">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="73628-119">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="73628-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73628-120">Permissions</span></span>
<span data-ttu-id="73628-121">В зависимости от ресурса, в который вы создаете расширенное свойство, и типа запрашиваемого разрешения (делегирования или приложения), разрешение, указанное в следующей таблице, является минимальным, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="73628-121">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="73628-122">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73628-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73628-123">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="73628-123">Supported resource</span></span> | <span data-ttu-id="73628-124">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73628-124">Delegated (work or school account)</span></span> | <span data-ttu-id="73628-125">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73628-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73628-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73628-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="73628-127">calendar</span><span class="sxs-lookup"><span data-stu-id="73628-127">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="73628-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="73628-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="73628-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-130">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="73628-131">контакт</span><span class="sxs-lookup"><span data-stu-id="73628-131">contact</span></span>](../resources/contact.md) | <span data-ttu-id="73628-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="73628-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="73628-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-134">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="73628-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="73628-135">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="73628-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="73628-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="73628-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-138">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="73628-139">event</span><span class="sxs-lookup"><span data-stu-id="73628-139">event</span></span>](../resources/event.md) | <span data-ttu-id="73628-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-140">Calendars.ReadWrite</span></span> | <span data-ttu-id="73628-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-141">Calendars.ReadWrite</span></span> |  <span data-ttu-id="73628-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-142">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="73628-143">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="73628-143">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="73628-144">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73628-144">Group.ReadWrite.All</span></span> | <span data-ttu-id="73628-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-145">Not supported</span></span> | <span data-ttu-id="73628-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-146">Not supported</span></span> |
| <span data-ttu-id="73628-147">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="73628-147">group [event](../resources/event.md)</span></span> | <span data-ttu-id="73628-148">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73628-148">Group.ReadWrite.All</span></span> | <span data-ttu-id="73628-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-149">Not supported</span></span> | <span data-ttu-id="73628-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-150">Not supported</span></span> |
| <span data-ttu-id="73628-151">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="73628-151">group [post](../resources/post.md)</span></span> | <span data-ttu-id="73628-152">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73628-152">Group.ReadWrite.All</span></span> | <span data-ttu-id="73628-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-153">Not supported</span></span> | <span data-ttu-id="73628-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-154">Not supported</span></span> |
| [<span data-ttu-id="73628-155">mailFolder</span><span class="sxs-lookup"><span data-stu-id="73628-155">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="73628-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-156">Mail.ReadWrite</span></span> | <span data-ttu-id="73628-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-157">Mail.ReadWrite</span></span> | <span data-ttu-id="73628-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-158">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="73628-159">message</span><span class="sxs-lookup"><span data-stu-id="73628-159">message</span></span>](../resources/message.md) | <span data-ttu-id="73628-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-160">Mail.ReadWrite</span></span> | <span data-ttu-id="73628-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-161">Mail.ReadWrite</span></span> | <span data-ttu-id="73628-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-162">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="73628-163">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="73628-163">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="73628-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="73628-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="73628-166">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-166">Not supported</span></span> |
| [<span data-ttu-id="73628-167">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="73628-167">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="73628-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="73628-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73628-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="73628-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73628-170">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="73628-171">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73628-171">HTTP request</span></span>
<span data-ttu-id="73628-172">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="73628-172">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="73628-173">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_.</span><span class="sxs-lookup"><span data-stu-id="73628-173">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="73628-174">Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания.</span><span class="sxs-lookup"><span data-stu-id="73628-174">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="73628-175">Дополнительные сведения о создании этих экземпляров ресурсов см. в соответствующих [](../api/group-post-events.md)темах для создания сообщения, [mailFolder,](../api/user-post-mailfolders.md) [события](../api/user-post-events.md) [,](../api/user-post-calendars.md)календаря, контакта , [contactFolder](../api/user-post-contactfolders.md), [задачи Outlook,](../resources/outlooktask.md)папки задач [Outlook,](../resources/outlooktaskfolder.md)события группы и публикации группы [.](../resources/post.md) [](../resources/message.md) [](../api/user-post-contacts.md)</span><span class="sxs-lookup"><span data-stu-id="73628-175">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span>

<span data-ttu-id="73628-176">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="73628-176">The following is the syntax of the requests.</span></span>

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

<span data-ttu-id="73628-177">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="73628-177">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="73628-178">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="73628-178">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="73628-179">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73628-179">Request headers</span></span>
| <span data-ttu-id="73628-180">Имя</span><span class="sxs-lookup"><span data-stu-id="73628-180">Name</span></span>       | <span data-ttu-id="73628-181">Значение</span><span class="sxs-lookup"><span data-stu-id="73628-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="73628-182">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73628-182">Authorization</span></span> | <span data-ttu-id="73628-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73628-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73628-185">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73628-185">Content-Type</span></span> | <span data-ttu-id="73628-186">application/json</span><span class="sxs-lookup"><span data-stu-id="73628-186">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="73628-187">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73628-187">Request body</span></span>

<span data-ttu-id="73628-188">Предоставьте тело JSON каждого объекта [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) в свойстве коллекции **singleValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="73628-188">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="73628-189">**Property**</span><span class="sxs-lookup"><span data-stu-id="73628-189">**Property**</span></span>|<span data-ttu-id="73628-190">**Тип**</span><span class="sxs-lookup"><span data-stu-id="73628-190">**Type**</span></span>|<span data-ttu-id="73628-191">**Описание**</span><span class="sxs-lookup"><span data-stu-id="73628-191">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73628-192">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="73628-192">singleValueExtendedProperties</span></span>|<span data-ttu-id="73628-193">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="73628-193">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="73628-194">Массив из одного или нескольких расширенных свойств с одним значением.</span><span class="sxs-lookup"><span data-stu-id="73628-194">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="73628-195">id</span><span class="sxs-lookup"><span data-stu-id="73628-195">id</span></span>|<span data-ttu-id="73628-196">Строка</span><span class="sxs-lookup"><span data-stu-id="73628-196">String</span></span>|<span data-ttu-id="73628-p104">Чтобы идентифицировать свойства в коллекции **singleValueExtendedProperties**, для каждого из них укажите этот параметр. Свойство должно быть одного из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="73628-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="73628-201">значение</span><span class="sxs-lookup"><span data-stu-id="73628-201">value</span></span>|<span data-ttu-id="73628-202">string</span><span class="sxs-lookup"><span data-stu-id="73628-202">string</span></span>|<span data-ttu-id="73628-p105">Для каждого свойства из коллекции **singleValueExtendedProperties** следует указать значение. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="73628-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="73628-205">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **singleValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73628-205">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="73628-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="73628-206">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="73628-207">Код ответа</span><span class="sxs-lookup"><span data-stu-id="73628-207">Response code</span></span>
<span data-ttu-id="73628-208">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="73628-208">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="73628-209">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="73628-209">In an existing resource instance, a successful create operation returns `200 OK`.</span></span>


#### <a name="response-body"></a><span data-ttu-id="73628-210">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="73628-210">Response body</span></span>

<span data-ttu-id="73628-p106">При создании расширенного свойства отклик будет включать только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы отобразить только что созданное расширенное свойство, [примените к экземпляру, содержащему это расширенное свойство, параметр $expand](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="73628-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="73628-213">Когда вы создаете расширенное свойство в _новом_ экземпляре [group post](../resources/post.md) при ответе на беседу или публикацию, отклик будет включать только код отклика, но не новую публикацию или расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="73628-213">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="73628-214">Пример</span><span class="sxs-lookup"><span data-stu-id="73628-214">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="73628-215">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="73628-215">Request 1</span></span>

<span data-ttu-id="73628-p107">Первый пример показывает создание нового события и расширенного свойства с одним значением с помощью одной и той же операции POST. Помимо свойств, которые вы обычно указываете для нового события, тело запроса включает коллекцию **singleValueExtendedProperties**, которая содержит одно расширенное свойство с одним значением, и следующие данные для этого свойства:</span><span class="sxs-lookup"><span data-stu-id="73628-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="73628-218">**id** (указывает тип свойства как `String`), GUID и свойство `Fun`.</span><span class="sxs-lookup"><span data-stu-id="73628-218">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="73628-219">**value** (указывает `Food` как значение свойства `Fun`).</span><span class="sxs-lookup"><span data-stu-id="73628-219">**value** specifies `Food` as the value of the `Fun` property.</span></span>

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

##### <a name="response-1"></a><span data-ttu-id="73628-220">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="73628-220">Response 1</span></span>

<span data-ttu-id="73628-p108">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="73628-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="73628-223">Чтобы отобразить только что созданное расширенное свойство, [примените к событию, к которому относится это свойство, параметр $expand](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="73628-223">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="73628-224">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="73628-224">Request 2</span></span>

<span data-ttu-id="73628-p109">Второй пример показывает создание расширенного свойства с одним значением для указанного существующего сообщения. Это расширенное свойство — единственный элемент в массиве **singleValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="73628-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="73628-228">**id** (указывает тип свойства как `String`), GUID и свойство `Color`.</span><span class="sxs-lookup"><span data-stu-id="73628-228">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="73628-229">**value** (указывает `Green` как значение свойства `Color`).</span><span class="sxs-lookup"><span data-stu-id="73628-229">**value** specifies `Green` as the value of the `Color` property.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="73628-230">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="73628-230">Response 2</span></span>

<span data-ttu-id="73628-p110">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="73628-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="73628-233">Чтобы отобразить только что созданное расширенное свойство, [примените к сообщению, к которому относится это свойство, параметр $expand](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="73628-233">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

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



