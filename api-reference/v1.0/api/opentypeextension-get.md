---
title: Получение открытого расширения
description: Получение открытого расширения (объекта openTypeExtension), указанного по имени или полному имени.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: c977bc2d84c84aacf851268d50858487b08f3115
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049501"
---
# <a name="get-open-extension"></a><span data-ttu-id="3bd9a-103">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="3bd9a-103">Get open extension</span></span>

<span data-ttu-id="3bd9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bd9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3bd9a-105">Получение открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)), определенного по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-105">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="3bd9a-106">В таблице раздела [Разрешения](#permissions) перечислены ресурсы, поддерживающие открытые расширения.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-106">The table in the [Permissions](#permissions) section lists the resources that support open extensions.</span></span>

<span data-ttu-id="3bd9a-107">В приведенной ниже таблице перечислены три сценария, согласно которым можно получить открытое расширение из поддерживаемого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-107">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="3bd9a-108">**Сценарий GET**</span><span class="sxs-lookup"><span data-stu-id="3bd9a-108">**GET scenario**</span></span>|<span data-ttu-id="3bd9a-109">**Поддерживаемые ресурсы**</span><span class="sxs-lookup"><span data-stu-id="3bd9a-109">**Supported resources**</span></span>|<span data-ttu-id="3bd9a-110">**Текст ответа**</span><span class="sxs-lookup"><span data-stu-id="3bd9a-110">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3bd9a-111">Получение определенного расширения из экземпляра известного ресурса.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-111">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="3bd9a-112">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md), [task](../resources/todotask.md), [tasklist](../resources/todotasklist.md).</span><span class="sxs-lookup"><span data-stu-id="3bd9a-112">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md), [task](../resources/todotask.md), [tasklist](../resources/todotasklist.md).</span></span>  | <span data-ttu-id="3bd9a-113">Только открытое расширение.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-113">Open extension only.</span></span>|
|<span data-ttu-id="3bd9a-114">Получение экземпляра известного ресурса, дополненного определенным расширением.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-114">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="3bd9a-115">Device, event, group, group event, group post, message, organization, personal contact, user, task, task list.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-115">Device, event, group, group event, group post, message, organization, personal contact, user, task, task list.</span></span> |<span data-ttu-id="3bd9a-116">Экземпляр известного ресурса, дополненный открытым расширением.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-116">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="3bd9a-117">Поиск экземпляров ресурсов и их дополнение определенным расширением.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-117">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="3bd9a-118">Event, group event, group post, message, personal contact, task, task list.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-118">Event, group event, group post, message, personal contact, task, task list.</span></span>|<span data-ttu-id="3bd9a-119">Экземпляры ресурса, дополненные открытым расширением.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-119">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="3bd9a-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bd9a-120">Permissions</span></span>

<span data-ttu-id="3bd9a-121">В зависимости от того, какой ресурс содержит расширение, и типа запрашиваемого расширения (делегированного или для приложений), разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-121">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3bd9a-122">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bd9a-122">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bd9a-123">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="3bd9a-123">Supported resource</span></span> | <span data-ttu-id="3bd9a-124">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bd9a-124">Delegated (work or school account)</span></span> | <span data-ttu-id="3bd9a-125">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bd9a-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bd9a-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bd9a-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3bd9a-127">device</span><span class="sxs-lookup"><span data-stu-id="3bd9a-127">device</span></span>](../resources/device.md) | <span data-ttu-id="3bd9a-128">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-128">Directory.Read.All</span></span> | <span data-ttu-id="3bd9a-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3bd9a-129">Not supported</span></span> | <span data-ttu-id="3bd9a-130">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-130">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="3bd9a-131">event</span><span class="sxs-lookup"><span data-stu-id="3bd9a-131">event</span></span>](../resources/event.md) | <span data-ttu-id="3bd9a-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-132">Calendars.Read</span></span> | <span data-ttu-id="3bd9a-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-133">Calendars.Read</span></span> | <span data-ttu-id="3bd9a-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-134">Calendars.Read</span></span> |
| [<span data-ttu-id="3bd9a-135">group</span><span class="sxs-lookup"><span data-stu-id="3bd9a-135">group</span></span>](../resources/group.md) | <span data-ttu-id="3bd9a-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-136">Group.Read.All</span></span> | <span data-ttu-id="3bd9a-137">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3bd9a-137">Not supported</span></span> | <span data-ttu-id="3bd9a-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-138">Group.Read.All</span></span> |
| [<span data-ttu-id="3bd9a-139">Событие для групп</span><span class="sxs-lookup"><span data-stu-id="3bd9a-139">group event</span></span>](../resources/event.md) | <span data-ttu-id="3bd9a-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-140">Group.Read.All</span></span> | <span data-ttu-id="3bd9a-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3bd9a-141">Not supported</span></span> | <span data-ttu-id="3bd9a-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3bd9a-142">Not supported</span></span> |
| <span data-ttu-id="3bd9a-143">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="3bd9a-143">[group post](../resources/post.md)</span></span> | <span data-ttu-id="3bd9a-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-144">Group.Read.All</span></span> | <span data-ttu-id="3bd9a-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3bd9a-145">Not supported</span></span> | <span data-ttu-id="3bd9a-146">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-146">Group.Read.All</span></span> |
| [<span data-ttu-id="3bd9a-147">message</span><span class="sxs-lookup"><span data-stu-id="3bd9a-147">message</span></span>](../resources/message.md) | <span data-ttu-id="3bd9a-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-148">Mail.Read</span></span> | <span data-ttu-id="3bd9a-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-149">Mail.Read</span></span> | <span data-ttu-id="3bd9a-150">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-150">Mail.Read</span></span> | 
| [<span data-ttu-id="3bd9a-151">organization</span><span class="sxs-lookup"><span data-stu-id="3bd9a-151">organization</span></span>](../resources/organization.md) | <span data-ttu-id="3bd9a-152">User.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-152">User.Read</span></span> | <span data-ttu-id="3bd9a-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3bd9a-153">Not supported</span></span> | <span data-ttu-id="3bd9a-154">Organization.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-154">Organization.Read.All</span></span> |
| <span data-ttu-id="3bd9a-155">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="3bd9a-155">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="3bd9a-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-156">Contacts.Read</span></span> | <span data-ttu-id="3bd9a-157">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-157">Contacts.Read</span></span> | <span data-ttu-id="3bd9a-158">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-158">Contacts.Read</span></span> |
| [<span data-ttu-id="3bd9a-159">user</span><span class="sxs-lookup"><span data-stu-id="3bd9a-159">user</span></span>](../resources/user.md) | <span data-ttu-id="3bd9a-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-160">User.Read</span></span> | <span data-ttu-id="3bd9a-161">User.Read</span><span class="sxs-lookup"><span data-stu-id="3bd9a-161">User.Read</span></span> | <span data-ttu-id="3bd9a-162">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-162">User.Read.All</span></span> |
| [<span data-ttu-id="3bd9a-163">task</span><span class="sxs-lookup"><span data-stu-id="3bd9a-163">task</span></span>](../resources/todotask.md) | <span data-ttu-id="3bd9a-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bd9a-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="3bd9a-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bd9a-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="3bd9a-166">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-166">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="3bd9a-167">tasklist</span><span class="sxs-lookup"><span data-stu-id="3bd9a-167">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="3bd9a-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bd9a-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="3bd9a-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bd9a-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="3bd9a-170">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd9a-170">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bd9a-171">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bd9a-171">HTTP request</span></span>

