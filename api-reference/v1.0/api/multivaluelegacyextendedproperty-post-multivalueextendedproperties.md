---
title: Создание расширенного свойства с несколькими значениями
description: 'Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса. '
localization_priority: Normal
ms.openlocfilehash: ded36690cdbe684f78bed6af6aee9dba0b09854d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560993"
---
# <a name="create-multi-value-extended-property"></a><span data-ttu-id="be447-103">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="be447-103">Create multi-value extended property</span></span>

<span data-ttu-id="be447-104">Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="be447-104">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="be447-105">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="be447-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="be447-106">calendar</span><span class="sxs-lookup"><span data-stu-id="be447-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="be447-107">contact</span><span class="sxs-lookup"><span data-stu-id="be447-107">contact</span></span>](../resources/contact.md)
- <span data-ttu-id="be447-108">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="be447-108">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="be447-109">event</span><span class="sxs-lookup"><span data-stu-id="be447-109">event</span></span>](../resources/event.md)
- <span data-ttu-id="be447-110">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="be447-110">[mailFolder](../resources/mailfolder.md)</span></span>
- [<span data-ttu-id="be447-111">message</span><span class="sxs-lookup"><span data-stu-id="be447-111">message</span></span>](../resources/message.md)

<span data-ttu-id="be447-112">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="be447-112">As well as the following group resources:</span></span>

- <span data-ttu-id="be447-113">[calendar](../resources/calendar.md) для групп</span><span class="sxs-lookup"><span data-stu-id="be447-113">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="be447-114">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="be447-114">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="be447-115">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="be447-115">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="be447-116">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="be447-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="be447-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be447-117">Permissions</span></span>
<span data-ttu-id="be447-118">В зависимости от ресурса, в котором вы создаете расширенное свойство и запрашивается тип разрешения (делегированное или приложение), разрешение, указанное в следующей таблице, является минимальным необходимым условием для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="be447-118">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="be447-119">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be447-119">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be447-120">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="be447-120">Supported resource</span></span> | <span data-ttu-id="be447-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be447-121">Delegated (work or school account)</span></span> | <span data-ttu-id="be447-122">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be447-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be447-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be447-123">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="be447-124">calendar</span><span class="sxs-lookup"><span data-stu-id="be447-124">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="be447-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-125">Calendars.ReadWrite</span></span> | <span data-ttu-id="be447-126">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-126">Calendars.ReadWrite</span></span> | <span data-ttu-id="be447-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-127">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="be447-128">contact</span><span class="sxs-lookup"><span data-stu-id="be447-128">contact</span></span>](../resources/contact.md) | <span data-ttu-id="be447-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-129">Contacts.ReadWrite</span></span> | <span data-ttu-id="be447-130">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-130">Contacts.ReadWrite</span></span> | <span data-ttu-id="be447-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-131">Contacts.ReadWrite</span></span> |
| <span data-ttu-id="be447-132">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="be447-132">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="be447-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="be447-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="be447-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-135">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="be447-136">event</span><span class="sxs-lookup"><span data-stu-id="be447-136">event</span></span>](../resources/event.md) | <span data-ttu-id="be447-137">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-137">Calendars.ReadWrite</span></span> | <span data-ttu-id="be447-138">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-138">Calendars.ReadWrite</span></span> |  <span data-ttu-id="be447-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-139">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="be447-140">[calendar](../resources/calendar.md) для групп</span><span class="sxs-lookup"><span data-stu-id="be447-140">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="be447-141">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be447-141">Group.ReadWrite.All</span></span> | <span data-ttu-id="be447-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be447-142">Not supported</span></span> | <span data-ttu-id="be447-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be447-143">Not supported</span></span> |
| <span data-ttu-id="be447-144">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="be447-144">group [event](../resources/event.md)</span></span> | <span data-ttu-id="be447-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be447-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="be447-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be447-146">Not supported</span></span> | <span data-ttu-id="be447-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be447-147">Not supported</span></span> |
| <span data-ttu-id="be447-148">group [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="be447-148">group [post](../resources/post.md)</span></span> | <span data-ttu-id="be447-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be447-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="be447-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be447-150">Not supported</span></span> | <span data-ttu-id="be447-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be447-151">Not supported</span></span> |
| <span data-ttu-id="be447-152">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="be447-152">[mailFolder](../resources/mailfolder.md)</span></span> | <span data-ttu-id="be447-153">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-153">Mail.ReadWrite</span></span> | <span data-ttu-id="be447-154">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-154">Mail.ReadWrite</span></span> | <span data-ttu-id="be447-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-155">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="be447-156">message</span><span class="sxs-lookup"><span data-stu-id="be447-156">message</span></span>](../resources/message.md) | <span data-ttu-id="be447-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-157">Mail.ReadWrite</span></span> | <span data-ttu-id="be447-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-158">Mail.ReadWrite</span></span> | <span data-ttu-id="be447-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be447-159">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be447-160">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be447-160">HTTP request</span></span>
<span data-ttu-id="be447-161">Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="be447-161">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="be447-p102">Чтобы создать одно или несколько расширенных свойств в _новом_ экземпляре ресурса, используйте тот же запрос REST, что и при создании этого экземпляра, включив в тело запроса свойства нового экземпляра ресурса _и расширенное свойство_. Обратите внимание, что некоторые ресурсы поддерживают несколько способов создания. Дополнительные сведения о создании этих экземпляров ресурса вы найдете в соответствующих статьях о создании [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md) и [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="be447-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="be447-165">Ниже приведен синтаксис запросов.</span><span class="sxs-lookup"><span data-stu-id="be447-165">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="be447-166">Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.</span><span class="sxs-lookup"><span data-stu-id="be447-166">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="be447-167">**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="be447-167">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="be447-168">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be447-168">Request headers</span></span>
| <span data-ttu-id="be447-169">Имя</span><span class="sxs-lookup"><span data-stu-id="be447-169">Name</span></span>       | <span data-ttu-id="be447-170">Значение</span><span class="sxs-lookup"><span data-stu-id="be447-170">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="be447-171">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be447-171">Authorization</span></span> | <span data-ttu-id="be447-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be447-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be447-174">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be447-174">Content-Type</span></span> | <span data-ttu-id="be447-175">application/json</span><span class="sxs-lookup"><span data-stu-id="be447-175">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="be447-176">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be447-176">Request body</span></span>

<span data-ttu-id="be447-177">Предоставьте тело в формате JSON для каждого объекта [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) в свойстве коллекции **multiValueExtendedProperties** для экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="be447-177">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="be447-178">Свойство</span><span class="sxs-lookup"><span data-stu-id="be447-178">Property</span></span>|<span data-ttu-id="be447-179">Тип</span><span class="sxs-lookup"><span data-stu-id="be447-179">Type</span></span>|<span data-ttu-id="be447-180">Описание</span><span class="sxs-lookup"><span data-stu-id="be447-180">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="be447-181">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="be447-181">multiValueExtendedProperties</span></span>|<span data-ttu-id="be447-182">Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="be447-182">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="be447-183">Массив из одного или нескольких многозначных расширенных свойств.</span><span class="sxs-lookup"><span data-stu-id="be447-183">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="be447-184">id</span><span class="sxs-lookup"><span data-stu-id="be447-184">id</span></span>|<span data-ttu-id="be447-185">String</span><span class="sxs-lookup"><span data-stu-id="be447-185">String</span></span>|<span data-ttu-id="be447-p104">Чтобы идентифицировать свойства в коллекции **multiValueExtendedProperties**, укажите этот параметр для каждого из них. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="be447-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="be447-190">значение</span><span class="sxs-lookup"><span data-stu-id="be447-190">value</span></span>|<span data-ttu-id="be447-191">string</span><span class="sxs-lookup"><span data-stu-id="be447-191">string</span></span>|<span data-ttu-id="be447-p105">Укажите значение для каждого свойства в коллекции **multiValueExtendedProperties**. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="be447-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="be447-194">При создании расширенного свойства в _новом_ экземпляре ресурса, в дополнение к новой коллекции **multiValueExtendedProperties** , необходимо также предоставить представление этого экземпляра ресурса в формате JSON ( [сообщение](../resources/message.md), [mailFolder ](../resources/mailfolder.md), [событие](../resources/event.md)и т. д.).</span><span class="sxs-lookup"><span data-stu-id="be447-194">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance as well (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.).</span></span>


## <a name="response"></a><span data-ttu-id="be447-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="be447-195">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="be447-196">Код ответа</span><span class="sxs-lookup"><span data-stu-id="be447-196">Response code</span></span>
<span data-ttu-id="be447-197">В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).</span><span class="sxs-lookup"><span data-stu-id="be447-197">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="be447-198">В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="be447-198">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="be447-199">Текст отклика</span><span class="sxs-lookup"><span data-stu-id="be447-199">Response body</span></span>

