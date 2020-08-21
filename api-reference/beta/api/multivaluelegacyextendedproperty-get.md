---
title: Получение объекта multiValueLegacyExtendedProperty
description: expand'.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: ab8b9441bb6e97d6302d4f57c6c06077506d391b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849438"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="3fa8e-103">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="3fa8e-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="3fa8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fa8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="3fa8e-105">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-105">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="3fa8e-106">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-106">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="3fa8e-107">Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-107">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="3fa8e-108">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-108">The following user resources are supported:</span></span>

- <span data-ttu-id="3fa8e-109">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="3fa8e-109">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="3fa8e-110">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="3fa8e-110">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="3fa8e-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3fa8e-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="3fa8e-112">event</span><span class="sxs-lookup"><span data-stu-id="3fa8e-112">event</span></span>](../resources/event.md)
- [<span data-ttu-id="3fa8e-113">mailFolder</span><span class="sxs-lookup"><span data-stu-id="3fa8e-113">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="3fa8e-114">message</span><span class="sxs-lookup"><span data-stu-id="3fa8e-114">message</span></span>](../resources/message.md)
- [<span data-ttu-id="3fa8e-115">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="3fa8e-115">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="3fa8e-116">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="3fa8e-116">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="3fa8e-117">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-117">As well as the following group resources:</span></span>

- <span data-ttu-id="3fa8e-118">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="3fa8e-118">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="3fa8e-119">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="3fa8e-119">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="3fa8e-120">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-120">group [post](../resources/post.md)</span></span>

<span data-ttu-id="3fa8e-121">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="3fa8e-121">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fa8e-122">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa8e-122">Permissions</span></span>
<span data-ttu-id="3fa8e-123">В зависимости от ресурса, из которого вы получаете расширенное свойство, и типа запрашиваемого разрешения (делегированное или приложение), то для вызова этого API необходимо как минимум указать разрешение, указанное в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-123">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="3fa8e-124">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa8e-124">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fa8e-125">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="3fa8e-125">Supported resource</span></span> | <span data-ttu-id="3fa8e-126">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fa8e-126">Delegated (work or school account)</span></span> | <span data-ttu-id="3fa8e-127">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fa8e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fa8e-128">Приложение</span><span class="sxs-lookup"><span data-stu-id="3fa8e-128">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3fa8e-129">calendar</span><span class="sxs-lookup"><span data-stu-id="3fa8e-129">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="3fa8e-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-130">Calendars.Read</span></span> | <span data-ttu-id="3fa8e-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-131">Calendars.Read</span></span> | <span data-ttu-id="3fa8e-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-132">Calendars.Read</span></span> |
| [<span data-ttu-id="3fa8e-133">contact</span><span class="sxs-lookup"><span data-stu-id="3fa8e-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="3fa8e-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-134">Contacts.Read</span></span> | <span data-ttu-id="3fa8e-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-135">Contacts.Read</span></span> | <span data-ttu-id="3fa8e-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-136">Contacts.Read</span></span> |
| [<span data-ttu-id="3fa8e-137">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3fa8e-137">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="3fa8e-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-138">Contacts.Read</span></span> | <span data-ttu-id="3fa8e-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-139">Contacts.Read</span></span> | <span data-ttu-id="3fa8e-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-140">Contacts.Read</span></span> |
| [<span data-ttu-id="3fa8e-141">event</span><span class="sxs-lookup"><span data-stu-id="3fa8e-141">event</span></span>](../resources/event.md) | <span data-ttu-id="3fa8e-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-142">Calendars.Read</span></span> | <span data-ttu-id="3fa8e-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-143">Calendars.Read</span></span> |  <span data-ttu-id="3fa8e-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-144">Calendars.Read</span></span>|
| <span data-ttu-id="3fa8e-145">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="3fa8e-145">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="3fa8e-146">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fa8e-146">Group.Read.All</span></span> | <span data-ttu-id="3fa8e-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fa8e-147">Not supported</span></span> | <span data-ttu-id="3fa8e-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fa8e-148">Not supported</span></span> |
| <span data-ttu-id="3fa8e-149">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="3fa8e-149">group [event](../resources/event.md)</span></span> | <span data-ttu-id="3fa8e-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fa8e-150">Group.Read.All</span></span> | <span data-ttu-id="3fa8e-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fa8e-151">Not supported</span></span> | <span data-ttu-id="3fa8e-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fa8e-152">Not supported</span></span> |
| <span data-ttu-id="3fa8e-153">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-153">group [post](../resources/post.md)</span></span> | <span data-ttu-id="3fa8e-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fa8e-154">Group.Read.All</span></span> | <span data-ttu-id="3fa8e-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fa8e-155">Not supported</span></span> | <span data-ttu-id="3fa8e-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fa8e-156">Group.Read.All</span></span> |
| [<span data-ttu-id="3fa8e-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="3fa8e-157">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="3fa8e-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-158">Mail.Read</span></span> | <span data-ttu-id="3fa8e-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-159">Mail.Read</span></span> | <span data-ttu-id="3fa8e-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-160">Mail.Read</span></span> |
| [<span data-ttu-id="3fa8e-161">message</span><span class="sxs-lookup"><span data-stu-id="3fa8e-161">message</span></span>](../resources/message.md) | <span data-ttu-id="3fa8e-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-162">Mail.Read</span></span> | <span data-ttu-id="3fa8e-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-163">Mail.Read</span></span> | <span data-ttu-id="3fa8e-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-164">Mail.Read</span></span> |
| [<span data-ttu-id="3fa8e-165">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="3fa8e-165">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="3fa8e-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-166">Tasks.Read</span></span> | <span data-ttu-id="3fa8e-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-167">Tasks.Read</span></span> | <span data-ttu-id="3fa8e-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fa8e-168">Not supported</span></span> |
| [<span data-ttu-id="3fa8e-169">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="3fa8e-169">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="3fa8e-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-170">Tasks.Read</span></span> | <span data-ttu-id="3fa8e-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3fa8e-171">Tasks.Read</span></span> | <span data-ttu-id="3fa8e-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3fa8e-172">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fa8e-173">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fa8e-173">HTTP request</span></span>

<span data-ttu-id="3fa8e-p103">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="3fa8e-176">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-176">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="3fa8e-177">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-177">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="3fa8e-178">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-178">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="3fa8e-179">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-179">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="3fa8e-180">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-180">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="3fa8e-181">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-181">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="3fa8e-182">Получение **экземпляра outlookTask:**</span><span class="sxs-lookup"><span data-stu-id="3fa8e-182">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="3fa8e-183">Получение **экземпляра outlookTaskFolder:**</span><span class="sxs-lookup"><span data-stu-id="3fa8e-183">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="3fa8e-184">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-184">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="3fa8e-185">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="3fa8e-185">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="3fa8e-186">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3fa8e-186">Path parameters</span></span>
|<span data-ttu-id="3fa8e-187">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="3fa8e-187">**Parameter**</span></span>|<span data-ttu-id="3fa8e-188">**Тип**</span><span class="sxs-lookup"><span data-stu-id="3fa8e-188">**Type**</span></span>|<span data-ttu-id="3fa8e-189">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3fa8e-189">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3fa8e-190">id_value</span><span class="sxs-lookup"><span data-stu-id="3fa8e-190">id_value</span></span>|<span data-ttu-id="3fa8e-191">String</span><span class="sxs-lookup"><span data-stu-id="3fa8e-191">String</span></span>|<span data-ttu-id="3fa8e-p104">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3fa8e-196">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fa8e-196">Request headers</span></span>
| <span data-ttu-id="3fa8e-197">Имя</span><span class="sxs-lookup"><span data-stu-id="3fa8e-197">Name</span></span>      |<span data-ttu-id="3fa8e-198">Описание</span><span class="sxs-lookup"><span data-stu-id="3fa8e-198">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3fa8e-199">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fa8e-199">Authorization</span></span>  | <span data-ttu-id="3fa8e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fa8e-202">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fa8e-202">Request body</span></span>
<span data-ttu-id="3fa8e-203">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-203">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fa8e-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa8e-204">Response</span></span>

<span data-ttu-id="3fa8e-205">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-205">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="3fa8e-206">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="3fa8e-206">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="3fa8e-207">Пример</span><span class="sxs-lookup"><span data-stu-id="3fa8e-207">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fa8e-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fa8e-208">Request</span></span>
<span data-ttu-id="3fa8e-p106">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="3fa8e-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="3fa8e-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa8e-211">Response</span></span>

<span data-ttu-id="3fa8e-212">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-212">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="3fa8e-p107">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3fa8e-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
