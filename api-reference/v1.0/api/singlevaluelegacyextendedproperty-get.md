---
title: Получение объекта singleValueLegacyExtendedProperty
description: Можно получить один экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурса.
localization_priority: Normal
ms.openlocfilehash: c4e028ecd7e881d42ee165560beced4dd097c553
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279256"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="48e71-103">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="48e71-103">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="48e71-104">Вы можете получить отдельный экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурсов, включающую расширенные свойства, которые соответствуют фильтру.</span><span class="sxs-lookup"><span data-stu-id="48e71-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="48e71-105">Параметр запроса `$expand` позволяет получить указанный экземпляр ресурса, дополненный определенным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="48e71-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="48e71-106">Используйте операторы `$filter` и `eq` в свойстве **id**, чтобы указать расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="48e71-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="48e71-107">На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="48e71-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="48e71-108">Чтобы получить экземпляры ресурсов, которые содержат определенные расширенные свойства, используйте параметр запроса `$filter` и примените оператор `eq` к свойству **id**.</span><span class="sxs-lookup"><span data-stu-id="48e71-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="48e71-109">Кроме того, для числовых расширенных свойств примените один из следующих операторов к свойству **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="48e71-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="48e71-110">Для расширенных свойств строкового типа примените оператор `contains`, `startswith`, `eq` или `ne` к свойству **value**.</span><span class="sxs-lookup"><span data-stu-id="48e71-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="48e71-111">Фильтр применяется ко всем экземплярам ресурса в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="48e71-111">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="48e71-112">При фильтрации имени строки (`Name`) в свойстве **id** расширенного свойства учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="48e71-112">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="48e71-113">При фильтрации свойства **value** расширенного свойства регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="48e71-113">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="48e71-114">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="48e71-114">The following user resources are supported:</span></span>

- <span data-ttu-id="48e71-115">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="48e71-115">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="48e71-116">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="48e71-116">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="48e71-117">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="48e71-117">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="48e71-118">event</span><span class="sxs-lookup"><span data-stu-id="48e71-118">event</span></span>](../resources/event.md)
- [<span data-ttu-id="48e71-119">mailFolder</span><span class="sxs-lookup"><span data-stu-id="48e71-119">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="48e71-120">message</span><span class="sxs-lookup"><span data-stu-id="48e71-120">message</span></span>](../resources/message.md) 

<span data-ttu-id="48e71-121">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="48e71-121">As well as the following group resources:</span></span>

