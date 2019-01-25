---
title: Получение объекта multiValueLegacyExtendedProperty
description: Expand
localization_priority: Normal
ms.openlocfilehash: 7a649020bf326d4ec1ed3a83ae0c759a012378d4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525243"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="31b82-103">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="31b82-103">Get multiValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31b82-104">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="31b82-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="31b82-105">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="31b82-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="31b82-106">Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="31b82-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="31b82-107">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="31b82-107">The following user resources are supported:</span></span>

- <span data-ttu-id="31b82-108">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="31b82-108">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="31b82-109">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="31b82-109">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="31b82-110">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="31b82-110">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="31b82-111">event</span><span class="sxs-lookup"><span data-stu-id="31b82-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="31b82-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="31b82-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="31b82-113">message</span><span class="sxs-lookup"><span data-stu-id="31b82-113">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="31b82-114">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="31b82-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="31b82-115">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="31b82-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="31b82-116">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="31b82-116">As well as the following group resources:</span></span>

- <span data-ttu-id="31b82-117">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="31b82-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="31b82-118">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="31b82-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="31b82-119">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="31b82-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="31b82-120">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="31b82-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="31b82-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31b82-121">Permissions</span></span>
<span data-ttu-id="31b82-122">В зависимости от ресурса они будут расширенные свойства из и разрешение введите (делегированные или приложения) вы запроса, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="31b82-122">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="31b82-123">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31b82-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31b82-124">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="31b82-124">Supported resource</span></span> | <span data-ttu-id="31b82-125">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31b82-125">Delegated (work or school account)</span></span> | <span data-ttu-id="31b82-126">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31b82-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31b82-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31b82-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="31b82-128">calendar</span><span class="sxs-lookup"><span data-stu-id="31b82-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="31b82-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-129">Calendars.Read</span></span> | <span data-ttu-id="31b82-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-130">Calendars.Read</span></span> | <span data-ttu-id="31b82-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-131">Calendars.Read</span></span> |
| [<span data-ttu-id="31b82-132">contact</span><span class="sxs-lookup"><span data-stu-id="31b82-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="31b82-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-133">Contacts.Read</span></span> | <span data-ttu-id="31b82-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-134">Contacts.Read</span></span> | <span data-ttu-id="31b82-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-135">Contacts.Read</span></span> |
| <span data-ttu-id="31b82-136">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="31b82-136">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="31b82-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-137">Contacts.Read</span></span> | <span data-ttu-id="31b82-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-138">Contacts.Read</span></span> | <span data-ttu-id="31b82-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-139">Contacts.Read</span></span> |
| [<span data-ttu-id="31b82-140">event</span><span class="sxs-lookup"><span data-stu-id="31b82-140">event</span></span>](../resources/event.md) | <span data-ttu-id="31b82-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-141">Calendars.Read</span></span> | <span data-ttu-id="31b82-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-142">Calendars.Read</span></span> |  <span data-ttu-id="31b82-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-143">Calendars.Read</span></span>|
| <span data-ttu-id="31b82-144">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="31b82-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="31b82-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b82-145">Group.Read.All</span></span> | <span data-ttu-id="31b82-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31b82-146">Not supported</span></span> | <span data-ttu-id="31b82-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31b82-147">Not supported</span></span> |
| <span data-ttu-id="31b82-148">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="31b82-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="31b82-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b82-149">Group.Read.All</span></span> | <span data-ttu-id="31b82-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31b82-150">Not supported</span></span> | <span data-ttu-id="31b82-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31b82-151">Not supported</span></span> |
| <span data-ttu-id="31b82-152">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="31b82-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="31b82-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b82-153">Group.Read.All</span></span> | <span data-ttu-id="31b82-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31b82-154">Not supported</span></span> | <span data-ttu-id="31b82-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31b82-155">Group.Read.All</span></span> |
| [<span data-ttu-id="31b82-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="31b82-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="31b82-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-157">Mail.Read</span></span> | <span data-ttu-id="31b82-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-158">Mail.Read</span></span> | <span data-ttu-id="31b82-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-159">Mail.Read</span></span> |
| [<span data-ttu-id="31b82-160">message</span><span class="sxs-lookup"><span data-stu-id="31b82-160">message</span></span>](../resources/message.md) | <span data-ttu-id="31b82-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-161">Mail.Read</span></span> | <span data-ttu-id="31b82-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-162">Mail.Read</span></span> | <span data-ttu-id="31b82-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-163">Mail.Read</span></span> |
| [<span data-ttu-id="31b82-164">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="31b82-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="31b82-165">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-165">Tasks.Read</span></span> | <span data-ttu-id="31b82-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-166">Tasks.Read</span></span> | <span data-ttu-id="31b82-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31b82-167">Not supported</span></span> |
| [<span data-ttu-id="31b82-168">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="31b82-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="31b82-169">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-169">Tasks.Read</span></span> | <span data-ttu-id="31b82-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="31b82-170">Tasks.Read</span></span> | <span data-ttu-id="31b82-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31b82-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="31b82-172">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31b82-172">HTTP request</span></span>

<span data-ttu-id="31b82-p103">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="31b82-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="31b82-175">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="31b82-175">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31b82-176">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="31b82-176">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="31b82-177">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="31b82-177">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31b82-178">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="31b82-178">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31b82-179">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="31b82-179">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31b82-180">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="31b82-180">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="31b82-181">Получение экземпляра **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="31b82-181">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31b82-182">Получение экземпляра **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="31b82-182">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="31b82-183">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="31b82-183">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="31b82-184">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="31b82-184">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="31b82-185">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="31b82-185">Path parameters</span></span>
|<span data-ttu-id="31b82-186">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="31b82-186">**Parameter**</span></span>|<span data-ttu-id="31b82-187">**Тип**</span><span class="sxs-lookup"><span data-stu-id="31b82-187">**Type**</span></span>|<span data-ttu-id="31b82-188">**Описание**</span><span class="sxs-lookup"><span data-stu-id="31b82-188">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="31b82-189">id_value</span><span class="sxs-lookup"><span data-stu-id="31b82-189">id_value</span></span>|<span data-ttu-id="31b82-190">String</span><span class="sxs-lookup"><span data-stu-id="31b82-190">String</span></span>|<span data-ttu-id="31b82-p104">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31b82-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="31b82-195">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31b82-195">Request headers</span></span>
| <span data-ttu-id="31b82-196">Имя</span><span class="sxs-lookup"><span data-stu-id="31b82-196">Name</span></span>      |<span data-ttu-id="31b82-197">Описание</span><span class="sxs-lookup"><span data-stu-id="31b82-197">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31b82-198">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31b82-198">Authorization</span></span>  | <span data-ttu-id="31b82-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31b82-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31b82-201">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31b82-201">Request body</span></span>
<span data-ttu-id="31b82-202">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31b82-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31b82-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="31b82-203">Response</span></span>

<span data-ttu-id="31b82-204">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="31b82-204">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="31b82-205">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="31b82-205">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="31b82-206">Пример</span><span class="sxs-lookup"><span data-stu-id="31b82-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31b82-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="31b82-207">Request</span></span>
<span data-ttu-id="31b82-p106">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="31b82-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="31b82-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="31b82-210">Response</span></span>

<span data-ttu-id="31b82-211">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="31b82-211">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="31b82-p107">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="31b82-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