<span data-ttu-id="3bd9a-172">В этом разделе указан синтаксис для каждого из трех перечисленных выше сценариев с `GET`.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-172">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="3bd9a-173">Получение определенного расширения в известном экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="3bd9a-173">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="3bd9a-174">Используйте такой же запрос REST, что и при получении экземпляра ресурса, и определите расширение с помощью свойства навигации **extensions** этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-174">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/extensions/{extensionId}
```

### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="3bd9a-175">Получение известного экземпляра ресурса с соответствующим расширением</span><span class="sxs-lookup"><span data-stu-id="3bd9a-175">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="3bd9a-176">Для типов ресурса, таких как event, group event, group post, message, personal contact, task, task list, можно использовать такой же запрос REST, что и при получении экземпляра ресурса. Найдите расширение, соответствующее заданному свойству **id**, и дополните экземпляр расширением.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-176">For the event, group event, group post, message, personal contact, task, task list resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="3bd9a-177">Отклик включает большинство свойств ресурса.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-177">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/todo/lists/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```

<span data-ttu-id="3bd9a-178">Для типов ресурса device, group, organization и user также необходимо использовать параметр `$select`, чтобы включить свойство **id** и другие свойства, которые необходимо получить из экземпляра ресурса:</span><span class="sxs-lookup"><span data-stu-id="3bd9a-178">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="3bd9a-179">Фильтрация экземпляров ресурсов с соответствующим расширением</span><span class="sxs-lookup"><span data-stu-id="3bd9a-179">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="3bd9a-180">Используйте такой же запрос REST, что и при получении коллекции поддерживаемого ресурса, отфильтруйте в коллекции экземпляры, содержащие расширение с соответствующим свойством **id**, и дополните эти экземпляры расширением.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-180">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="3bd9a-181">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения коллекции или экземпляров ресурсов, чье расширение нужно получить.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-181">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it.</span></span> <span data-ttu-id="3bd9a-182">Все другие варианты синтаксиса, позволяющие определить эти коллекции или экземпляры ресурсов, поддерживают получение открытых расширений этих экземпляров или коллекций подобным образом.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-182">All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="3bd9a-183">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3bd9a-183">Path parameters</span></span>
|<span data-ttu-id="3bd9a-184">Параметр</span><span class="sxs-lookup"><span data-stu-id="3bd9a-184">Parameter</span></span>|<span data-ttu-id="3bd9a-185">Тип</span><span class="sxs-lookup"><span data-stu-id="3bd9a-185">Type</span></span>|<span data-ttu-id="3bd9a-186">Описание</span><span class="sxs-lookup"><span data-stu-id="3bd9a-186">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3bd9a-187">Id</span><span class="sxs-lookup"><span data-stu-id="3bd9a-187">Id</span></span>|<span data-ttu-id="3bd9a-188">string</span><span class="sxs-lookup"><span data-stu-id="3bd9a-188">string</span></span>|<span data-ttu-id="3bd9a-p104">Заполнитель уникального идентификатора для объекта в соответствующей коллекции, например сообщения, события или контакта. Обязательный. Не следует путать его со свойством **id** объекта **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="3bd9a-192">extensionId</span><span class="sxs-lookup"><span data-stu-id="3bd9a-192">extensionId</span></span>|<span data-ttu-id="3bd9a-193">string</span><span class="sxs-lookup"><span data-stu-id="3bd9a-193">string</span></span>|<span data-ttu-id="3bd9a-p105">Заполнитель имени расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полного имени, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве **id** при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="3bd9a-197">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3bd9a-197">Optional query parameters</span></span>

