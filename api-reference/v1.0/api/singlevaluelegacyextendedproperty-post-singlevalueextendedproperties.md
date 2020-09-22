---
title: Создание расширенного свойства с одним значением
description: 'Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d94bfaca767eeafbeced12b4597186831b115b69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038188"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="00ded-103">Создание расширенного свойства с одним значением</span><span class="sxs-lookup"><span data-stu-id="00ded-103">Create single-value extended property</span></span>

<span data-ttu-id="00ded-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00ded-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00ded-105">Создайте одно или несколько свойств с одним значением в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="00ded-105">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span>

<span data-ttu-id="00ded-106">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="00ded-106">The following user resources are supported:</span></span>

- <span data-ttu-id="00ded-107">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="00ded-107">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="00ded-108">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="00ded-108">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="00ded-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="00ded-109">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="00ded-110">event</span><span class="sxs-lookup"><span data-stu-id="00ded-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="00ded-111">mailFolder</span><span class="sxs-lookup"><span data-stu-id="00ded-111">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="00ded-112">message</span><span class="sxs-lookup"><span data-stu-id="00ded-112">message</span></span>](../resources/message.md)

<span data-ttu-id="00ded-113">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="00ded-113">As well as the following group resources:</span></span>

- <span data-ttu-id="00ded-114">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="00ded-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="00ded-115">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="00ded-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="00ded-116">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="00ded-116">group [post](../resources/post.md)</span></span>