<span data-ttu-id="be447-p106">При создании расширенного свойства в поддерживаемом ресурсе, отличном от [post для групп](../resources/post.md), отклик включает только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы просмотреть только что созданное расширенное свойство, [разверните экземпляр с этим свойством](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="be447-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="be447-p107">При создании расширенного свойства в _новом_ экземпляре post для групп отклик включает только код отклика и не содержит ни новой записи, ни расширенного свойства. Расширенное свойство невозможно создать в существующем экземпляре post для групп.</span><span class="sxs-lookup"><span data-stu-id="be447-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="be447-204">Пример</span><span class="sxs-lookup"><span data-stu-id="be447-204">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="be447-205">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="be447-205">Request 1</span></span>

<span data-ttu-id="be447-p108">В первом примере в новом экземпляре event создается многозначное расширенное свойство с помощью одной операции POST. Помимо свойств, которые обычно указываются для нового события, тело запроса включает коллекцию **multiValueExtendedProperties**, которая содержит одно расширенное свойство. Тело запроса включает следующие данные для многозначного расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="be447-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="be447-209">**id**. Задает свойство в виде массива строк с заданным идентификатором GUID и именем `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="be447-209">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="be447-210">**value**. Задает `Recreation` в виде массива из 3 строковых значений, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="be447-210">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

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

##### <a name="response-1"></a><span data-ttu-id="be447-211">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="be447-211">Response 1</span></span>

<span data-ttu-id="be447-p109">Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="be447-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="be447-214">Чтобы отобразить только что созданное расширенное свойство, [примените к событию, к которому относится это свойство, параметр $expand](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="be447-214">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="be447-215">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="be447-215">Request 2</span></span>

<span data-ttu-id="be447-p110">Во втором примере создается многозначное расширенное свойство для указанного сообщения. Это расширенное свойство — единственный элемент в коллекции **multiValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:</span><span class="sxs-lookup"><span data-stu-id="be447-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="be447-219">**id**. Задает свойство в виде массива строк с указанным идентификатором GUID и именем `Palette`.</span><span class="sxs-lookup"><span data-stu-id="be447-219">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="be447-220">**value**. Задает `Palette` в виде массива 3 строковых значений, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="be447-220">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="be447-221">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="be447-221">Response 2</span></span>

<span data-ttu-id="be447-p111">Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="be447-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="be447-224">Чтобы отобразить только что созданное расширенное свойство, [примените к сообщению, к которому относится это свойство, параметр $expand](../api/multivaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="be447-224">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty-get.md).</span></span>


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




