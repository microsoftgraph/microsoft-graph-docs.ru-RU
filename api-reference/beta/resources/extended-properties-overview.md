---
title: Общие сведения о расширенных свойствах Outlook
description: 'Расширенные свойства позволяют хранить пользовательские данные и специально служат в качестве резервного механизма для приложений, чтобы получать доступ '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 1b6364fd42b72e175a58bfcd28c0bdacc5e9629e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866835"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="627a7-103">Общие сведения о расширенных свойствах Outlook</span><span class="sxs-lookup"><span data-stu-id="627a7-103">Outlook extended properties overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="627a7-p101">Расширенные свойства позволяют хранить пользовательские данные и специально служат в качестве резервного механизма для приложений, чтобы получать доступ к пользовательским данным для свойств Outlook MAPI, когда эти свойства _еще не представлены в метаданных API Microsoft Graph_. Можно использовать расширенные свойства API REST, чтобы хранить или получать такие пользовательские данные в следующих пользовательских ресурсах:</span><span class="sxs-lookup"><span data-stu-id="627a7-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- <span data-ttu-id="627a7-106">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="627a7-106">[message](../resources/message.md)</span></span>
- <span data-ttu-id="627a7-107">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="627a7-107">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="627a7-108">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="627a7-108">[event](../resources/event.md)</span></span>
- <span data-ttu-id="627a7-109">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="627a7-109">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="627a7-110">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="627a7-110">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="627a7-111">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="627a7-111">[contactFolder](../resources/contactfolder.md)</span></span>
- [<span data-ttu-id="627a7-112">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="627a7-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="627a7-113">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="627a7-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="627a7-114">Или в следующих ресурсах группы Office 365:</span><span class="sxs-lookup"><span data-stu-id="627a7-114">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="627a7-115">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="627a7-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="627a7-116">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="627a7-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="627a7-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="627a7-117">group [post](../resources/post.md)</span></span>

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="627a7-118">Что использовать — расширенные свойства или открытые расширения</span><span class="sxs-lookup"><span data-stu-id="627a7-118">Use extended properties or open extensions?</span></span>

<span data-ttu-id="627a7-p102">В большинстве часто применяемых сценариев у вас должна быть возможность использования открытых расширений (они представлены объектом [openTypeExtension](../resources/opentypeextension.md) и ранее звались расширениями данных Office 365), чтобы хранить пользовательские данные и получать к ним доступ для экземпляров ресурса в почтовом ящике пользователя. Используйте расширенные свойства, только если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены в [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api).</span><span class="sxs-lookup"><span data-stu-id="627a7-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="627a7-121">Типы расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="627a7-121">Types of extended properties</span></span>

<span data-ttu-id="627a7-122">В зависимости от того, собираетесь ли вы хранить одно или несколько значений (одинакового типа) в расширенном свойстве, можно создавать расширенное свойство [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) или [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="627a7-122">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="627a7-123">Каждый из этих типов определяет свойство по идентификатору **id** и хранит данные в значении **value**.</span><span class="sxs-lookup"><span data-stu-id="627a7-123">Each of these types identifies the property by its **id** and stores data in **value**.</span></span>

<span data-ttu-id="627a7-124">Можно использовать идентификатор **id** для получения конкретного экземпляра ресурса с расширенным свойством или фильтровать расширенное свойство с одним значением для получения всех экземпляров с таким свойством.</span><span class="sxs-lookup"><span data-stu-id="627a7-124">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span>

<span data-ttu-id="627a7-125">**Примечание.** Невозможно использовать API REST для получения всех расширенных свойств конкретного экземпляра в одном вызове.</span><span class="sxs-lookup"><span data-stu-id="627a7-125">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>


### <a name="id-formats"></a><span data-ttu-id="627a7-126">Форматы идентификаторов</span><span class="sxs-lookup"><span data-stu-id="627a7-126">id formats</span></span>

<span data-ttu-id="627a7-127">**Идентификатор** расширенного свойства можно указать в одном из трех форматов:</span><span class="sxs-lookup"><span data-stu-id="627a7-127">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="627a7-128">Как именованное свойство, определенное по типу расширенного свойства, пространству имен и имени строки.</span><span class="sxs-lookup"><span data-stu-id="627a7-128">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="627a7-129">Как именованное свойство, определенное по типу расширенного свойства, пространству имен и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="627a7-129">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="627a7-130">В формате proptag, определенном по типу расширенного свойства и [тегу свойства MAPI](/office/client-developer/outlook/mapi/mapi-property-tags).</span><span class="sxs-lookup"><span data-stu-id="627a7-130">In a proptag format, identified by the extended property type and a [MAPI property tag](/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="627a7-131">В следующих двух таблицах описаны эти форматы, применяемые к расширенным свойствам с одним или несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="627a7-131">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="627a7-132">{_тип_} представляет собой тип значения или значений расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="627a7-132">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="627a7-133">В примерах показаны типы string, integer и массивы этих типов.</span><span class="sxs-lookup"><span data-stu-id="627a7-133">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="627a7-134">**Действительные форматы идентификаторов для расширенных свойств с одним значением**</span><span class="sxs-lookup"><span data-stu-id="627a7-134">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="627a7-135">**Формат**</span><span class="sxs-lookup"><span data-stu-id="627a7-135">**Format**</span></span>|<span data-ttu-id="627a7-136">**Пример**</span><span class="sxs-lookup"><span data-stu-id="627a7-136">**Example**</span></span>|<span data-ttu-id="627a7-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="627a7-137">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="627a7-138">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="627a7-138">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="627a7-139">Определяет свойство по пространству имен (GUID), к которому оно принадлежит, и имени строки.</span><span class="sxs-lookup"><span data-stu-id="627a7-139">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="627a7-140">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="627a7-140">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="627a7-141">Определяет свойство по пространству имен (GUID), к которому оно принадлежит, и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="627a7-141">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="627a7-142">"{_тип_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="627a7-142">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="627a7-143">Определяет встроенное свойство по тегу свойства.</span><span class="sxs-lookup"><span data-stu-id="627a7-143">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="627a7-144">**Действительные форматы идентификаторов для расширенных свойств с несколькими значениями**</span><span class="sxs-lookup"><span data-stu-id="627a7-144">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="627a7-145">**Формат**</span><span class="sxs-lookup"><span data-stu-id="627a7-145">**Format**</span></span>|<span data-ttu-id="627a7-146">**Пример**</span><span class="sxs-lookup"><span data-stu-id="627a7-146">**Example**</span></span>|<span data-ttu-id="627a7-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="627a7-147">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="627a7-148">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="627a7-148">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="627a7-149">Определяет свойство по пространству имен (GUID) и имени строки.</span><span class="sxs-lookup"><span data-stu-id="627a7-149">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="627a7-150">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="627a7-150">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="627a7-151">Определяет свойство по пространству имен (GUID) и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="627a7-151">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="627a7-152">"{_тип_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="627a7-152">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="627a7-153">Определяет встроенное свойство по тегу свойства.</span><span class="sxs-lookup"><span data-stu-id="627a7-153">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="627a7-154">Чтобы определить расширенное свойство с одним или несколькими значениями в качестве настраиваемого свойства, используйте любой из форматов именованных свойств.</span><span class="sxs-lookup"><span data-stu-id="627a7-154">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="627a7-155">Первый из двух форматов, который использует имя строки (**Name**), является предпочтительным для упрощения ссылки.</span><span class="sxs-lookup"><span data-stu-id="627a7-155">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="627a7-156">У именованных свойств есть [идентификаторы свойств](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) в диапазоне 0x8000-0xfffe.</span><span class="sxs-lookup"><span data-stu-id="627a7-156">Named properties have their [property identifiers](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="627a7-157">Чтобы получить доступ к свойствам, предопределенным с помощью MAPI, клиента или сервера, которые еще не представлены в Microsoft Graph, используйте формат proptag.</span><span class="sxs-lookup"><span data-stu-id="627a7-157">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="627a7-158">У этих свойств есть идентификаторы в диапазоне 0x0001-0x7fff.</span><span class="sxs-lookup"><span data-stu-id="627a7-158">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="627a7-159">Не пытайтесь определять пользовательское свойство с помощью формата proptag.</span><span class="sxs-lookup"><span data-stu-id="627a7-159">Do not try to define a custom property using the proptag format.</span></span>

<span data-ttu-id="627a7-160">Информацию о соответствии расширенных свойств и существующих свойств MAPI, таких как идентификатор свойства или GUID, можно найти в статье \[\][MS-OXPROPS: Основной список свойств для протоколов Exchange Server](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="627a7-160">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="627a7-161">**Примечание.** После выбора формата для свойства **id** получайте доступ к этому расширенному свойству, используя только этот формат.</span><span class="sxs-lookup"><span data-stu-id="627a7-161">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="627a7-162">Операции с API REST</span><span class="sxs-lookup"><span data-stu-id="627a7-162">REST API operations</span></span>

<span data-ttu-id="627a7-163">Ниже приведены операции с расширенными свойствами с одним значением.</span><span class="sxs-lookup"><span data-stu-id="627a7-163">Single-value extended property operations:</span></span>

- [<span data-ttu-id="627a7-164">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="627a7-164">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="627a7-165">Получение одного или коллекции экземпляров ресурсов с расширенным свойством с помощью параметра `$expand` или `$filter`</span><span class="sxs-lookup"><span data-stu-id="627a7-165">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="627a7-166">Ниже приведены операции с расширенными свойствами с несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="627a7-166">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="627a7-167">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="627a7-167">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="627a7-168">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`</span><span class="sxs-lookup"><span data-stu-id="627a7-168">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

