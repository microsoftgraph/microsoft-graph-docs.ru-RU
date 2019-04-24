---
title: Получение объекта multiValueLegacyExtendedProperty
description: Разверните узел ".
localization_priority: Normal
ms.openlocfilehash: c1d95e319637df17f04e706055245d5e19762a87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585316"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="31e56-103">Получение объекта multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="31e56-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="31e56-104">Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="31e56-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="31e56-105">С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством.</span><span class="sxs-lookup"><span data-stu-id="31e56-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="31e56-106">Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.</span><span class="sxs-lookup"><span data-stu-id="31e56-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="31e56-107">Поддерживаются следующие ресурсы пользователей:</span><span class="sxs-lookup"><span data-stu-id="31e56-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="31e56-108">calendar</span><span class="sxs-lookup"><span data-stu-id="31e56-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="31e56-109">contact</span><span class="sxs-lookup"><span data-stu-id="31e56-109">contact</span></span>](../resources/contact.md)
- <span data-ttu-id="31e56-110">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="31e56-110">[contactFolder](../resources/contactfolder.md)</span></span> 
- [<span data-ttu-id="31e56-111">event</span><span class="sxs-lookup"><span data-stu-id="31e56-111">event</span></span>](../resources/event.md)
- <span data-ttu-id="31e56-112">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="31e56-112">[mailFolder](../resources/mailfolder.md)</span></span>
- [<span data-ttu-id="31e56-113">message</span><span class="sxs-lookup"><span data-stu-id="31e56-113">message</span></span>](../resources/message.md) 

<span data-ttu-id="31e56-114">Кроме того, поддерживаются следующие ресурсы групп:</span><span class="sxs-lookup"><span data-stu-id="31e56-114">As well as the following group resources:</span></span>

- <span data-ttu-id="31e56-115">[calendar](../resources/calendar.md) для групп</span><span class="sxs-lookup"><span data-stu-id="31e56-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="31e56-116">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="31e56-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="31e56-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="31e56-117">group [post](../resources/post.md)</span></span>

