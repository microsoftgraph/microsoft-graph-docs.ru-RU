---
title: Получение объекта singleValueLegacyExtendedProperty
description: Можно получить один экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурса.
localization_priority: Normal
ms.openlocfilehash: 49df9dcc6142086cead43731243c50911e2a7cc7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520923"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="f2885-103">Получение объекта singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="f2885-103">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="f2885-104">Вы можете получить отдельный экземпляр ресурса, дополненный определенным расширенным свойством, или коллекцию экземпляров ресурсов, включающую расширенные свойства, которые соответствуют фильтру.</span><span class="sxs-lookup"><span data-stu-id="f2885-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="f2885-105">Параметр запроса `$expand` позволяет получить указанный экземпляр ресурса, дополненный определенным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="f2885-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="f2885-106">Используйте операторы `$filter` и `eq` в свойстве **id**, чтобы указать расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="f2885-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="f2885-107">На данный момент это единственный способ получить объект [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="f2885-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="f2885-108">Чтобы получить экземпляры ресурсов, которые содержат определенные расширенные свойства, используйте параметр запроса `$filter` и примените оператор `eq` к свойству **id**.</span><span class="sxs-lookup"><span data-stu-id="f2885-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="f2885-109">Кроме того, для числовых расширенных свойств примените один из следующих операторов к свойству **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="f2885-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="f2885-110">Для расширенных свойств строкового типа примените оператор `contains`, `startswith`, `eq` или `ne` к свойству **value**.</span><span class="sxs-lookup"><span data-stu-id="f2885-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="f2885-111">Фильтр применяется ко всем экземплярам ресурса в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2885-111">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="f2885-112">При фильтрации имени строки (`Name`) в свойстве **id** расширенного свойства учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f2885-112">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="f2885-113">При фильтрации свойства **value** расширенного свойства регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="f2885-113">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="f2885-114">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="f2885-114">The following user resources are supported:</span></span>

- [<span data-ttu-id="f2885-115">calendar</span><span class="sxs-lookup"><span data-stu-id="f2885-115">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="f2885-116">contact</span><span class="sxs-lookup"><span data-stu-id="f2885-116">contact</span></span>](../resources/contact.md)
- <span data-ttu-id="f2885-117">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f2885-117">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="f2885-118">event</span><span class="sxs-lookup"><span data-stu-id="f2885-118">event</span></span>](../resources/event.md)
- <span data-ttu-id="f2885-119">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="f2885-119">[mailFolder](../resources/mailfolder.md)</span></span>
- [<span data-ttu-id="f2885-120">message</span><span class="sxs-lookup"><span data-stu-id="f2885-120">message</span></span>](../resources/message.md) 

<span data-ttu-id="f2885-121">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="f2885-121">As well as the following group resources:</span></span>

- <span data-ttu-id="f2885-122">[calendar](../resources/calendar.md) для групп</span><span class="sxs-lookup"><span data-stu-id="f2885-122">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="f2885-123">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="f2885-123">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="f2885-124">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="f2885-124">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="f2885-125">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="f2885-125">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2885-126">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2885-126">Permissions</span></span>
<span data-ttu-id="f2885-127">В зависимости от ресурса, из которого вы получаете расширенное свойство, а также от запрашиваемого типа разрешения (делегированного или приложения), для вызова этого API требуется минимум разрешение, указанное в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f2885-127">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="f2885-128">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2885-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2885-129">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="f2885-129">Supported resource</span></span> | <span data-ttu-id="f2885-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2885-130">Delegated (work or school account)</span></span> | <span data-ttu-id="f2885-131">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2885-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2885-132">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2885-132">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="f2885-133">calendar</span><span class="sxs-lookup"><span data-stu-id="f2885-133">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="f2885-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-134">Calendars.Read</span></span> | <span data-ttu-id="f2885-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-135">Calendars.Read</span></span> | <span data-ttu-id="f2885-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-136">Calendars.Read</span></span> |
| [<span data-ttu-id="f2885-137">contact</span><span class="sxs-lookup"><span data-stu-id="f2885-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="f2885-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-138">Contacts.Read</span></span> | <span data-ttu-id="f2885-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-139">Contacts.Read</span></span> | <span data-ttu-id="f2885-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-140">Contacts.Read</span></span> |
| <span data-ttu-id="f2885-141">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="f2885-141">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="f2885-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-142">Contacts.Read</span></span> | <span data-ttu-id="f2885-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-143">Contacts.Read</span></span> | <span data-ttu-id="f2885-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-144">Contacts.Read</span></span> |
| [<span data-ttu-id="f2885-145">event</span><span class="sxs-lookup"><span data-stu-id="f2885-145">event</span></span>](../resources/event.md) | <span data-ttu-id="f2885-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-146">Calendars.Read</span></span> | <span data-ttu-id="f2885-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-147">Calendars.Read</span></span> |  <span data-ttu-id="f2885-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-148">Calendars.Read</span></span>|
| <span data-ttu-id="f2885-149">[calendar](../resources/calendar.md) для групп</span><span class="sxs-lookup"><span data-stu-id="f2885-149">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="f2885-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2885-150">Group.Read.All</span></span> | <span data-ttu-id="f2885-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f2885-151">Not supported</span></span> | <span data-ttu-id="f2885-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f2885-152">Not supported</span></span> |
| <span data-ttu-id="f2885-153">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="f2885-153">group [event](../resources/event.md)</span></span> | <span data-ttu-id="f2885-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2885-154">Group.Read.All</span></span> | <span data-ttu-id="f2885-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f2885-155">Not supported</span></span> | <span data-ttu-id="f2885-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f2885-156">Not supported</span></span> |
| <span data-ttu-id="f2885-157">group [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="f2885-157">group [post](../resources/post.md)</span></span> | <span data-ttu-id="f2885-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2885-158">Group.Read.All</span></span> | <span data-ttu-id="f2885-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f2885-159">Not supported</span></span> | <span data-ttu-id="f2885-160">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2885-160">Group.Read.All</span></span> |
| <span data-ttu-id="f2885-161">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="f2885-161">[mailFolder](../resources/mailfolder.md)</span></span> | <span data-ttu-id="f2885-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-162">Mail.Read</span></span> | <span data-ttu-id="f2885-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-163">Mail.Read</span></span> | <span data-ttu-id="f2885-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-164">Mail.Read</span></span> |
| [<span data-ttu-id="f2885-165">message</span><span class="sxs-lookup"><span data-stu-id="f2885-165">message</span></span>](../resources/message.md) | <span data-ttu-id="f2885-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-166">Mail.Read</span></span> | <span data-ttu-id="f2885-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-167">Mail.Read</span></span> | <span data-ttu-id="f2885-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f2885-168">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2885-169">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2885-169">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="f2885-170">Получение экземпляра ресурса, дополненного расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="f2885-170">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="f2885-p105">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="f2885-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="f2885-173">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="f2885-173">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f2885-174">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="f2885-174">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="f2885-175">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="f2885-175">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f2885-176">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="f2885-176">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f2885-177">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="f2885-177">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f2885-178">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="f2885-178">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="f2885-179">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="f2885-179">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="f2885-180">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="f2885-180">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="f2885-181">Получение экземпляров ресурсов с числовыми расширенными свойствами, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="f2885-181">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="f2885-182">Получите экземпляры поддерживаемого ресурса с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="f2885-182">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="f2885-183">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `eq`, `ne`, `ge`, `gt`, `le` или `lt`.</span><span class="sxs-lookup"><span data-stu-id="f2885-183">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="f2885-184">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="f2885-184">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="f2885-185">В приведенных ниже строках синтаксиса показан фильтр, в случае которого один оператор `eq` используется для свойства id, а другой оператор `eq` — для свойства value.</span><span class="sxs-lookup"><span data-stu-id="f2885-185">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="f2885-186">Вы можете заменить оператор `eq` для свойства **value** любым из других операторов (`ne`, `ge`, `gt`, `le` или `lt`), которые применяются к числовым значениям.</span><span class="sxs-lookup"><span data-stu-id="f2885-186">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="f2885-187">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="f2885-187">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="f2885-188">Получение экземпляров объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="f2885-188">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="f2885-189">Список экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="f2885-189">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="f2885-190">Получение экземпляров объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="f2885-190">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="f2885-191">Получение экземпляров объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="f2885-191">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="f2885-192">Получение экземпляров объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="f2885-192">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="f2885-193">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="f2885-193">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="f2885-194">Получение экземпляров объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="f2885-194">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="f2885-195">Получение экземпляров ресурсов с расширенными свойствами строкового типа, которые соответствуют фильтру</span><span class="sxs-lookup"><span data-stu-id="f2885-195">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="f2885-196">Получите экземпляры ресурса **message** или **event**, которые включают расширенное свойство строкового типа, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="f2885-196">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="f2885-197">В случае фильтра используется оператор `eq` для свойства **id**, а также применяется один из следующих операторов для свойства **value**: `contains`, `startswith`, `eq` или `ne`.</span><span class="sxs-lookup"><span data-stu-id="f2885-197">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="f2885-198">Применяйте [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для следующих символов в строке фильтра: двоеточие, косая черта и пробел.</span><span class="sxs-lookup"><span data-stu-id="f2885-198">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="f2885-199">Получение экземпляров объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="f2885-199">Get **message** instances:</span></span>
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

<span data-ttu-id="f2885-200">Получение экземпляров объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="f2885-200">Get **event** instances:</span></span>
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

<span data-ttu-id="f2885-201">Получение экземпляров объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="f2885-201">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="f2885-202">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="f2885-202">Path parameters</span></span>
|<span data-ttu-id="f2885-203">Параметр</span><span class="sxs-lookup"><span data-stu-id="f2885-203">Parameter</span></span>|<span data-ttu-id="f2885-204">Тип</span><span class="sxs-lookup"><span data-stu-id="f2885-204">Type</span></span>|<span data-ttu-id="f2885-205">Описание</span><span class="sxs-lookup"><span data-stu-id="f2885-205">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f2885-206">id_value</span><span class="sxs-lookup"><span data-stu-id="f2885-206">id_value</span></span>|<span data-ttu-id="f2885-207">String</span><span class="sxs-lookup"><span data-stu-id="f2885-207">String</span></span>|<span data-ttu-id="f2885-p109">Идентификатор сопоставляемого расширенного свойства. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2885-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="f2885-212">property_value</span><span class="sxs-lookup"><span data-stu-id="f2885-212">property_value</span></span> |<span data-ttu-id="f2885-213">String</span><span class="sxs-lookup"><span data-stu-id="f2885-213">String</span></span>|<span data-ttu-id="f2885-214">Значение сопоставляемого расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="f2885-214">The value of the extended property to match.</span></span> <span data-ttu-id="f2885-215">Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос** выше.</span><span class="sxs-lookup"><span data-stu-id="f2885-215">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="f2885-216">Если параметр {property_value} не является строкой, явно приведите `ep/value` к правильному типу данных Edm при сравнении с параметром {property_value}.</span><span class="sxs-lookup"><span data-stu-id="f2885-216">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="f2885-217">Примеры см. в разделе [Запрос 4](#request-4).</span><span class="sxs-lookup"><span data-stu-id="f2885-217">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f2885-218">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2885-218">Request headers</span></span>
| <span data-ttu-id="f2885-219">Имя</span><span class="sxs-lookup"><span data-stu-id="f2885-219">Name</span></span>      |<span data-ttu-id="f2885-220">Описание</span><span class="sxs-lookup"><span data-stu-id="f2885-220">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2885-221">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2885-221">Authorization</span></span>  | <span data-ttu-id="f2885-p111">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2885-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2885-224">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2885-224">Request body</span></span>
<span data-ttu-id="f2885-225">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2885-225">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2885-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2885-226">Response</span></span>

<span data-ttu-id="f2885-227">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f2885-227">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="f2885-228">Получение экземпляра ресурса с соответствующим расширенным свойством</span><span class="sxs-lookup"><span data-stu-id="f2885-228">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="f2885-229">Тело отклика содержит объект, который представляет запрашиваемый экземпляр ресурса, дополненный соответствующим объектом [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="f2885-229">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="f2885-230">Получение экземпляров ресурсов с расширенным свойством, которое соответствует фильтру</span><span class="sxs-lookup"><span data-stu-id="f2885-230">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="f2885-231">Тело отклика содержит один или несколько объектов, представляющих экземпляры ресурсов, которые содержат соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="f2885-231">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="f2885-232">Тело отклика не включает расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="f2885-232">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="f2885-233">Пример</span><span class="sxs-lookup"><span data-stu-id="f2885-233">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="f2885-234">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="f2885-234">Request 1</span></span>

<span data-ttu-id="f2885-p113">В первом примере показано, как получить указанное сообщение и дополнить его расширенным свойством с одним значением. Фильтр возвращает расширенное свойство, значение **id** которого совпадает со строкой `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL).</span><span class="sxs-lookup"><span data-stu-id="f2885-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="f2885-237">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="f2885-237">Response 1</span></span>
<span data-ttu-id="f2885-238">Текст отклика включает все свойства указанного сообщения и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="f2885-238">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="f2885-p114">Примечание. Показанный здесь объект **message** усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2885-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="f2885-241">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="f2885-241">Request 2</span></span>

<span data-ttu-id="f2885-242">Во втором примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством типа string.</span><span class="sxs-lookup"><span data-stu-id="f2885-242">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="f2885-243">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="f2885-243">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="f2885-244">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="f2885-244">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="f2885-245">его свойство **value** равно строке `Green`.</span><span class="sxs-lookup"><span data-stu-id="f2885-245">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="f2885-246">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="f2885-246">Response 2</span></span>

<span data-ttu-id="f2885-p116">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а текст отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру. Текст отклика аналогичен отклику при [получении коллекции сообщений](../api/user-list-messages.md). Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="f2885-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="f2885-250">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="f2885-250">Request 3</span></span>

<span data-ttu-id="f2885-251">В третьем примере показано, как получить сообщения с указанным в фильтре однозначным расширенным свойством строкового типа.</span><span class="sxs-lookup"><span data-stu-id="f2885-251">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="f2885-252">Фильтр ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="f2885-252">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="f2885-253">его свойство **id** соответствует строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (для наглядности здесь убрана кодировка URL-адреса);</span><span class="sxs-lookup"><span data-stu-id="f2885-253">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="f2885-254">его свойство **value** включает строку `green`.</span><span class="sxs-lookup"><span data-stu-id="f2885-254">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="f2885-255">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="f2885-255">Response 3</span></span>

<span data-ttu-id="f2885-256">В случае успешного выполнения возвращается код отклика `HTTP 200 OK`, а тело отклика включает все свойства сообщений, у которых есть расширенное свойство, соответствующее фильтру.</span><span class="sxs-lookup"><span data-stu-id="f2885-256">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="f2885-257">Например, сообщение, которое содержит однозначное расширенное свойство со свойством **id**, равным строке `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, и свойством **value**, равным строке `Light green`, будет соответствовать фильтру и включено в отклик.</span><span class="sxs-lookup"><span data-stu-id="f2885-257">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="f2885-258">Тело отклика такое же, как при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="f2885-258">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="f2885-259">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="f2885-259">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="f2885-260">Запрос 4</span><span class="sxs-lookup"><span data-stu-id="f2885-260">Request 4</span></span>

<span data-ttu-id="f2885-261">В следующих двух примерах показано, как получить сообщения с однозначными расширенными свойствами типа, отличного от строкового.</span><span class="sxs-lookup"><span data-stu-id="f2885-261">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="f2885-262">Необходимая кодировка URL не указана для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="f2885-262">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="f2885-263">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="f2885-263">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="f2885-264">Свойство **id** соответствует строке `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="f2885-264">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="f2885-265">Свойство **value** равно GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="f2885-265">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="f2885-266">Чтобы сравнить значение свойства с GUID, приведите `ep/value` к `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="f2885-266">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="f2885-267">В следующем примере показан фильтр, который ищет расширенное свойство со следующими параметрами:</span><span class="sxs-lookup"><span data-stu-id="f2885-267">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="f2885-268">Свойство **id** соответствует строке `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="f2885-268">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="f2885-269">Свойство **value** равно целому числу 12.</span><span class="sxs-lookup"><span data-stu-id="f2885-269">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="f2885-270">Чтобы сравнить значение свойства с целым числом, приведите `ep/value` к `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="f2885-270">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="f2885-271">Отклик 4</span><span class="sxs-lookup"><span data-stu-id="f2885-271">Response 4</span></span>

<span data-ttu-id="f2885-272">В предыдущих двух примерах в случае успешного выполнения возвращается код ответа `HTTP 200 OK`, а текст ответа включает все свойства сообщений с расширенным свойством, соответствующим фильтру.</span><span class="sxs-lookup"><span data-stu-id="f2885-272">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="f2885-273">Текст ответа аналогичен ответу при [получении коллекции сообщений](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="f2885-273">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="f2885-274">Отклик не включает соответствующее расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="f2885-274">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
