---
title: Общие сведения о расширенных свойствах Outlook
description: 'Расширенные свойства позволяют хранить пользовательские данные и специально служат в качестве резервного механизма для приложений, чтобы получать доступ '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: f8a30c69b42ce52f6a81450ffa8739d7d87a12f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026966"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="e15fd-103">Общие сведения о расширенных свойствах Outlook</span><span class="sxs-lookup"><span data-stu-id="e15fd-103">Outlook extended properties overview</span></span>

<span data-ttu-id="e15fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e15fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="e15fd-p101">Расширенные свойства позволяют хранить пользовательские данные и специально служат в качестве резервного механизма для приложений, чтобы получать доступ к пользовательским данным для свойств Outlook MAPI, когда эти свойства _еще не представлены в метаданных API Microsoft Graph_. Можно использовать расширенные свойства API REST, чтобы хранить или получать такие пользовательские данные в следующих пользовательских ресурсах:</span><span class="sxs-lookup"><span data-stu-id="e15fd-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- <span data-ttu-id="e15fd-107">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="e15fd-107">[message](../resources/message.md)</span></span>
- <span data-ttu-id="e15fd-108">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="e15fd-108">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="e15fd-109">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="e15fd-109">[event](../resources/event.md)</span></span>
- <span data-ttu-id="e15fd-110">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="e15fd-110">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e15fd-111">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="e15fd-111">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="e15fd-112">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e15fd-112">[contactFolder](../resources/contactfolder.md)</span></span>
- [<span data-ttu-id="e15fd-113">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="e15fd-113">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="e15fd-114">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="e15fd-114">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="e15fd-115">Или в следующих ресурсах группы Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="e15fd-115">Or, in the following Microsoft 365 group resources:</span></span>

- <span data-ttu-id="e15fd-116">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="e15fd-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="e15fd-117">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="e15fd-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="e15fd-118">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="e15fd-118">group [post](../resources/post.md)</span></span>

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="e15fd-119">Что использовать — расширенные свойства или открытые расширения</span><span class="sxs-lookup"><span data-stu-id="e15fd-119">Use extended properties or open extensions?</span></span>

<span data-ttu-id="e15fd-p102">В большинстве часто применяемых сценариев у вас должна быть возможность использования открытых расширений (они представлены объектом [openTypeExtension](../resources/opentypeextension.md) и ранее звались расширениями данных Office 365), чтобы хранить пользовательские данные и получать к ним доступ для экземпляров ресурса в почтовом ящике пользователя. Используйте расширенные свойства, только если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены в [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api).</span><span class="sxs-lookup"><span data-stu-id="e15fd-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="e15fd-122">Типы расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="e15fd-122">Types of extended properties</span></span>

<span data-ttu-id="e15fd-123">В зависимости от того, собираетесь ли вы хранить одно или несколько значений (одинакового типа) в расширенном свойстве, можно создавать расширенное свойство [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) или [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="e15fd-123">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="e15fd-124">Каждый из этих типов определяет свойство по идентификатору **id** и хранит данные в значении **value**.</span><span class="sxs-lookup"><span data-stu-id="e15fd-124">Each of these types identifies the property by its **id** and stores data in **value**.</span></span>

<span data-ttu-id="e15fd-125">Можно использовать идентификатор **id** для получения конкретного экземпляра ресурса с расширенным свойством или фильтровать расширенное свойство с одним значением для получения всех экземпляров с таким свойством.</span><span class="sxs-lookup"><span data-stu-id="e15fd-125">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span>

<span data-ttu-id="e15fd-126">**Примечание.** Невозможно использовать API REST для получения всех расширенных свойств конкретного экземпляра в одном вызове.</span><span class="sxs-lookup"><span data-stu-id="e15fd-126">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>


### <a name="id-formats"></a><span data-ttu-id="e15fd-127">Форматы идентификаторов</span><span class="sxs-lookup"><span data-stu-id="e15fd-127">id formats</span></span>

<span data-ttu-id="e15fd-128">**Идентификатор** расширенного свойства можно указать в одном из трех форматов:</span><span class="sxs-lookup"><span data-stu-id="e15fd-128">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="e15fd-129">Как именованное свойство, определенное по типу расширенного свойства, пространству имен и имени строки.</span><span class="sxs-lookup"><span data-stu-id="e15fd-129">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="e15fd-130">Как именованное свойство, определенное по типу расширенного свойства, пространству имен и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="e15fd-130">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="e15fd-131">В формате proptag, определенном по типу расширенного свойства и [тегу свойства MAPI](/office/client-developer/outlook/mapi/mapi-property-tags).</span><span class="sxs-lookup"><span data-stu-id="e15fd-131">In a proptag format, identified by the extended property type and a [MAPI property tag](/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="e15fd-132">В следующих двух таблицах описаны эти форматы, применяемые к расширенным свойствам с одним или несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="e15fd-132">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="e15fd-133">{_тип_} представляет собой тип значения или значений расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="e15fd-133">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="e15fd-134">В примерах показаны типы string, integer и массивы этих типов.</span><span class="sxs-lookup"><span data-stu-id="e15fd-134">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="e15fd-135">**Действительные форматы идентификаторов для расширенных свойств с одним значением**</span><span class="sxs-lookup"><span data-stu-id="e15fd-135">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="e15fd-136">**Формат**</span><span class="sxs-lookup"><span data-stu-id="e15fd-136">**Format**</span></span>|<span data-ttu-id="e15fd-137">**Пример**</span><span class="sxs-lookup"><span data-stu-id="e15fd-137">**Example**</span></span>|<span data-ttu-id="e15fd-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e15fd-138">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="e15fd-139">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="e15fd-139">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="e15fd-140">Определяет свойство по пространству имен (GUID), к которому оно принадлежит, и имени строки.</span><span class="sxs-lookup"><span data-stu-id="e15fd-140">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="e15fd-141">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="e15fd-141">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="e15fd-142">Определяет свойство по пространству имен (GUID), к которому оно принадлежит, и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="e15fd-142">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="e15fd-143">"{_тип_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="e15fd-143">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="e15fd-144">Определяет встроенное свойство по тегу свойства.</span><span class="sxs-lookup"><span data-stu-id="e15fd-144">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="e15fd-145">**Действительные форматы идентификаторов для расширенных свойств с несколькими значениями**</span><span class="sxs-lookup"><span data-stu-id="e15fd-145">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="e15fd-146">**Формат**</span><span class="sxs-lookup"><span data-stu-id="e15fd-146">**Format**</span></span>|<span data-ttu-id="e15fd-147">**Пример**</span><span class="sxs-lookup"><span data-stu-id="e15fd-147">**Example**</span></span>|<span data-ttu-id="e15fd-148">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e15fd-148">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="e15fd-149">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="e15fd-149">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="e15fd-150">Определяет свойство по пространству имен (GUID) и имени строки.</span><span class="sxs-lookup"><span data-stu-id="e15fd-150">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="e15fd-151">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="e15fd-151">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="e15fd-152">Определяет свойство по пространству имен (GUID) и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="e15fd-152">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="e15fd-153">"{_тип_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="e15fd-153">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="e15fd-154">Определяет встроенное свойство по тегу свойства.</span><span class="sxs-lookup"><span data-stu-id="e15fd-154">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="e15fd-155">Чтобы определить расширенное свойство с одним или несколькими значениями в качестве настраиваемого свойства, используйте любой из форматов именованных свойств.</span><span class="sxs-lookup"><span data-stu-id="e15fd-155">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="e15fd-156">Первый из двух форматов, который использует имя строки (**Name**), является предпочтительным для упрощения ссылки.</span><span class="sxs-lookup"><span data-stu-id="e15fd-156">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="e15fd-157">У именованных свойств есть [идентификаторы свойств](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) в диапазоне 0x8000-0xfffe.</span><span class="sxs-lookup"><span data-stu-id="e15fd-157">Named properties have their [property identifiers](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="e15fd-158">Чтобы получить доступ к свойствам, предопределенным с помощью MAPI, клиента или сервера, которые еще не представлены в Microsoft Graph, используйте формат proptag.</span><span class="sxs-lookup"><span data-stu-id="e15fd-158">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="e15fd-159">У этих свойств есть идентификаторы в диапазоне 0x0001-0x7fff.</span><span class="sxs-lookup"><span data-stu-id="e15fd-159">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="e15fd-160">Не пытайтесь определять пользовательское свойство с помощью формата proptag.</span><span class="sxs-lookup"><span data-stu-id="e15fd-160">Do not try to define a custom property using the proptag format.</span></span>

<span data-ttu-id="e15fd-161">Информацию о соответствии расширенных свойств и существующих свойств MAPI, таких как идентификатор свойства или GUID, можно найти в статье \[\][MS-OXPROPS: Основной список свойств для протоколов Exchange Server](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e15fd-161">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="e15fd-162">**Примечание.** После выбора формата для свойства **id** получайте доступ к этому расширенному свойству, используя только этот формат.</span><span class="sxs-lookup"><span data-stu-id="e15fd-162">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="e15fd-163">Операции с API REST</span><span class="sxs-lookup"><span data-stu-id="e15fd-163">REST API operations</span></span>

<span data-ttu-id="e15fd-164">Ниже приведены операции с расширенными свойствами с одним значением.</span><span class="sxs-lookup"><span data-stu-id="e15fd-164">Single-value extended property operations:</span></span>

- [<span data-ttu-id="e15fd-165">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="e15fd-165">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="e15fd-166">Получение одного или коллекции экземпляров ресурсов с расширенным свойством с помощью параметра `$expand` или `$filter`</span><span class="sxs-lookup"><span data-stu-id="e15fd-166">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="e15fd-167">Ниже приведены операции с расширенными свойствами с несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="e15fd-167">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="e15fd-168">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="e15fd-168">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="e15fd-169">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`</span><span class="sxs-lookup"><span data-stu-id="e15fd-169">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)



