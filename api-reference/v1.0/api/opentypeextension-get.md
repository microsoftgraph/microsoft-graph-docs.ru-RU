---
title: Получение открытого расширения
description: Получение открытого расширения (объекта openTypeExtension), указанного по имени или полному имени.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 5e861c038a6baa28e820775e4c0030a25e9095ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063102"
---
# <a name="get-open-extension"></a><span data-ttu-id="7cf5a-103">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="7cf5a-103">Get open extension</span></span>

<span data-ttu-id="7cf5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cf5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cf5a-105">Получение открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)), определенного по имени или полному имени.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-105">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="7cf5a-106">В приведенной ниже таблице перечислены три сценария, согласно которым можно получить открытое расширение из поддерживаемого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-106">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="7cf5a-107">**Сценарий GET**</span><span class="sxs-lookup"><span data-stu-id="7cf5a-107">**GET scenario**</span></span>|<span data-ttu-id="7cf5a-108">**Поддерживаемые ресурсы**</span><span class="sxs-lookup"><span data-stu-id="7cf5a-108">**Supported resources**</span></span>|<span data-ttu-id="7cf5a-109">**Текст ответа**</span><span class="sxs-lookup"><span data-stu-id="7cf5a-109">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7cf5a-110">Получение определенного расширения из экземпляра известного ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-110">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="7cf5a-111">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="7cf5a-111">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="7cf5a-112">Только открытое расширение.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-112">Open extension only.</span></span>|
|<span data-ttu-id="7cf5a-113">Получение экземпляра известного ресурса, дополненного определенным расширением.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-113">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="7cf5a-114">Device, event, group, group event, group post, message, organization, personal contact, user</span><span class="sxs-lookup"><span data-stu-id="7cf5a-114">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="7cf5a-115">Экземпляр известного ресурса, дополненный открытым расширением.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-115">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="7cf5a-116">Поиск экземпляров ресурсов и их дополнение определенным расширением.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-116">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="7cf5a-117">Event, group event, group post, message, personal contact</span><span class="sxs-lookup"><span data-stu-id="7cf5a-117">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="7cf5a-118">Экземпляры ресурса, дополненные открытым расширением.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-118">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="7cf5a-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cf5a-119">Permissions</span></span>

