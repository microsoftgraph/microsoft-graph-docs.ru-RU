---
title: Создание расширенного свойства с несколькими значениями
description: 'Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e63dd8b810feba508addccc6e30a30993b1e1ccf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511434"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="860ad-103">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="860ad-103">Create multi-value extended property</span></span>

<span data-ttu-id="860ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="860ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="860ad-105">Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="860ad-105">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="860ad-106">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="860ad-106">The following user resources are supported:</span></span>

- <span data-ttu-id="860ad-107">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="860ad-107">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="860ad-108">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="860ad-108">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="860ad-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="860ad-109">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="860ad-110">event</span><span class="sxs-lookup"><span data-stu-id="860ad-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="860ad-111">mailFolder</span><span class="sxs-lookup"><span data-stu-id="860ad-111">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="860ad-112">message</span><span class="sxs-lookup"><span data-stu-id="860ad-112">message</span></span>](../resources/message.md)

<span data-ttu-id="860ad-113">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="860ad-113">As well as the following group resources:</span></span>

- <span data-ttu-id="860ad-114">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="860ad-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="860ad-115">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="860ad-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="860ad-116">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="860ad-116">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="860ad-117">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="860ad-117">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="860ad-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="860ad-118">Permissions</span></span>
<span data-ttu-id="860ad-119">В зависимости от ресурса, в котором вы создаете расширенное свойство и запрашивается тип разрешения (делегированное или приложение), разрешение, указанное в следующей таблице, является минимальным необходимым условием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="860ad-119">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="860ad-120">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="860ad-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="860ad-121">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="860ad-121">Supported resource</span></span> | <span data-ttu-id="860ad-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="860ad-122">Delegated (work or school account)</span></span> | <span data-ttu-id="860ad-123">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="860ad-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="860ad-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="860ad-124">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="860ad-125">calendar</span><span class="sxs-lookup"><span data-stu-id="860ad-125">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="860ad-126">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-126">Calendars.ReadWrite</span></span> | <span data-ttu-id="860ad-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="860ad-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-128">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="860ad-129">contact</span><span class="sxs-lookup"><span data-stu-id="860ad-129">contact</span></span>](../resources/contact.md) | <span data-ttu-id="860ad-130">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-130">Contacts.ReadWrite</span></span> | <span data-ttu-id="860ad-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="860ad-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-132">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="860ad-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="860ad-133">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="860ad-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="860ad-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="860ad-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-136">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="860ad-137">event</span><span class="sxs-lookup"><span data-stu-id="860ad-137">event</span></span>](../resources/event.md) | <span data-ttu-id="860ad-138">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-138">Calendars.ReadWrite</span></span> | <span data-ttu-id="860ad-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-139">Calendars.ReadWrite</span></span> |  <span data-ttu-id="860ad-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-140">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="860ad-141">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="860ad-141">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="860ad-142">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="860ad-142">Group.ReadWrite.All</span></span> | <span data-ttu-id="860ad-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="860ad-143">Not supported</span></span> | <span data-ttu-id="860ad-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="860ad-144">Not supported</span></span> |
| <span data-ttu-id="860ad-145">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="860ad-145">group [event](../resources/event.md)</span></span> | <span data-ttu-id="860ad-146">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="860ad-146">Group.ReadWrite.All</span></span> | <span data-ttu-id="860ad-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="860ad-147">Not supported</span></span> | <span data-ttu-id="860ad-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="860ad-148">Not supported</span></span> |
| <span data-ttu-id="860ad-149">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="860ad-149">group [post](../resources/post.md)</span></span> | <span data-ttu-id="860ad-150">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="860ad-150">Group.ReadWrite.All</span></span> | <span data-ttu-id="860ad-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="860ad-151">Not supported</span></span> | <span data-ttu-id="860ad-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="860ad-152">Not supported</span></span> |
| [<span data-ttu-id="860ad-153">mailFolder</span><span class="sxs-lookup"><span data-stu-id="860ad-153">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="860ad-154">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-154">Mail.ReadWrite</span></span> | <span data-ttu-id="860ad-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-155">Mail.ReadWrite</span></span> | <span data-ttu-id="860ad-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-156">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="860ad-157">message</span><span class="sxs-lookup"><span data-stu-id="860ad-157">message</span></span>](../resources/message.md) | <span data-ttu-id="860ad-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-158">Mail.ReadWrite</span></span> | <span data-ttu-id="860ad-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-159">Mail.ReadWrite</span></span> | <span data-ttu-id="860ad-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="860ad-160">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="860ad-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="860ad-161">HTTP request</span></span>
<span data-ttu-id="860ad-162">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="860ad-162">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="860ad-p102">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_. Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания. Дополнительные сведения о создании этих экземпляров ресурса вы найдете в соответствующих статьях о создании [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md) и [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="860ad-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="860ad-166">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="860ad-166">The following is the syntax of the requests.</span></span> 

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

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="860ad-167">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="860ad-167">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="860ad-168">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="860ad-168">**Note** You cannot create an extended property in an existing group post.</span></span>

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

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="860ad-169">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="860ad-169">Request headers</span></span>
| <span data-ttu-id="860ad-170">Имя</span><span class="sxs-lookup"><span data-stu-id="860ad-170">Name</span></span>       | <span data-ttu-id="860ad-171">Значение</span><span class="sxs-lookup"><span data-stu-id="860ad-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="860ad-172">Авторизация</span><span class="sxs-lookup"><span data-stu-id="860ad-172">Authorization</span></span> | <span data-ttu-id="860ad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="860ad-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="860ad-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="860ad-175">Content-Type</span></span> | <span data-ttu-id="860ad-176">application/json</span><span class="sxs-lookup"><span data-stu-id="860ad-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="860ad-177">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="860ad-177">Request body</span></span>

<span data-ttu-id="860ad-178">Предоставьте тело в формате JSON для каждого объекта [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) в свойстве коллекции **multiValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="860ad-178">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="860ad-179">Свойство</span><span class="sxs-lookup"><span data-stu-id="860ad-179">Property</span></span>|<span data-ttu-id="860ad-180">Тип</span><span class="sxs-lookup"><span data-stu-id="860ad-180">Type</span></span>|<span data-ttu-id="860ad-181">Описание</span><span class="sxs-lookup"><span data-stu-id="860ad-181">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="860ad-182">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="860ad-182">multiValueExtendedProperties</span></span>|<span data-ttu-id="860ad-183">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="860ad-183">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="860ad-184">Массив из одного или нескольких многозначных расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="860ad-184">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="860ad-185">id</span><span class="sxs-lookup"><span data-stu-id="860ad-185">id</span></span>|<span data-ttu-id="860ad-186">String</span><span class="sxs-lookup"><span data-stu-id="860ad-186">String</span></span>|<span data-ttu-id="860ad-p104">Чтобы идентифицировать свойства в коллекции **multiValueExtendedProperties**, укажите этот параметр для каждого из них. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="860ad-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="860ad-191">значение</span><span class="sxs-lookup"><span data-stu-id="860ad-191">value</span></span>|<span data-ttu-id="860ad-192">string</span><span class="sxs-lookup"><span data-stu-id="860ad-192">string</span></span>|<span data-ttu-id="860ad-p105">Укажите значение для каждого свойства в коллекции **multiValueExtendedProperties**. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="860ad-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="860ad-195">При создании расширенного свойства в _новом_ экземпляре ресурса в дополнение к новой коллекции **multiValueExtendedProperties** предоставьте представление этого экземпляра ресурса в формате JSON (то есть [сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [событие](../resources/event.md)и т. д.).</span><span class="sxs-lookup"><span data-stu-id="860ad-195">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance as well (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.).</span></span>


## <a name="response"></a><span data-ttu-id="860ad-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="860ad-196">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="860ad-197">Код ответа</span><span class="sxs-lookup"><span data-stu-id="860ad-197">Response code</span></span>
<span data-ttu-id="860ad-198">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="860ad-198">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="860ad-199">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="860ad-199">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="860ad-200">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="860ad-200">Response body</span></span>

<span data-ttu-id="860ad-p106">При создании расширенного свойства в поддерживаемом ресурсе, отличном от [post для групп](../resources/post.md), отклик включает только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы просмотреть только что созданное расширенное свойство, [разверните экземпляр с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="860ad-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="860ad-p107">При создании расширенного свойства в _новом_ экземпляре post для групп отклик включает только код отклика и не содержит ни новой записи, ни расширенного свойства. Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="860ad-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="860ad-205">Пример</span><span class="sxs-lookup"><span data-stu-id="860ad-205">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="860ad-206">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="860ad-206">Request 1</span></span>

<span data-ttu-id="860ad-p108">В первом примере в новом экземпляре event создается многозначное расширенное свойство с помощью одной операции POST. Помимо свойств, которые обычно указываются для нового события, тело запроса включает коллекцию **multiValueExtendedProperties**, которая содержит одно расширенное свойство. Тело запроса включает следующие данные для многозначного расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="860ad-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="860ad-210">**id**. Задает свойство в виде массива строк с заданным идентификатором GUID и именем `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="860ad-210">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="860ad-211">**value**. Задает `Recreation` в виде массива из 3 строковых значений, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="860ad-211">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
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

##### <a name="response-1"></a><span data-ttu-id="860ad-212">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="860ad-212">Response 1</span></span>

<span data-ttu-id="860ad-p109">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="860ad-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="860ad-215">Чтобы отобразить только что созданное расширенное свойство, [примените к событию, к которому относится это свойство, параметр $expand](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="860ad-215">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="860ad-216">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="860ad-216">Request 2</span></span>

<span data-ttu-id="860ad-p110">Во втором примере создается многозначное расширенное свойство для указанного сообщения. Это расширенное свойство — единственный элемент в коллекции **multiValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="860ad-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="860ad-220">**id**. Задает свойство в виде массива строк с указанным идентификатором GUID и именем `Palette`.</span><span class="sxs-lookup"><span data-stu-id="860ad-220">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="860ad-221">**value**. Задает `Palette` в виде массива 3 строковых значений, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="860ad-221">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

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

##### <a name="response-2"></a><span data-ttu-id="860ad-222">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="860ad-222">Response 2</span></span>

<span data-ttu-id="860ad-p111">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="860ad-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="860ad-225">Чтобы отобразить только что созданное расширенное свойство, [примените к сообщению, к которому относится это свойство, параметр $expand](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="860ad-225">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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