<span data-ttu-id="3bd9a-198">Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке `$filter`.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-198">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="3bd9a-199">Параметр</span><span class="sxs-lookup"><span data-stu-id="3bd9a-199">Parameter</span></span>|<span data-ttu-id="3bd9a-200">Описание</span><span class="sxs-lookup"><span data-stu-id="3bd9a-200">Description</span></span>|<span data-ttu-id="3bd9a-201">Пример</span><span class="sxs-lookup"><span data-stu-id="3bd9a-201">Example</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="3bd9a-202">$filter</span><span class="sxs-lookup"><span data-stu-id="3bd9a-202">$filter</span></span>|<span data-ttu-id="3bd9a-203">Возвращает расширение, свойство **id** которого совпадает со значением параметра `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-203">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="3bd9a-204">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="3bd9a-204">Request 3</span></span>](#request-3)|
|<span data-ttu-id="3bd9a-205">$filter с **любым** оператором</span><span class="sxs-lookup"><span data-stu-id="3bd9a-205">$filter with **any** operator</span></span>|<span data-ttu-id="3bd9a-206">Возвращает экземпляры коллекции ресурсов, содержащие расширение, свойство **id** которого совпадает со значением параметра `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-206">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="3bd9a-207">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="3bd9a-207">Request 5</span></span>](#request-5)|
|<span data-ttu-id="3bd9a-208">$expand</span><span class="sxs-lookup"><span data-stu-id="3bd9a-208">$expand</span></span>|<span data-ttu-id="3bd9a-209">Дополняет экземпляр ресурса расширением.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-209">Expands a resource instance to include an extension.</span></span> |<span data-ttu-id="3bd9a-210">[Запрос 3](#request-3) и [запрос 5](#request-5)</span><span class="sxs-lookup"><span data-stu-id="3bd9a-210">[Request 3](#request-3) and [request 5](#request-5)</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3bd9a-211">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bd9a-211">Request headers</span></span>
| <span data-ttu-id="3bd9a-212">Имя</span><span class="sxs-lookup"><span data-stu-id="3bd9a-212">Name</span></span>       | <span data-ttu-id="3bd9a-213">Значение</span><span class="sxs-lookup"><span data-stu-id="3bd9a-213">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3bd9a-214">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bd9a-214">Authorization</span></span> | <span data-ttu-id="3bd9a-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bd9a-217">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bd9a-217">Request body</span></span>
<span data-ttu-id="3bd9a-218">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-218">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bd9a-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bd9a-219">Response</span></span>

<span data-ttu-id="3bd9a-p107">В случае успеха этот метод возвращает код отклика `200 OK` и объект [openTypeExtension](../resources/opentypeextension.md) в тексте отклика. Точный текст отклика зависит от запроса GET.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="3bd9a-222">Пример</span><span class="sxs-lookup"><span data-stu-id="3bd9a-222">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="3bd9a-223">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="3bd9a-223">Request 1</span></span>

<span data-ttu-id="3bd9a-p108">В первом примере показаны 2 способа обращения к расширению и получение расширения в указанном сообщении. Отклик не зависит от того, как вы ссылаетесь на расширение.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="3bd9a-226">По имени:</span><span class="sxs-lookup"><span data-stu-id="3bd9a-226">First, by its name:</span></span> 


# <a name="http"></a>[<span data-ttu-id="3bd9a-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bd9a-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="3bd9a-228">C#</span><span class="sxs-lookup"><span data-stu-id="3bd9a-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bd9a-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bd9a-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bd9a-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bd9a-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bd9a-231">Java</span><span class="sxs-lookup"><span data-stu-id="3bd9a-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="3bd9a-232">По идентификатору (полному имени):</span><span class="sxs-lookup"><span data-stu-id="3bd9a-232">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="3bd9a-233">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="3bd9a-233">Response 1</span></span>
<span data-ttu-id="3bd9a-234">Ниже представлен отклик для первого примера.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-234">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="3bd9a-235">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="3bd9a-235">Request 2</span></span>

<span data-ttu-id="3bd9a-236">Во втором примере показано, как сослаться на расширение по его имени и получить расширение в указанном событии группы.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-236">The second example references an extension by its name and gets the extension in the specified group event.</span></span>


# <a name="http"></a>[<span data-ttu-id="3bd9a-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bd9a-237">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```
# <a name="c"></a>[<span data-ttu-id="3bd9a-238">C#</span><span class="sxs-lookup"><span data-stu-id="3bd9a-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bd9a-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bd9a-239">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bd9a-240">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bd9a-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bd9a-241">Java</span><span class="sxs-lookup"><span data-stu-id="3bd9a-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="3bd9a-242">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="3bd9a-242">Response 2</span></span>

<span data-ttu-id="3bd9a-243">Ниже представлен отклик из второго примера.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-243">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="3bd9a-244">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="3bd9a-244">Request 3</span></span>

<span data-ttu-id="3bd9a-p109">В третьем примере показано, как получить и дополнить указанное сообщение, добавив расширение, возвращенное из фильтра. Фильтр возвращает расширение, свойство **id** которого совпадает с полным именем.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>


# <a name="http"></a>[<span data-ttu-id="3bd9a-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bd9a-247">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```
# <a name="c"></a>[<span data-ttu-id="3bd9a-248">C#</span><span class="sxs-lookup"><span data-stu-id="3bd9a-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bd9a-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bd9a-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bd9a-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bd9a-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bd9a-251">Java</span><span class="sxs-lookup"><span data-stu-id="3bd9a-251">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response-3"></a><span data-ttu-id="3bd9a-252">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="3bd9a-252">Response 3</span></span>

<span data-ttu-id="3bd9a-253">Ниже представлен отклик из третьего примера.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-253">And here is the response from the third example.</span></span> <span data-ttu-id="3bd9a-254">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-254">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a><span data-ttu-id="3bd9a-255">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="3bd9a-255">Request 4</span></span>

<span data-ttu-id="3bd9a-256">В четвертом примере показано, как сослаться на расширение по его полному имени и получить расширение в указанной записи группы.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-256">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>


# <a name="http"></a>[<span data-ttu-id="3bd9a-257">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bd9a-257">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```
# <a name="c"></a>[<span data-ttu-id="3bd9a-258">C#</span><span class="sxs-lookup"><span data-stu-id="3bd9a-258">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bd9a-259">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bd9a-259">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bd9a-260">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bd9a-260">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bd9a-261">Java</span><span class="sxs-lookup"><span data-stu-id="3bd9a-261">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-4"></a><span data-ttu-id="3bd9a-262">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="3bd9a-262">Response 4</span></span>

<span data-ttu-id="3bd9a-263">Ниже представлен отклик из четвертого примера.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-263">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a><span data-ttu-id="3bd9a-264">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="3bd9a-264">Request 5</span></span>

<span data-ttu-id="3bd9a-p111">В пятом примере показано, как найти в почтовом ящике вошедшего пользователя сообщения с расширениями, соответствующими фильтру, и дополнить их расширением. Фильтр возвращает расширения, свойство **id** которых совпадает с именем расширения `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="3bd9a-267">Отклик 5</span><span class="sxs-lookup"><span data-stu-id="3bd9a-267">Response 5</span></span>

<span data-ttu-id="3bd9a-268">В этом отклике для пятого примера почтовый ящик пользователя содержит только одно сообщение, свойство **id** которого имеет значение `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-268">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="3bd9a-269">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3bd9a-269">Note: The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