- <span data-ttu-id="48e71-122">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="48e71-122">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="48e71-123">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="48e71-123">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="48e71-124">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="48e71-124">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="48e71-125">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="48e71-125">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="48e71-126">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48e71-126">Permissions</span></span>
<span data-ttu-id="48e71-127">В зависимости от ресурса, из которого вы получаете расширенное свойство, а также от запрашиваемого типа разрешения (делегированного или приложения), для вызова этого API требуется минимум разрешение, указанное в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="48e71-127">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="48e71-128">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e71-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48e71-129">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="48e71-129">Supported resource</span></span> | <span data-ttu-id="48e71-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48e71-130">Delegated (work or school account)</span></span> | <span data-ttu-id="48e71-131">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48e71-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48e71-132">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48e71-132">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="48e71-133">calendar</span><span class="sxs-lookup"><span data-stu-id="48e71-133">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="48e71-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-134">Calendars.Read</span></span> | <span data-ttu-id="48e71-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-135">Calendars.Read</span></span> | <span data-ttu-id="48e71-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-136">Calendars.Read</span></span> |
| [<span data-ttu-id="48e71-137">contact</span><span class="sxs-lookup"><span data-stu-id="48e71-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="48e71-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-138">Contacts.Read</span></span> | <span data-ttu-id="48e71-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-139">Contacts.Read</span></span> | <span data-ttu-id="48e71-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-140">Contacts.Read</span></span> |
| <span data-ttu-id="48e71-141">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="48e71-141">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="48e71-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-142">Contacts.Read</span></span> | <span data-ttu-id="48e71-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-143">Contacts.Read</span></span> | <span data-ttu-id="48e71-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-144">Contacts.Read</span></span> |
| [<span data-ttu-id="48e71-145">event</span><span class="sxs-lookup"><span data-stu-id="48e71-145">event</span></span>](../resources/event.md) | <span data-ttu-id="48e71-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-146">Calendars.Read</span></span> | <span data-ttu-id="48e71-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-147">Calendars.Read</span></span> |  <span data-ttu-id="48e71-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-148">Calendars.Read</span></span>|
| <span data-ttu-id="48e71-149">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="48e71-149">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="48e71-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="48e71-150">Group.Read.All</span></span> | <span data-ttu-id="48e71-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48e71-151">Not supported</span></span> | <span data-ttu-id="48e71-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48e71-152">Not supported</span></span> |
| <span data-ttu-id="48e71-153">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="48e71-153">group [event](../resources/event.md)</span></span> | <span data-ttu-id="48e71-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="48e71-154">Group.Read.All</span></span> | <span data-ttu-id="48e71-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48e71-155">Not supported</span></span> | <span data-ttu-id="48e71-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48e71-156">Not supported</span></span> |
| <span data-ttu-id="48e71-157">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="48e71-157">group [post](../resources/post.md)</span></span> | <span data-ttu-id="48e71-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="48e71-158">Group.Read.All</span></span> | <span data-ttu-id="48e71-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="48e71-159">Not supported</span></span> | <span data-ttu-id="48e71-160">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="48e71-160">Group.Read.All</span></span> |
| [<span data-ttu-id="48e71-161">mailFolder</span><span class="sxs-lookup"><span data-stu-id="48e71-161">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="48e71-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-162">Mail.Read</span></span> | <span data-ttu-id="48e71-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-163">Mail.Read</span></span> | <span data-ttu-id="48e71-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-164">Mail.Read</span></span> |
| [<span data-ttu-id="48e71-165">message</span><span class="sxs-lookup"><span data-stu-id="48e71-165">message</span></span>](../resources/message.md) | <span data-ttu-id="48e71-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-166">Mail.Read</span></span> | <span data-ttu-id="48e71-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-167">Mail.Read</span></span> | <span data-ttu-id="48e71-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="48e71-168">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="48e71-169">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48e71-169">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="48e71-170">Получение экземпляра ресурса, дополненного расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="48e71-170">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="48e71-p105">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="48e71-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="48e71-173">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="48e71-173">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="48e71-174">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="48e71-174">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="48e71-175">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="48e71-175">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="48e71-176">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="48e71-176">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="48e71-177">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="48e71-177">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="48e71-178">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="48e71-178">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="48e71-179">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="48e71-179">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="48e71-180">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="48e71-180">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="48e71-181">Получение экземпляров ресурсов с числовыми расширенными свойствами, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="48e71-181">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="48e71-182">Получите экземпляры поддерживаемого ресурса с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="48e71-182">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="48e71-183">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="48e71-183">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="48e71-184">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="48e71-184">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="48e71-185">В приведенных ниже строках синтаксиса показан фильтр, в случае которого один оператор `eq` используется для свойства id, а другой оператор `eq` — для свойства value.</span><span class="sxs-lookup"><span data-stu-id="48e71-185">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="48e71-186">Вы можете заменить оператор `eq` для свойства **value** любым из других операторов (`ne`, `ge`, `gt`, `le` или `lt`), которые применяются к числовым значениям.</span><span class="sxs-lookup"><span data-stu-id="48e71-186">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="48e71-187">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="48e71-187">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="48e71-188">Получение экземпляров объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="48e71-188">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="48e71-189">Список экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="48e71-189">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="48e71-190">Получение экземпляров объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="48e71-190">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="48e71-191">Получение экземпляров объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="48e71-191">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="48e71-192">Получение экземпляров объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="48e71-192">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="48e71-193">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="48e71-193">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="48e71-194">Получение экземпляров объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="48e71-194">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="48e71-195">Получение экземпляров ресурсов с расширенными свойствами строкового типа, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="48e71-195">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="48e71-196">Получите экземпляры ресурса **message** или **event**, которые включают расширенное свойство строкового типа, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="48e71-196">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="48e71-197">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `contains`, `startswith`, `eq` или `ne`.</span><span class="sxs-lookup"><span data-stu-id="48e71-197">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="48e71-198">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="48e71-198">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="48e71-199">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="48e71-199">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="48e71-200">Получение экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="48e71-200">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="48e71-201">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="48e71-201">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="48e71-202">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="48e71-202">Path parameters</span></span>
|<span data-ttu-id="48e71-203">Параметр</span><span class="sxs-lookup"><span data-stu-id="48e71-203">Parameter</span></span>|<span data-ttu-id="48e71-204">Тип</span><span class="sxs-lookup"><span data-stu-id="48e71-204">Type</span></span>|<span data-ttu-id="48e71-205">Описание</span><span class="sxs-lookup"><span data-stu-id="48e71-205">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="48e71-206">id_value</span><span class="sxs-lookup"><span data-stu-id="48e71-206">id_value</span></span>|<span data-ttu-id="48e71-207">String</span><span class="sxs-lookup"><span data-stu-id="48e71-207">String</span></span>|<span data-ttu-id="48e71-p109">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48e71-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="48e71-212">property_value</span><span class="sxs-lookup"><span data-stu-id="48e71-212">property_value</span></span> |<span data-ttu-id="48e71-213">String</span><span class="sxs-lookup"><span data-stu-id="48e71-213">String</span></span>|<span data-ttu-id="48e71-214">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="48e71-214">The value of the extended property to match.</span></span> <span data-ttu-id="48e71-215">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="48e71-215">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="48e71-216">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="48e71-216">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="48e71-217">Примеры см. в разделе [Запрос 4](#request-4).</span><span class="sxs-lookup"><span data-stu-id="48e71-217">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="48e71-218">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48e71-218">Request headers</span></span>
| <span data-ttu-id="48e71-219">Имя</span><span class="sxs-lookup"><span data-stu-id="48e71-219">Name</span></span>      |<span data-ttu-id="48e71-220">Описание</span><span class="sxs-lookup"><span data-stu-id="48e71-220">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48e71-221">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48e71-221">Authorization</span></span>  | <span data-ttu-id="48e71-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48e71-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48e71-224">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48e71-224">Request body</span></span>
<span data-ttu-id="48e71-225">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48e71-225">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48e71-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="48e71-226">Response</span></span>

<span data-ttu-id="48e71-227">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="48e71-227">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="48e71-228">Получение экземпляра ресурса с соответствующим расширенным свойством</span><span class="sxs-lookup"><span data-stu-id="48e71-228">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="48e71-229">Тело отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="48e71-229">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="48e71-230">Получение экземпляров ресурсов с расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="48e71-230">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="48e71-231">Тело отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="48e71-231">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="48e71-232">Тело отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="48e71-232">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="48e71-233">Пример</span><span class="sxs-lookup"><span data-stu-id="48e71-233">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="48e71-234">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="48e71-234">Request 1</span></span>

<span data-ttu-id="48e71-p113">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="48e71-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="48e71-237">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="48e71-237">Response 1</span></span>
<span data-ttu-id="48e71-238">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="48e71-238">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="48e71-p114">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48e71-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="48e71-241">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="48e71-241">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="48e71-242">C#</span><span class="sxs-lookup"><span data-stu-id="48e71-242">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48e71-243">Javascript</span><span class="sxs-lookup"><span data-stu-id="48e71-243">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="48e71-244">Цель — C</span><span class="sxs-lookup"><span data-stu-id="48e71-244">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_singlevaluelegacyextendedproperty_1-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="48e71-245">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="48e71-245">Request 2</span></span>

<span data-ttu-id="48e71-246">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="48e71-246">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="48e71-247">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="48e71-247">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="48e71-248">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="48e71-248">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="48e71-249">его свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="48e71-249">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="48e71-250">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="48e71-250">Response 2</span></span>

<span data-ttu-id="48e71-p116">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user-list-messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="48e71-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="48e71-254">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="48e71-254">Request 3</span></span>

<span data-ttu-id="48e71-255">В третьем примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством строкового типа.</span><span class="sxs-lookup"><span data-stu-id="48e71-255">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="48e71-256">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="48e71-256">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="48e71-257">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="48e71-257">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="48e71-258">его свойство **value** включает строку `green`.</span><span class="sxs-lookup"><span data-stu-id="48e71-258">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="48e71-259">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="48e71-259">Response 3</span></span>

<span data-ttu-id="48e71-260">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а тело отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="48e71-260">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="48e71-261">Например, сообщение, которое содержит однозначное расширенное свойство со свойством **id**, равным строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, и свойством **value**, равным строке `Light green`, будет соответствовать фильтру и включено в отклик.</span><span class="sxs-lookup"><span data-stu-id="48e71-261">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="48e71-262">Тело отклика такое же, как при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="48e71-262">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="48e71-263">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="48e71-263">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="48e71-264">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="48e71-264">Request 4</span></span>

<span data-ttu-id="48e71-265">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от строкового.</span><span class="sxs-lookup"><span data-stu-id="48e71-265">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="48e71-266">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="48e71-266">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="48e71-267">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="48e71-267">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="48e71-268">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="48e71-268">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="48e71-269">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="48e71-269">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="48e71-270">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="48e71-270">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="48e71-271">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="48e71-271">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="48e71-272">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="48e71-272">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="48e71-273">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="48e71-273">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="48e71-274">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="48e71-274">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="48e71-275">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="48e71-275">Response 4</span></span>

<span data-ttu-id="48e71-276">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="48e71-276">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="48e71-277">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="48e71-277">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="48e71-278">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="48e71-278">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/singlevaluelegacyextendedproperty-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