<span data-ttu-id="7cf5a-120">В зависимости от того, какой ресурс содержит расширение, и типа запрашиваемого расширения (делегированного или для приложений), разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-120">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7cf5a-121">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf5a-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7cf5a-122">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="7cf5a-122">Supported resource</span></span> | <span data-ttu-id="7cf5a-123">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cf5a-123">Delegated (work or school account)</span></span> | <span data-ttu-id="7cf5a-124">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cf5a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cf5a-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cf5a-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="7cf5a-126">device</span><span class="sxs-lookup"><span data-stu-id="7cf5a-126">device</span></span>](../resources/device.md) | <span data-ttu-id="7cf5a-127">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-127">Directory.Read.All</span></span> | <span data-ttu-id="7cf5a-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cf5a-128">Not supported</span></span> | <span data-ttu-id="7cf5a-129">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-129">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="7cf5a-130">event</span><span class="sxs-lookup"><span data-stu-id="7cf5a-130">event</span></span>](../resources/event.md) | <span data-ttu-id="7cf5a-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-131">Calendars.Read</span></span> | <span data-ttu-id="7cf5a-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-132">Calendars.Read</span></span> | <span data-ttu-id="7cf5a-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-133">Calendars.Read</span></span> |
| [<span data-ttu-id="7cf5a-134">group</span><span class="sxs-lookup"><span data-stu-id="7cf5a-134">group</span></span>](../resources/group.md) | <span data-ttu-id="7cf5a-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-135">Group.Read.All</span></span> | <span data-ttu-id="7cf5a-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cf5a-136">Not supported</span></span> | <span data-ttu-id="7cf5a-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-137">Group.Read.All</span></span> |
| [<span data-ttu-id="7cf5a-138">Событие для групп</span><span class="sxs-lookup"><span data-stu-id="7cf5a-138">group event</span></span>](../resources/event.md) | <span data-ttu-id="7cf5a-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-139">Group.Read.All</span></span> | <span data-ttu-id="7cf5a-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cf5a-140">Not supported</span></span> | <span data-ttu-id="7cf5a-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cf5a-141">Not supported</span></span> |
| <span data-ttu-id="7cf5a-142">[post](../resources/post.md) для групп</span><span class="sxs-lookup"><span data-stu-id="7cf5a-142">[group post](../resources/post.md)</span></span> | <span data-ttu-id="7cf5a-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-143">Group.Read.All</span></span> | <span data-ttu-id="7cf5a-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cf5a-144">Not supported</span></span> | <span data-ttu-id="7cf5a-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-145">Group.Read.All</span></span> |
| [<span data-ttu-id="7cf5a-146">message</span><span class="sxs-lookup"><span data-stu-id="7cf5a-146">message</span></span>](../resources/message.md) | <span data-ttu-id="7cf5a-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-147">Mail.Read</span></span> | <span data-ttu-id="7cf5a-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-148">Mail.Read</span></span> | <span data-ttu-id="7cf5a-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-149">Mail.Read</span></span> | 
| [<span data-ttu-id="7cf5a-150">organization</span><span class="sxs-lookup"><span data-stu-id="7cf5a-150">organization</span></span>](../resources/organization.md) | <span data-ttu-id="7cf5a-151">User.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-151">User.Read</span></span> | <span data-ttu-id="7cf5a-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7cf5a-152">Not supported</span></span> | <span data-ttu-id="7cf5a-153">Organization.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-153">Organization.Read.All</span></span> |
| <span data-ttu-id="7cf5a-154">[contact](../resources/contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="7cf5a-154">[personal contact](../resources/contact.md)</span></span> | <span data-ttu-id="7cf5a-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-155">Contacts.Read</span></span> | <span data-ttu-id="7cf5a-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-156">Contacts.Read</span></span> | <span data-ttu-id="7cf5a-157">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-157">Contacts.Read</span></span> |
| [<span data-ttu-id="7cf5a-158">user</span><span class="sxs-lookup"><span data-stu-id="7cf5a-158">user</span></span>](../resources/user.md) | <span data-ttu-id="7cf5a-159">User.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-159">User.Read</span></span> | <span data-ttu-id="7cf5a-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="7cf5a-160">User.Read</span></span> | <span data-ttu-id="7cf5a-161">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cf5a-161">User.Read.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="7cf5a-162">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cf5a-162">HTTP request</span></span>

<span data-ttu-id="7cf5a-163">В этом разделе указан синтаксис для каждого из трех перечисленных выше сценариев с `GET`.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-163">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="7cf5a-164">Получение определенного расширения в известном экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="7cf5a-164">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="7cf5a-165">Используйте такой же запрос REST, что и при получении экземпляра ресурса, и определите расширение с помощью свойства навигации **extensions** этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-165">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

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
```


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="7cf5a-166">Получение известного экземпляра ресурса с соответствующим расширением</span><span class="sxs-lookup"><span data-stu-id="7cf5a-166">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="7cf5a-167">Для типов ресурса, таких как event, group event, group post, message, personal contact, можно использовать такой же запрос REST, что и при получении экземпляра ресурса. Найдите расширение, соответствующее заданному свойству **id**, и дополните экземпляр расширением.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-167">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="7cf5a-168">Отклик включает большинство свойств ресурса.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-168">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="7cf5a-169">Для типов ресурса device, group, organization и user также необходимо использовать параметр `$select`, чтобы включить свойство **id** и другие свойства, которые необходимо получить из экземпляра ресурса:</span><span class="sxs-lookup"><span data-stu-id="7cf5a-169">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="7cf5a-170">Фильтрация экземпляров ресурсов с соответствующим расширением</span><span class="sxs-lookup"><span data-stu-id="7cf5a-170">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="7cf5a-171">Используйте такой же запрос REST, что и при получении коллекции поддерживаемого ресурса, отфильтруйте в коллекции экземпляры, содержащие расширение с соответствующим свойством **id**, и дополните эти экземпляры расширением.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-171">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="7cf5a-172">**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения коллекции или экземпляров ресурсов, чье расширение нужно получить.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-172">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it.</span></span> <span data-ttu-id="7cf5a-173">Все другие варианты синтаксиса, позволяющие определить эти коллекции или экземпляры ресурсов, поддерживают получение открытых расширений этих экземпляров или коллекций подобным образом.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-173">All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="7cf5a-174">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="7cf5a-174">Path parameters</span></span>
|<span data-ttu-id="7cf5a-175">Параметр</span><span class="sxs-lookup"><span data-stu-id="7cf5a-175">Parameter</span></span>|<span data-ttu-id="7cf5a-176">Тип</span><span class="sxs-lookup"><span data-stu-id="7cf5a-176">Type</span></span>|<span data-ttu-id="7cf5a-177">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf5a-177">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7cf5a-178">Id</span><span class="sxs-lookup"><span data-stu-id="7cf5a-178">Id</span></span>|<span data-ttu-id="7cf5a-179">string</span><span class="sxs-lookup"><span data-stu-id="7cf5a-179">string</span></span>|<span data-ttu-id="7cf5a-p104">Заполнитель уникального идентификатора для объекта в соответствующей коллекции, например сообщения, события или контакта. Обязательный. Не следует путать его со свойством **id** объекта **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="7cf5a-183">extensionId</span><span class="sxs-lookup"><span data-stu-id="7cf5a-183">extensionId</span></span>|<span data-ttu-id="7cf5a-184">string</span><span class="sxs-lookup"><span data-stu-id="7cf5a-184">string</span></span>|<span data-ttu-id="7cf5a-p105">Заполнитель имени расширения, которое представляет собой уникальный текстовый идентификатор для расширения, либо полного имени, в котором сцеплены тип расширения и уникальный текстовый идентификатор. Полное имя возвращается в свойстве **id** при создании расширения. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="7cf5a-188">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7cf5a-188">Optional query parameters</span></span>

<span data-ttu-id="7cf5a-189">Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-189">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="7cf5a-190">Параметр</span><span class="sxs-lookup"><span data-stu-id="7cf5a-190">Parameter</span></span>|<span data-ttu-id="7cf5a-191">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf5a-191">Description</span></span>|<span data-ttu-id="7cf5a-192">Пример</span><span class="sxs-lookup"><span data-stu-id="7cf5a-192">Example</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="7cf5a-193">$filter</span><span class="sxs-lookup"><span data-stu-id="7cf5a-193">$filter</span></span>|<span data-ttu-id="7cf5a-194">Возвращает расширение, свойство **id** которого совпадает со значением параметра `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-194">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="7cf5a-195">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="7cf5a-195">Request 3</span></span>](#request-3)|
|<span data-ttu-id="7cf5a-196">$filter с **любым** оператором</span><span class="sxs-lookup"><span data-stu-id="7cf5a-196">$filter with **any** operator</span></span>|<span data-ttu-id="7cf5a-197">Возвращает экземпляры коллекции ресурсов, содержащие расширение, свойство **id** которого совпадает со значением параметра `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-197">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="7cf5a-198">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="7cf5a-198">Request 5</span></span>](#request-5)|
|<span data-ttu-id="7cf5a-199">$expand</span><span class="sxs-lookup"><span data-stu-id="7cf5a-199">$expand</span></span>|<span data-ttu-id="7cf5a-200">Дополняет экземпляр ресурса расширением.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-200">Expands a resource instance to include an extension.</span></span> |<span data-ttu-id="7cf5a-201">[Запрос 3](#request-3) и [запрос 5](#request-5)</span><span class="sxs-lookup"><span data-stu-id="7cf5a-201">[Request 3](#request-3) and [request 5](#request-5)</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7cf5a-202">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cf5a-202">Request headers</span></span>
| <span data-ttu-id="7cf5a-203">Имя</span><span class="sxs-lookup"><span data-stu-id="7cf5a-203">Name</span></span>       | <span data-ttu-id="7cf5a-204">Значение</span><span class="sxs-lookup"><span data-stu-id="7cf5a-204">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7cf5a-205">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7cf5a-205">Authorization</span></span> | <span data-ttu-id="7cf5a-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cf5a-208">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cf5a-208">Request body</span></span>
<span data-ttu-id="7cf5a-209">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cf5a-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cf5a-210">Response</span></span>

<span data-ttu-id="7cf5a-p107">В случае успеха этот метод возвращает код отклика `200 OK` и объект [openTypeExtension](../resources/opentypeextension.md) в тексте отклика. Точный текст отклика зависит от запроса GET.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="7cf5a-213">Пример</span><span class="sxs-lookup"><span data-stu-id="7cf5a-213">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="7cf5a-214">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="7cf5a-214">Request 1</span></span>

<span data-ttu-id="7cf5a-p108">В первом примере показаны 2 способа обращения к расширению и получение расширения в указанном сообщении. Отклик не зависит от того, как вы ссылаетесь на расширение.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="7cf5a-217">По имени:</span><span class="sxs-lookup"><span data-stu-id="7cf5a-217">First, by its name:</span></span> 


# <a name="http"></a>[<span data-ttu-id="7cf5a-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf5a-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="7cf5a-219">C#</span><span class="sxs-lookup"><span data-stu-id="7cf5a-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cf5a-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cf5a-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cf5a-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cf5a-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cf5a-222">Java</span><span class="sxs-lookup"><span data-stu-id="7cf5a-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="7cf5a-223">По идентификатору (полному имени):</span><span class="sxs-lookup"><span data-stu-id="7cf5a-223">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="7cf5a-224">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="7cf5a-224">Response 1</span></span>
<span data-ttu-id="7cf5a-225">Ниже представлен отклик для первого примера.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-225">Here is the response for the first example.</span></span>
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


#### <a name="request-2"></a><span data-ttu-id="7cf5a-226">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="7cf5a-226">Request 2</span></span>

<span data-ttu-id="7cf5a-227">Во втором примере показано, как сослаться на расширение по его имени и получить расширение в указанном событии группы.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-227">The second example references an extension by its name and gets the extension in the specified group event.</span></span>


# <a name="http"></a>[<span data-ttu-id="7cf5a-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf5a-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```
# <a name="c"></a>[<span data-ttu-id="7cf5a-229">C#</span><span class="sxs-lookup"><span data-stu-id="7cf5a-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cf5a-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cf5a-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cf5a-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cf5a-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cf5a-232">Java</span><span class="sxs-lookup"><span data-stu-id="7cf5a-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="7cf5a-233">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="7cf5a-233">Response 2</span></span>

<span data-ttu-id="7cf5a-234">Ниже представлен отклик из второго примера.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-234">Here is the response from the second example.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="7cf5a-235">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="7cf5a-235">Request 3</span></span>

<span data-ttu-id="7cf5a-p109">В третьем примере показано, как получить и дополнить указанное сообщение, добавив расширение, возвращенное из фильтра. Фильтр возвращает расширение, свойство **id** которого совпадает с полным именем.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>


# <a name="http"></a>[<span data-ttu-id="7cf5a-238">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf5a-238">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```
# <a name="c"></a>[<span data-ttu-id="7cf5a-239">C#</span><span class="sxs-lookup"><span data-stu-id="7cf5a-239">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cf5a-240">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cf5a-240">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cf5a-241">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cf5a-241">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cf5a-242">Java</span><span class="sxs-lookup"><span data-stu-id="7cf5a-242">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response-3"></a><span data-ttu-id="7cf5a-243">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="7cf5a-243">Response 3</span></span>

<span data-ttu-id="7cf5a-p110">Ниже представлен отклик из третьего примера. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

#### <a name="request-4"></a><span data-ttu-id="7cf5a-247">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="7cf5a-247">Request 4</span></span>

<span data-ttu-id="7cf5a-248">В четвертом примере показано, как сослаться на расширение по его полному имени и получить расширение в указанной записи группы.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-248">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```

#### <a name="response-4"></a><span data-ttu-id="7cf5a-249">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="7cf5a-249">Response 4</span></span>

<span data-ttu-id="7cf5a-250">Ниже представлен отклик из четвертого примера.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-250">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "ignored",
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


#### <a name="request-5"></a><span data-ttu-id="7cf5a-251">Запрос 5</span><span class="sxs-lookup"><span data-stu-id="7cf5a-251">Request 5</span></span>

<span data-ttu-id="7cf5a-p111">В пятом примере показано, как найти в почтовом ящике вошедшего пользователя сообщения с расширениями, соответствующими фильтру, и дополнить их расширением. Фильтр возвращает расширения, свойство **id** которых совпадает с именем расширения `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="7cf5a-254">Отклик 5</span><span class="sxs-lookup"><span data-stu-id="7cf5a-254">Response 5</span></span>

<span data-ttu-id="7cf5a-255">В этом отклике для пятого примера почтовый ящик пользователя содержит только одно сообщение, свойство **id** которого имеет значение `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-255">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="7cf5a-p112">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7cf5a-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

