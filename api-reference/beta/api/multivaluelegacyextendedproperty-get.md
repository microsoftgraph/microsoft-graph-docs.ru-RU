---
title: Получение объекта multiValueLegacyExtendedProperty
description: Разверните узел ".
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: f7a8122ecd4440b1d43ff05eed21c023535d57f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043103"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="74c32-103">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="74c32-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="74c32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74c32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="74c32-105">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="74c32-105">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="74c32-106">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="74c32-106">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="74c32-107">Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="74c32-107">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="74c32-108">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="74c32-108">The following user resources are supported:</span></span>

- <span data-ttu-id="74c32-109">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="74c32-109">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="74c32-110">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="74c32-110">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="74c32-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="74c32-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="74c32-112">event</span><span class="sxs-lookup"><span data-stu-id="74c32-112">event</span></span>](../resources/event.md)
- [<span data-ttu-id="74c32-113">mailFolder</span><span class="sxs-lookup"><span data-stu-id="74c32-113">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="74c32-114">message</span><span class="sxs-lookup"><span data-stu-id="74c32-114">message</span></span>](../resources/message.md)
- [<span data-ttu-id="74c32-115">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="74c32-115">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="74c32-116">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="74c32-116">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="74c32-117">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="74c32-117">As well as the following group resources:</span></span>

- <span data-ttu-id="74c32-118">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="74c32-118">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="74c32-119">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="74c32-119">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="74c32-120">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="74c32-120">group [post](../resources/post.md)</span></span>

<span data-ttu-id="74c32-121">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="74c32-121">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="74c32-122">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74c32-122">Permissions</span></span>
<span data-ttu-id="74c32-123">В зависимости от ресурса, из которого вы получаете расширенное свойство, а также от запрашиваемого типа разрешения (делегированного или приложения), для вызова этого API требуется минимум разрешение, указанное в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="74c32-123">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="74c32-124">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74c32-124">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74c32-125">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="74c32-125">Supported resource</span></span> | <span data-ttu-id="74c32-126">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74c32-126">Delegated (work or school account)</span></span> | <span data-ttu-id="74c32-127">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74c32-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c32-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74c32-128">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="74c32-129">calendar</span><span class="sxs-lookup"><span data-stu-id="74c32-129">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="74c32-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-130">Calendars.Read</span></span> | <span data-ttu-id="74c32-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-131">Calendars.Read</span></span> | <span data-ttu-id="74c32-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-132">Calendars.Read</span></span> |
| [<span data-ttu-id="74c32-133">contact</span><span class="sxs-lookup"><span data-stu-id="74c32-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="74c32-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-134">Contacts.Read</span></span> | <span data-ttu-id="74c32-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-135">Contacts.Read</span></span> | <span data-ttu-id="74c32-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-136">Contacts.Read</span></span> |
| [<span data-ttu-id="74c32-137">contactFolder</span><span class="sxs-lookup"><span data-stu-id="74c32-137">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="74c32-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-138">Contacts.Read</span></span> | <span data-ttu-id="74c32-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-139">Contacts.Read</span></span> | <span data-ttu-id="74c32-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-140">Contacts.Read</span></span> |
| [<span data-ttu-id="74c32-141">event</span><span class="sxs-lookup"><span data-stu-id="74c32-141">event</span></span>](../resources/event.md) | <span data-ttu-id="74c32-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-142">Calendars.Read</span></span> | <span data-ttu-id="74c32-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-143">Calendars.Read</span></span> |  <span data-ttu-id="74c32-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-144">Calendars.Read</span></span>|
| <span data-ttu-id="74c32-145">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="74c32-145">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="74c32-146">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="74c32-146">Group.Read.All</span></span> | <span data-ttu-id="74c32-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74c32-147">Not supported</span></span> | <span data-ttu-id="74c32-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74c32-148">Not supported</span></span> |
| <span data-ttu-id="74c32-149">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="74c32-149">group [event](../resources/event.md)</span></span> | <span data-ttu-id="74c32-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="74c32-150">Group.Read.All</span></span> | <span data-ttu-id="74c32-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74c32-151">Not supported</span></span> | <span data-ttu-id="74c32-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74c32-152">Not supported</span></span> |
| <span data-ttu-id="74c32-153">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="74c32-153">group [post](../resources/post.md)</span></span> | <span data-ttu-id="74c32-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="74c32-154">Group.Read.All</span></span> | <span data-ttu-id="74c32-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74c32-155">Not supported</span></span> | <span data-ttu-id="74c32-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="74c32-156">Group.Read.All</span></span> |
| [<span data-ttu-id="74c32-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="74c32-157">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="74c32-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-158">Mail.Read</span></span> | <span data-ttu-id="74c32-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-159">Mail.Read</span></span> | <span data-ttu-id="74c32-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-160">Mail.Read</span></span> |
| [<span data-ttu-id="74c32-161">message</span><span class="sxs-lookup"><span data-stu-id="74c32-161">message</span></span>](../resources/message.md) | <span data-ttu-id="74c32-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-162">Mail.Read</span></span> | <span data-ttu-id="74c32-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-163">Mail.Read</span></span> | <span data-ttu-id="74c32-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-164">Mail.Read</span></span> |
| [<span data-ttu-id="74c32-165">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="74c32-165">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="74c32-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-166">Tasks.Read</span></span> | <span data-ttu-id="74c32-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-167">Tasks.Read</span></span> | <span data-ttu-id="74c32-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74c32-168">Not supported</span></span> |
| [<span data-ttu-id="74c32-169">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="74c32-169">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="74c32-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-170">Tasks.Read</span></span> | <span data-ttu-id="74c32-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="74c32-171">Tasks.Read</span></span> | <span data-ttu-id="74c32-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="74c32-172">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="74c32-173">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74c32-173">HTTP request</span></span>

<span data-ttu-id="74c32-p103">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="74c32-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="74c32-176">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="74c32-176">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="74c32-177">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="74c32-177">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="74c32-178">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="74c32-178">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="74c32-179">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="74c32-179">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="74c32-180">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="74c32-180">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="74c32-181">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="74c32-181">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="74c32-182">Получение экземпляра **outlookTask** :</span><span class="sxs-lookup"><span data-stu-id="74c32-182">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="74c32-183">Получение экземпляра **outlookTaskFolder** :</span><span class="sxs-lookup"><span data-stu-id="74c32-183">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="74c32-184">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="74c32-184">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="74c32-185">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="74c32-185">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="74c32-186">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="74c32-186">Path parameters</span></span>
|<span data-ttu-id="74c32-187">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="74c32-187">**Parameter**</span></span>|<span data-ttu-id="74c32-188">**Тип**</span><span class="sxs-lookup"><span data-stu-id="74c32-188">**Type**</span></span>|<span data-ttu-id="74c32-189">**Описание**</span><span class="sxs-lookup"><span data-stu-id="74c32-189">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="74c32-190">id_value</span><span class="sxs-lookup"><span data-stu-id="74c32-190">id_value</span></span>|<span data-ttu-id="74c32-191">String</span><span class="sxs-lookup"><span data-stu-id="74c32-191">String</span></span>|<span data-ttu-id="74c32-p104">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74c32-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="74c32-196">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74c32-196">Request headers</span></span>
| <span data-ttu-id="74c32-197">Имя</span><span class="sxs-lookup"><span data-stu-id="74c32-197">Name</span></span>      |<span data-ttu-id="74c32-198">Описание</span><span class="sxs-lookup"><span data-stu-id="74c32-198">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="74c32-199">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74c32-199">Authorization</span></span>  | <span data-ttu-id="74c32-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74c32-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74c32-202">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74c32-202">Request body</span></span>
<span data-ttu-id="74c32-203">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74c32-203">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74c32-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="74c32-204">Response</span></span>

<span data-ttu-id="74c32-205">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="74c32-205">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="74c32-206">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="74c32-206">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="74c32-207">Пример</span><span class="sxs-lookup"><span data-stu-id="74c32-207">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74c32-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="74c32-208">Request</span></span>
<span data-ttu-id="74c32-p106">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="74c32-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="74c32-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="74c32-211">Response</span></span>

<span data-ttu-id="74c32-212">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="74c32-212">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="74c32-p107">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74c32-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->