<span data-ttu-id="00ded-117">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="00ded-117">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="00ded-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00ded-118">Permissions</span></span>
<span data-ttu-id="00ded-119">В зависимости от ресурса, в котором вы создаете расширенное свойство и запрашивается тип разрешения (делегированное или приложение), разрешение, указанное в следующей таблице, является минимальным необходимым условием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="00ded-119">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="00ded-120">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00ded-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00ded-121">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="00ded-121">Supported resource</span></span> | <span data-ttu-id="00ded-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00ded-122">Delegated (work or school account)</span></span> | <span data-ttu-id="00ded-123">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00ded-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ded-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00ded-124">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="00ded-125">calendar</span><span class="sxs-lookup"><span data-stu-id="00ded-125">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="00ded-126">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-126">Calendars.ReadWrite</span></span> | <span data-ttu-id="00ded-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="00ded-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-128">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="00ded-129">contact</span><span class="sxs-lookup"><span data-stu-id="00ded-129">contact</span></span>](../resources/contact.md) | <span data-ttu-id="00ded-130">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-130">Contacts.ReadWrite</span></span> | <span data-ttu-id="00ded-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="00ded-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-132">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="00ded-133">contactFolder</span><span class="sxs-lookup"><span data-stu-id="00ded-133">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="00ded-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="00ded-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="00ded-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-136">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="00ded-137">event</span><span class="sxs-lookup"><span data-stu-id="00ded-137">event</span></span>](../resources/event.md) | <span data-ttu-id="00ded-138">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-138">Calendars.ReadWrite</span></span> | <span data-ttu-id="00ded-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-139">Calendars.ReadWrite</span></span> |  <span data-ttu-id="00ded-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-140">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="00ded-141">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="00ded-141">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="00ded-142">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ded-142">Group.ReadWrite.All</span></span> | <span data-ttu-id="00ded-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00ded-143">Not supported</span></span> | <span data-ttu-id="00ded-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00ded-144">Not supported</span></span> |
| <span data-ttu-id="00ded-145">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="00ded-145">group [event](../resources/event.md)</span></span> | <span data-ttu-id="00ded-146">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ded-146">Group.ReadWrite.All</span></span> | <span data-ttu-id="00ded-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00ded-147">Not supported</span></span> | <span data-ttu-id="00ded-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00ded-148">Not supported</span></span> |
| <span data-ttu-id="00ded-149">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="00ded-149">group [post](../resources/post.md)</span></span> | <span data-ttu-id="00ded-150">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ded-150">Group.ReadWrite.All</span></span> | <span data-ttu-id="00ded-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00ded-151">Not supported</span></span> | <span data-ttu-id="00ded-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="00ded-152">Not supported</span></span> |
| [<span data-ttu-id="00ded-153">mailFolder</span><span class="sxs-lookup"><span data-stu-id="00ded-153">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="00ded-154">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-154">Mail.ReadWrite</span></span> | <span data-ttu-id="00ded-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-155">Mail.ReadWrite</span></span> | <span data-ttu-id="00ded-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-156">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="00ded-157">message</span><span class="sxs-lookup"><span data-stu-id="00ded-157">message</span></span>](../resources/message.md) | <span data-ttu-id="00ded-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-158">Mail.ReadWrite</span></span> | <span data-ttu-id="00ded-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-159">Mail.ReadWrite</span></span> | <span data-ttu-id="00ded-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00ded-160">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00ded-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00ded-161">HTTP request</span></span>
<span data-ttu-id="00ded-162">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="00ded-162">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="00ded-p102">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_. Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания. Дополнительные сведения о создании этих экземпляров ресурса вы найдете в соответствующих статьях о создании [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md) и [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="00ded-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span>

<span data-ttu-id="00ded-166">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="00ded-166">The following is the syntax of the requests.</span></span>

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

<span data-ttu-id="00ded-167">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="00ded-167">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="00ded-168">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="00ded-168">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="00ded-169">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00ded-169">Request headers</span></span>
| <span data-ttu-id="00ded-170">Имя</span><span class="sxs-lookup"><span data-stu-id="00ded-170">Name</span></span>       | <span data-ttu-id="00ded-171">Значение</span><span class="sxs-lookup"><span data-stu-id="00ded-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="00ded-172">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00ded-172">Authorization</span></span> | <span data-ttu-id="00ded-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00ded-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00ded-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00ded-175">Content-Type</span></span> | <span data-ttu-id="00ded-176">application/json</span><span class="sxs-lookup"><span data-stu-id="00ded-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="00ded-177">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00ded-177">Request body</span></span>

<span data-ttu-id="00ded-178">Предоставьте тело JSON каждого объекта [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) в свойстве коллекции **singleValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="00ded-178">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="00ded-179">Свойство</span><span class="sxs-lookup"><span data-stu-id="00ded-179">Property</span></span>|<span data-ttu-id="00ded-180">Тип</span><span class="sxs-lookup"><span data-stu-id="00ded-180">Type</span></span>|<span data-ttu-id="00ded-181">Описание</span><span class="sxs-lookup"><span data-stu-id="00ded-181">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="00ded-182">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="00ded-182">singleValueExtendedProperties</span></span>|<span data-ttu-id="00ded-183">Коллекция [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="00ded-183">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="00ded-184">Массив из одного или нескольких расширенных свойств с одним значением.</span><span class="sxs-lookup"><span data-stu-id="00ded-184">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="00ded-185">id</span><span class="sxs-lookup"><span data-stu-id="00ded-185">id</span></span>|<span data-ttu-id="00ded-186">String</span><span class="sxs-lookup"><span data-stu-id="00ded-186">String</span></span>|<span data-ttu-id="00ded-p104">Чтобы идентифицировать свойства в коллекции **singleValueExtendedProperties**, для каждого из них укажите этот параметр. Свойство должно быть одного из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="00ded-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="00ded-191">значение</span><span class="sxs-lookup"><span data-stu-id="00ded-191">value</span></span>|<span data-ttu-id="00ded-192">string</span><span class="sxs-lookup"><span data-stu-id="00ded-192">string</span></span>|<span data-ttu-id="00ded-p105">Для каждого свойства из коллекции **singleValueExtendedProperties** следует указать значение. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="00ded-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="00ded-195">При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **singleValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00ded-195">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="00ded-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="00ded-196">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="00ded-197">Код ответа</span><span class="sxs-lookup"><span data-stu-id="00ded-197">Response code</span></span>
<span data-ttu-id="00ded-198">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="00ded-198">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="00ded-199">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="00ded-199">In an existing resource instance, a successful create operation returns `200 OK`.</span></span>


#### <a name="response-body"></a><span data-ttu-id="00ded-200">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="00ded-200">Response body</span></span>

<span data-ttu-id="00ded-p106">При создании расширенного свойства отклик будет включать только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы отобразить только что созданное расширенное свойство, [примените к экземпляру, содержащему это расширенное свойство, параметр $expand](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="00ded-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="00ded-203">Когда вы создаете расширенное свойство в _новом_ экземпляре [group post](../resources/post.md) при ответе на беседу или публикацию, отклик будет включать только код отклика, но не новую публикацию или расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="00ded-203">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="00ded-204">Пример</span><span class="sxs-lookup"><span data-stu-id="00ded-204">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="00ded-205">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="00ded-205">Request 1</span></span>

<span data-ttu-id="00ded-p107">Первый пример показывает создание нового события и расширенного свойства с одним значением с помощью одной и той же операции POST. Помимо свойств, которые вы обычно указываете для нового события, тело запроса включает коллекцию **singleValueExtendedProperties**, которая содержит одно расширенное свойство с одним значением, и следующие данные для этого свойства:</span><span class="sxs-lookup"><span data-stu-id="00ded-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="00ded-208">**id** (указывает тип свойства как `String`), GUID и свойство `Fun`.</span><span class="sxs-lookup"><span data-stu-id="00ded-208">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="00ded-209">**value** (указывает `Food` как значение свойства `Fun`).</span><span class="sxs-lookup"><span data-stu-id="00ded-209">**value** specifies `Food` as the value of the `Fun` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
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

##### <a name="response-1"></a><span data-ttu-id="00ded-210">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="00ded-210">Response 1</span></span>

<span data-ttu-id="00ded-p108">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="00ded-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="00ded-213">Чтобы отобразить только что созданное расширенное свойство, [примените к событию, к которому относится это свойство, параметр $expand](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="00ded-213">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="00ded-214">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="00ded-214">Request 2</span></span>

<span data-ttu-id="00ded-p109">Второй пример показывает создание расширенного свойства с одним значением для указанного существующего сообщения. Это расширенное свойство — единственный элемент в массиве **singleValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="00ded-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="00ded-218">**id** (указывает тип свойства как `String`), GUID и свойство `Color`.</span><span class="sxs-lookup"><span data-stu-id="00ded-218">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="00ded-219">**value** (указывает `Green` как значение свойства `Color`).</span><span class="sxs-lookup"><span data-stu-id="00ded-219">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=

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

##### <a name="response-2"></a><span data-ttu-id="00ded-220">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="00ded-220">Response 2</span></span>

<span data-ttu-id="00ded-p110">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="00ded-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="00ded-223">Чтобы отобразить только что созданное расширенное свойство, [примените к сообщению, к которому относится это свойство, параметр $expand](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="00ded-223">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

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


