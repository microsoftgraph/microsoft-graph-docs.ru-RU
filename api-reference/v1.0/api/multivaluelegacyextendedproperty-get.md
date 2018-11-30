---
title: Получение объекта multiValueLegacyExtendedProperty
description: Разверните узел ".
ms.openlocfilehash: c56afa8492954bcb68c5f36df00abdfce51cc2b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027909"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="9e22b-103">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9e22b-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="9e22b-104">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="9e22b-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="9e22b-105">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="9e22b-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="9e22b-106">Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="9e22b-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="9e22b-107">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="9e22b-107">The following user resources are supported:</span></span>

- <span data-ttu-id="9e22b-108">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="9e22b-108">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="9e22b-109">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="9e22b-109">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="9e22b-110">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9e22b-110">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="9e22b-111">событие</span><span class="sxs-lookup"><span data-stu-id="9e22b-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="9e22b-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="9e22b-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="9e22b-113">message</span><span class="sxs-lookup"><span data-stu-id="9e22b-113">message</span></span>](../resources/message.md) 

<span data-ttu-id="9e22b-114">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="9e22b-114">As well as the following group resources:</span></span>

- <span data-ttu-id="9e22b-115">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="9e22b-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="9e22b-116">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="9e22b-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="9e22b-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="9e22b-117">group [post](../resources/post.md)</span></span>

<span data-ttu-id="9e22b-118">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9e22b-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e22b-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e22b-119">Permissions</span></span>
<span data-ttu-id="9e22b-120">В зависимости от ресурса они будут расширенные свойства из и разрешение введите (делегированные или приложения) вы запроса, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="9e22b-120">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="9e22b-121">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e22b-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e22b-122">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="9e22b-122">Supported resource</span></span> | <span data-ttu-id="9e22b-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e22b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="9e22b-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e22b-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e22b-125">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9e22b-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="9e22b-126">calendar</span><span class="sxs-lookup"><span data-stu-id="9e22b-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="9e22b-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-127">Calendars.Read</span></span> | <span data-ttu-id="9e22b-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-128">Calendars.Read</span></span> | <span data-ttu-id="9e22b-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-129">Calendars.Read</span></span> |
| [<span data-ttu-id="9e22b-130">контакт</span><span class="sxs-lookup"><span data-stu-id="9e22b-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="9e22b-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-131">Contacts.Read</span></span> | <span data-ttu-id="9e22b-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-132">Contacts.Read</span></span> | <span data-ttu-id="9e22b-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-133">Contacts.Read</span></span> |
| <span data-ttu-id="9e22b-134">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9e22b-134">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="9e22b-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-135">Contacts.Read</span></span> | <span data-ttu-id="9e22b-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-136">Contacts.Read</span></span> | <span data-ttu-id="9e22b-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-137">Contacts.Read</span></span> |
| [<span data-ttu-id="9e22b-138">событие</span><span class="sxs-lookup"><span data-stu-id="9e22b-138">event</span></span>](../resources/event.md) | <span data-ttu-id="9e22b-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-139">Calendars.Read</span></span> | <span data-ttu-id="9e22b-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-140">Calendars.Read</span></span> |  <span data-ttu-id="9e22b-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-141">Calendars.Read</span></span>|
| <span data-ttu-id="9e22b-142">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="9e22b-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="9e22b-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e22b-143">Group.Read.All</span></span> | <span data-ttu-id="9e22b-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9e22b-144">Not supported</span></span> | <span data-ttu-id="9e22b-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9e22b-145">Not supported</span></span> |
| <span data-ttu-id="9e22b-146">[event](../resources/event.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="9e22b-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="9e22b-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e22b-147">Group.Read.All</span></span> | <span data-ttu-id="9e22b-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9e22b-148">Not supported</span></span> | <span data-ttu-id="9e22b-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9e22b-149">Not supported</span></span> |
| <span data-ttu-id="9e22b-150">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="9e22b-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="9e22b-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e22b-151">Group.Read.All</span></span> | <span data-ttu-id="9e22b-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9e22b-152">Not supported</span></span> | <span data-ttu-id="9e22b-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e22b-153">Group.Read.All</span></span> |
| [<span data-ttu-id="9e22b-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="9e22b-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="9e22b-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-155">Mail.Read</span></span> | <span data-ttu-id="9e22b-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-156">Mail.Read</span></span> | <span data-ttu-id="9e22b-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-157">Mail.Read</span></span> |
| [<span data-ttu-id="9e22b-158">message</span><span class="sxs-lookup"><span data-stu-id="9e22b-158">message</span></span>](../resources/message.md) | <span data-ttu-id="9e22b-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-159">Mail.Read</span></span> | <span data-ttu-id="9e22b-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-160">Mail.Read</span></span> | <span data-ttu-id="9e22b-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e22b-161">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="9e22b-162">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e22b-162">HTTP request</span></span>

<span data-ttu-id="9e22b-p103">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="9e22b-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="9e22b-165">Получение экземпляра **сообщения** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-165">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="9e22b-166">Получение экземпляра **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-166">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="9e22b-167">Получение экземпляра **событий** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-167">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="9e22b-168">Получение экземпляра **календаря** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-168">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="9e22b-169">Получение экземпляра **контактов** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-169">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="9e22b-170">Получение экземпляра **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-170">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="9e22b-171">Получение экземпляра **события** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-171">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="9e22b-172">Получение экземпляра **публиковать** группы:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9e22b-172">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="9e22b-173">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="9e22b-173">Path parameters</span></span>
|<span data-ttu-id="9e22b-174">Параметр</span><span class="sxs-lookup"><span data-stu-id="9e22b-174">Parameter</span></span>|<span data-ttu-id="9e22b-175">Тип</span><span class="sxs-lookup"><span data-stu-id="9e22b-175">Type</span></span>|<span data-ttu-id="9e22b-176">Description</span><span class="sxs-lookup"><span data-stu-id="9e22b-176">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9e22b-177">id_value</span><span class="sxs-lookup"><span data-stu-id="9e22b-177">id_value</span></span>|<span data-ttu-id="9e22b-178">String</span><span class="sxs-lookup"><span data-stu-id="9e22b-178">String</span></span>|<span data-ttu-id="9e22b-p104">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e22b-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9e22b-183">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e22b-183">Request headers</span></span>
| <span data-ttu-id="9e22b-184">Имя</span><span class="sxs-lookup"><span data-stu-id="9e22b-184">Name</span></span>      |<span data-ttu-id="9e22b-185">Описание</span><span class="sxs-lookup"><span data-stu-id="9e22b-185">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e22b-186">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e22b-186">Authorization</span></span>  | <span data-ttu-id="9e22b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e22b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e22b-189">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e22b-189">Request body</span></span>
<span data-ttu-id="9e22b-190">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e22b-190">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e22b-191">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e22b-191">Response</span></span>

<span data-ttu-id="9e22b-192">При успешном выполнении этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="9e22b-192">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="9e22b-193">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="9e22b-193">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="9e22b-194">Пример</span><span class="sxs-lookup"><span data-stu-id="9e22b-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e22b-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e22b-195">Request</span></span>
<span data-ttu-id="9e22b-p106">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="9e22b-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="9e22b-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e22b-198">Response</span></span>

<span data-ttu-id="9e22b-199">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="9e22b-199">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="9e22b-p107">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9e22b-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
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
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
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