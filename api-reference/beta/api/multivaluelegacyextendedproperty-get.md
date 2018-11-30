---
title: Получение объекта multiValueLegacyExtendedProperty
description: Разверните узел ".
ms.openlocfilehash: 9429737f3965acbf4c6bcc61c516327556223111
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079856"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="2a765-103">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="2a765-103">Get multiValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="2a765-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2a765-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a765-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a765-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2a765-106">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="2a765-106">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="2a765-107">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="2a765-107">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="2a765-108">Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="2a765-108">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="2a765-109">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="2a765-109">The following user resources are supported:</span></span>

- <span data-ttu-id="2a765-110">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="2a765-110">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="2a765-111">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="2a765-111">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="2a765-112">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="2a765-112">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="2a765-113">событие</span><span class="sxs-lookup"><span data-stu-id="2a765-113">event</span></span>](../resources/event.md)
- [<span data-ttu-id="2a765-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="2a765-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="2a765-115">message</span><span class="sxs-lookup"><span data-stu-id="2a765-115">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="2a765-116">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="2a765-116">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="2a765-117">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="2a765-117">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="2a765-118">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="2a765-118">As well as the following group resources:</span></span>

- <span data-ttu-id="2a765-119">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="2a765-119">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="2a765-120">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="2a765-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="2a765-121">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="2a765-121">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="2a765-122">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2a765-122">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a765-123">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a765-123">Permissions</span></span>
<span data-ttu-id="2a765-124">В зависимости от ресурса они будут расширенные свойства из и разрешение введите (делегированные или приложения) вы запроса, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="2a765-124">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="2a765-125">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a765-125">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a765-126">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="2a765-126">Supported resource</span></span> | <span data-ttu-id="2a765-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a765-127">Delegated (work or school account)</span></span> | <span data-ttu-id="2a765-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a765-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a765-129">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2a765-129">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="2a765-130">calendar</span><span class="sxs-lookup"><span data-stu-id="2a765-130">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="2a765-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-131">Calendars.Read</span></span> | <span data-ttu-id="2a765-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-132">Calendars.Read</span></span> | <span data-ttu-id="2a765-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-133">Calendars.Read</span></span> |
| [<span data-ttu-id="2a765-134">контакт</span><span class="sxs-lookup"><span data-stu-id="2a765-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2a765-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-135">Contacts.Read</span></span> | <span data-ttu-id="2a765-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-136">Contacts.Read</span></span> | <span data-ttu-id="2a765-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-137">Contacts.Read</span></span> |
| <span data-ttu-id="2a765-138">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="2a765-138">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="2a765-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-139">Contacts.Read</span></span> | <span data-ttu-id="2a765-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-140">Contacts.Read</span></span> | <span data-ttu-id="2a765-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-141">Contacts.Read</span></span> |
| [<span data-ttu-id="2a765-142">событие</span><span class="sxs-lookup"><span data-stu-id="2a765-142">event</span></span>](../resources/event.md) | <span data-ttu-id="2a765-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-143">Calendars.Read</span></span> | <span data-ttu-id="2a765-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-144">Calendars.Read</span></span> |  <span data-ttu-id="2a765-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-145">Calendars.Read</span></span>|
| <span data-ttu-id="2a765-146">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="2a765-146">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="2a765-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a765-147">Group.Read.All</span></span> | <span data-ttu-id="2a765-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a765-148">Not supported</span></span> | <span data-ttu-id="2a765-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a765-149">Not supported</span></span> |
| <span data-ttu-id="2a765-150">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="2a765-150">group [event](../resources/event.md)</span></span> | <span data-ttu-id="2a765-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a765-151">Group.Read.All</span></span> | <span data-ttu-id="2a765-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a765-152">Not supported</span></span> | <span data-ttu-id="2a765-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a765-153">Not supported</span></span> |
| <span data-ttu-id="2a765-154">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="2a765-154">group [post](../resources/post.md)</span></span> | <span data-ttu-id="2a765-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a765-155">Group.Read.All</span></span> | <span data-ttu-id="2a765-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a765-156">Not supported</span></span> | <span data-ttu-id="2a765-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a765-157">Group.Read.All</span></span> |
| [<span data-ttu-id="2a765-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="2a765-158">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="2a765-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-159">Mail.Read</span></span> | <span data-ttu-id="2a765-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-160">Mail.Read</span></span> | <span data-ttu-id="2a765-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-161">Mail.Read</span></span> |
| [<span data-ttu-id="2a765-162">message</span><span class="sxs-lookup"><span data-stu-id="2a765-162">message</span></span>](../resources/message.md) | <span data-ttu-id="2a765-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-163">Mail.Read</span></span> | <span data-ttu-id="2a765-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-164">Mail.Read</span></span> | <span data-ttu-id="2a765-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-165">Mail.Read</span></span> |
| [<span data-ttu-id="2a765-166">Задачи Outlook</span><span class="sxs-lookup"><span data-stu-id="2a765-166">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="2a765-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-167">Tasks.Read</span></span> | <span data-ttu-id="2a765-168">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-168">Tasks.Read</span></span> | <span data-ttu-id="2a765-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a765-169">Not supported</span></span> |
| [<span data-ttu-id="2a765-170">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="2a765-170">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="2a765-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-171">Tasks.Read</span></span> | <span data-ttu-id="2a765-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2a765-172">Tasks.Read</span></span> | <span data-ttu-id="2a765-173">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2a765-173">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="2a765-174">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a765-174">HTTP request</span></span>

<span data-ttu-id="2a765-p104">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="2a765-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="2a765-177">Получение экземпляра **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-177">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="2a765-178">Получение экземпляра **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-178">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="2a765-179">Получение экземпляра **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-179">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="2a765-180">Получение экземпляра **календаря** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-180">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="2a765-181">Получение экземпляра **контактов** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-181">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="2a765-182">Получение экземпляра **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-182">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="2a765-183">Получение экземпляра **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-183">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="2a765-184">Получение экземпляра **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-184">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="2a765-185">Получение экземпляра **события** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-185">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="2a765-186">Получение экземпляра **публиковать** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2a765-186">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="2a765-187">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="2a765-187">Path parameters</span></span>
|<span data-ttu-id="2a765-188">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="2a765-188">**Parameter**</span></span>|<span data-ttu-id="2a765-189">**Тип**</span><span class="sxs-lookup"><span data-stu-id="2a765-189">**Type**</span></span>|<span data-ttu-id="2a765-190">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2a765-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2a765-191">id_value</span><span class="sxs-lookup"><span data-stu-id="2a765-191">id_value</span></span>|<span data-ttu-id="2a765-192">String</span><span class="sxs-lookup"><span data-stu-id="2a765-192">String</span></span>|<span data-ttu-id="2a765-p105">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a765-p105">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2a765-197">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a765-197">Request headers</span></span>
| <span data-ttu-id="2a765-198">Имя</span><span class="sxs-lookup"><span data-stu-id="2a765-198">Name</span></span>      |<span data-ttu-id="2a765-199">Описание</span><span class="sxs-lookup"><span data-stu-id="2a765-199">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a765-200">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a765-200">Authorization</span></span>  | <span data-ttu-id="2a765-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a765-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a765-203">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a765-203">Request body</span></span>
<span data-ttu-id="2a765-204">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a765-204">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a765-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a765-205">Response</span></span>

<span data-ttu-id="2a765-206">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2a765-206">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="2a765-207">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="2a765-207">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="2a765-208">Пример</span><span class="sxs-lookup"><span data-stu-id="2a765-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a765-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a765-209">Request</span></span>
<span data-ttu-id="2a765-p107">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="2a765-p107">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="2a765-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a765-212">Response</span></span>

<span data-ttu-id="2a765-213">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="2a765-213">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="2a765-p108">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2a765-p108">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->