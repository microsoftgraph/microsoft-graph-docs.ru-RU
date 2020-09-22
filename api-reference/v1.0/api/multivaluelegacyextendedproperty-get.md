---
title: Получение объекта multiValueLegacyExtendedProperty
description: Разверните узел ".
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b948c237bd4d63e23519b79b61f0573b734a19a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018986"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="520b7-103">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="520b7-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="520b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="520b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="520b7-105">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="520b7-105">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="520b7-106">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="520b7-106">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="520b7-107">Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="520b7-107">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="520b7-108">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="520b7-108">The following user resources are supported:</span></span>

- <span data-ttu-id="520b7-109">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="520b7-109">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="520b7-110">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="520b7-110">[contact](../resources/contact.md)</span></span>
- [<span data-ttu-id="520b7-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520b7-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="520b7-112">event</span><span class="sxs-lookup"><span data-stu-id="520b7-112">event</span></span>](../resources/event.md)
- [<span data-ttu-id="520b7-113">mailFolder</span><span class="sxs-lookup"><span data-stu-id="520b7-113">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="520b7-114">message</span><span class="sxs-lookup"><span data-stu-id="520b7-114">message</span></span>](../resources/message.md)

<span data-ttu-id="520b7-115">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="520b7-115">As well as the following group resources:</span></span>

- <span data-ttu-id="520b7-116">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="520b7-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="520b7-117">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="520b7-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="520b7-118">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="520b7-118">group [post](../resources/post.md)</span></span>

<span data-ttu-id="520b7-119">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="520b7-119">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="520b7-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="520b7-120">Permissions</span></span>
<span data-ttu-id="520b7-121">В зависимости от ресурса, из которого вы получаете расширенное свойство, а также от запрашиваемого типа разрешения (делегированного или приложения), для вызова этого API требуется минимум разрешение, указанное в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="520b7-121">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="520b7-122">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="520b7-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="520b7-123">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="520b7-123">Supported resource</span></span> | <span data-ttu-id="520b7-124">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="520b7-124">Delegated (work or school account)</span></span> | <span data-ttu-id="520b7-125">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="520b7-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="520b7-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="520b7-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="520b7-127">calendar</span><span class="sxs-lookup"><span data-stu-id="520b7-127">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="520b7-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-128">Calendars.Read</span></span> | <span data-ttu-id="520b7-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-129">Calendars.Read</span></span> | <span data-ttu-id="520b7-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-130">Calendars.Read</span></span> |
| [<span data-ttu-id="520b7-131">contact</span><span class="sxs-lookup"><span data-stu-id="520b7-131">contact</span></span>](../resources/contact.md) | <span data-ttu-id="520b7-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-132">Contacts.Read</span></span> | <span data-ttu-id="520b7-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-133">Contacts.Read</span></span> | <span data-ttu-id="520b7-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-134">Contacts.Read</span></span> |
| [<span data-ttu-id="520b7-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="520b7-135">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="520b7-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-136">Contacts.Read</span></span> | <span data-ttu-id="520b7-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-137">Contacts.Read</span></span> | <span data-ttu-id="520b7-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-138">Contacts.Read</span></span> |
| [<span data-ttu-id="520b7-139">event</span><span class="sxs-lookup"><span data-stu-id="520b7-139">event</span></span>](../resources/event.md) | <span data-ttu-id="520b7-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-140">Calendars.Read</span></span> | <span data-ttu-id="520b7-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-141">Calendars.Read</span></span> |  <span data-ttu-id="520b7-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-142">Calendars.Read</span></span>|
| <span data-ttu-id="520b7-143">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="520b7-143">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="520b7-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="520b7-144">Group.Read.All</span></span> | <span data-ttu-id="520b7-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="520b7-145">Not supported</span></span> | <span data-ttu-id="520b7-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="520b7-146">Not supported</span></span> |
| <span data-ttu-id="520b7-147">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="520b7-147">group [event](../resources/event.md)</span></span> | <span data-ttu-id="520b7-148">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="520b7-148">Group.Read.All</span></span> | <span data-ttu-id="520b7-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="520b7-149">Not supported</span></span> | <span data-ttu-id="520b7-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="520b7-150">Not supported</span></span> |
| <span data-ttu-id="520b7-151">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="520b7-151">group [post](../resources/post.md)</span></span> | <span data-ttu-id="520b7-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="520b7-152">Group.Read.All</span></span> | <span data-ttu-id="520b7-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="520b7-153">Not supported</span></span> | <span data-ttu-id="520b7-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="520b7-154">Group.Read.All</span></span> |
| [<span data-ttu-id="520b7-155">mailFolder</span><span class="sxs-lookup"><span data-stu-id="520b7-155">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="520b7-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-156">Mail.Read</span></span> | <span data-ttu-id="520b7-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-157">Mail.Read</span></span> | <span data-ttu-id="520b7-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-158">Mail.Read</span></span> |
| [<span data-ttu-id="520b7-159">message</span><span class="sxs-lookup"><span data-stu-id="520b7-159">message</span></span>](../resources/message.md) | <span data-ttu-id="520b7-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-160">Mail.Read</span></span> | <span data-ttu-id="520b7-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-161">Mail.Read</span></span> | <span data-ttu-id="520b7-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="520b7-162">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="520b7-163">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="520b7-163">HTTP request</span></span>

<span data-ttu-id="520b7-p103">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="520b7-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="520b7-166">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="520b7-166">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="520b7-167">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="520b7-167">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="520b7-168">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="520b7-168">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="520b7-169">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="520b7-169">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="520b7-170">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="520b7-170">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="520b7-171">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="520b7-171">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="520b7-172">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="520b7-172">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="520b7-173">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="520b7-173">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="520b7-174">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="520b7-174">Path parameters</span></span>
|<span data-ttu-id="520b7-175">Параметр</span><span class="sxs-lookup"><span data-stu-id="520b7-175">Parameter</span></span>|<span data-ttu-id="520b7-176">Тип</span><span class="sxs-lookup"><span data-stu-id="520b7-176">Type</span></span>|<span data-ttu-id="520b7-177">Описание</span><span class="sxs-lookup"><span data-stu-id="520b7-177">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="520b7-178">id_value</span><span class="sxs-lookup"><span data-stu-id="520b7-178">id_value</span></span>|<span data-ttu-id="520b7-179">String</span><span class="sxs-lookup"><span data-stu-id="520b7-179">String</span></span>|<span data-ttu-id="520b7-p104">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="520b7-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="520b7-184">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="520b7-184">Request headers</span></span>
| <span data-ttu-id="520b7-185">Имя</span><span class="sxs-lookup"><span data-stu-id="520b7-185">Name</span></span>      |<span data-ttu-id="520b7-186">Описание</span><span class="sxs-lookup"><span data-stu-id="520b7-186">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="520b7-187">Авторизация</span><span class="sxs-lookup"><span data-stu-id="520b7-187">Authorization</span></span>  | <span data-ttu-id="520b7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="520b7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="520b7-190">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="520b7-190">Request body</span></span>
<span data-ttu-id="520b7-191">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="520b7-191">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="520b7-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="520b7-192">Response</span></span>

<span data-ttu-id="520b7-193">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="520b7-193">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="520b7-194">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="520b7-194">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="520b7-195">Пример</span><span class="sxs-lookup"><span data-stu-id="520b7-195">Example</span></span>
##### <a name="request"></a><span data-ttu-id="520b7-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="520b7-196">Request</span></span>
<span data-ttu-id="520b7-p106">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="520b7-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="520b7-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="520b7-199">Response</span></span>

<span data-ttu-id="520b7-200">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="520b7-200">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="520b7-p107">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="520b7-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