<span data-ttu-id="31e56-118">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="31e56-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="31e56-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31e56-119">Permissions</span></span>
<span data-ttu-id="31e56-120">В зависимости от ресурса, из которого вы получаете расширенное свойство, а также от запрашиваемого типа разрешения (делегированного или приложения), для вызова этого API требуется минимум разрешение, указанное в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="31e56-120">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="31e56-121">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31e56-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31e56-122">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="31e56-122">Supported resource</span></span> | <span data-ttu-id="31e56-123">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31e56-123">Delegated (work or school account)</span></span> | <span data-ttu-id="31e56-124">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31e56-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31e56-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31e56-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="31e56-126">calendar</span><span class="sxs-lookup"><span data-stu-id="31e56-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="31e56-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-127">Calendars.Read</span></span> | <span data-ttu-id="31e56-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-128">Calendars.Read</span></span> | <span data-ttu-id="31e56-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-129">Calendars.Read</span></span> |
| [<span data-ttu-id="31e56-130">contact</span><span class="sxs-lookup"><span data-stu-id="31e56-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="31e56-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-131">Contacts.Read</span></span> | <span data-ttu-id="31e56-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-132">Contacts.Read</span></span> | <span data-ttu-id="31e56-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-133">Contacts.Read</span></span> |
| <span data-ttu-id="31e56-134">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="31e56-134">[contactFolder](../resources/contactfolder.md)</span></span> | <span data-ttu-id="31e56-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-135">Contacts.Read</span></span> | <span data-ttu-id="31e56-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-136">Contacts.Read</span></span> | <span data-ttu-id="31e56-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-137">Contacts.Read</span></span> |
| [<span data-ttu-id="31e56-138">event</span><span class="sxs-lookup"><span data-stu-id="31e56-138">event</span></span>](../resources/event.md) | <span data-ttu-id="31e56-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-139">Calendars.Read</span></span> | <span data-ttu-id="31e56-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-140">Calendars.Read</span></span> |  <span data-ttu-id="31e56-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-141">Calendars.Read</span></span>|
| <span data-ttu-id="31e56-142">[calendar](../resources/calendar.md) для групп</span><span class="sxs-lookup"><span data-stu-id="31e56-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="31e56-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31e56-143">Group.Read.All</span></span> | <span data-ttu-id="31e56-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31e56-144">Not supported</span></span> | <span data-ttu-id="31e56-145">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31e56-145">Not supported</span></span> |
| <span data-ttu-id="31e56-146">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="31e56-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="31e56-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31e56-147">Group.Read.All</span></span> | <span data-ttu-id="31e56-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31e56-148">Not supported</span></span> | <span data-ttu-id="31e56-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31e56-149">Not supported</span></span> |
| <span data-ttu-id="31e56-150">group [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="31e56-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="31e56-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31e56-151">Group.Read.All</span></span> | <span data-ttu-id="31e56-152">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="31e56-152">Not supported</span></span> | <span data-ttu-id="31e56-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="31e56-153">Group.Read.All</span></span> |
| <span data-ttu-id="31e56-154">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="31e56-154">[mailFolder](../resources/mailfolder.md)</span></span> | <span data-ttu-id="31e56-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-155">Mail.Read</span></span> | <span data-ttu-id="31e56-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-156">Mail.Read</span></span> | <span data-ttu-id="31e56-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-157">Mail.Read</span></span> |
| [<span data-ttu-id="31e56-158">message</span><span class="sxs-lookup"><span data-stu-id="31e56-158">message</span></span>](../resources/message.md) | <span data-ttu-id="31e56-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-159">Mail.Read</span></span> | <span data-ttu-id="31e56-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-160">Mail.Read</span></span> | <span data-ttu-id="31e56-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="31e56-161">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="31e56-162">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31e56-162">HTTP request</span></span>

<span data-ttu-id="31e56-p103">Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.</span><span class="sxs-lookup"><span data-stu-id="31e56-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="31e56-165">Получение экземпляра объекта **message**:</span><span class="sxs-lookup"><span data-stu-id="31e56-165">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31e56-166">Получение экземпляра объекта **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="31e56-166">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="31e56-167">Получение экземпляра объекта **event**:</span><span class="sxs-lookup"><span data-stu-id="31e56-167">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31e56-168">Получение экземпляра объекта **calendar**:</span><span class="sxs-lookup"><span data-stu-id="31e56-168">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31e56-169">Получение экземпляра объекта **contact**:</span><span class="sxs-lookup"><span data-stu-id="31e56-169">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31e56-170">Получение экземпляра объекта **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="31e56-170">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="31e56-171">Получение экземпляра объекта **event** для группы:</span><span class="sxs-lookup"><span data-stu-id="31e56-171">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="31e56-172">Получение экземпляра объекта **post** для группы:</span><span class="sxs-lookup"><span data-stu-id="31e56-172">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="31e56-173">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="31e56-173">Path parameters</span></span>
|<span data-ttu-id="31e56-174">Параметр</span><span class="sxs-lookup"><span data-stu-id="31e56-174">Parameter</span></span>|<span data-ttu-id="31e56-175">Тип</span><span class="sxs-lookup"><span data-stu-id="31e56-175">Type</span></span>|<span data-ttu-id="31e56-176">Описание</span><span class="sxs-lookup"><span data-stu-id="31e56-176">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="31e56-177">id_value</span><span class="sxs-lookup"><span data-stu-id="31e56-177">id_value</span></span>|<span data-ttu-id="31e56-178">String</span><span class="sxs-lookup"><span data-stu-id="31e56-178">String</span></span>|<span data-ttu-id="31e56-p104">Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31e56-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="31e56-183">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31e56-183">Request headers</span></span>
| <span data-ttu-id="31e56-184">Имя</span><span class="sxs-lookup"><span data-stu-id="31e56-184">Name</span></span>      |<span data-ttu-id="31e56-185">Описание</span><span class="sxs-lookup"><span data-stu-id="31e56-185">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31e56-186">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31e56-186">Authorization</span></span>  | <span data-ttu-id="31e56-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31e56-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31e56-189">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31e56-189">Request body</span></span>
<span data-ttu-id="31e56-190">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31e56-190">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31e56-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="31e56-191">Response</span></span>

<span data-ttu-id="31e56-192">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="31e56-192">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="31e56-193">Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="31e56-193">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="31e56-194">Пример</span><span class="sxs-lookup"><span data-stu-id="31e56-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31e56-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="31e56-195">Request</span></span>
<span data-ttu-id="31e56-p106">В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).</span><span class="sxs-lookup"><span data-stu-id="31e56-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="31e56-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="31e56-198">Response</span></span>

<span data-ttu-id="31e56-199">Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.</span><span class="sxs-lookup"><span data-stu-id="31e56-199">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="31e56-p107">Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="31e56-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
