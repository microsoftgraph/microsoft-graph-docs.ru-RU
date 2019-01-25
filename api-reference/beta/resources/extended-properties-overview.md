---
title: Общие сведения о расширенных свойствах Outlook
description: 'Разрешить хранение пользовательских данных и специально работать как резервный механизм для приложений для доступа к расширенных свойств '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ead40279547fa838b7224a25c3605d0825c3f797
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517997"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="b56ed-103">Общие сведения о расширенных свойствах Outlook</span><span class="sxs-lookup"><span data-stu-id="b56ed-103">Outlook extended properties overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b56ed-p101">Расширенные свойства позволяют хранить пользовательские данные и специально служат в качестве резервного механизма для приложений, чтобы получать доступ к пользовательским данным для свойств Outlook MAPI, когда эти свойства _еще не представлены в метаданных API Microsoft Graph_. Можно использовать расширенные свойства API REST, чтобы хранить или получать такие пользовательские данные в следующих пользовательских ресурсах:</span><span class="sxs-lookup"><span data-stu-id="b56ed-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- <span data-ttu-id="b56ed-106">[message](../resources/message.md);</span><span class="sxs-lookup"><span data-stu-id="b56ed-106">[message](../resources/message.md)</span></span>
- <span data-ttu-id="b56ed-107">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="b56ed-107">[mailFolder](../resources/mailfolder.md)</span></span>
- <span data-ttu-id="b56ed-108">[event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="b56ed-108">[event](../resources/event.md)</span></span>
- <span data-ttu-id="b56ed-109">[calendar](../resources/calendar.md);</span><span class="sxs-lookup"><span data-stu-id="b56ed-109">[calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="b56ed-110">[contact](../resources/contact.md);</span><span class="sxs-lookup"><span data-stu-id="b56ed-110">[contact](../resources/contact.md)</span></span>
- <span data-ttu-id="b56ed-111">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="b56ed-111">[contactFolder](../resources/contactfolder.md)</span></span>
- [<span data-ttu-id="b56ed-112">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="b56ed-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="b56ed-113">Папки задач Outlook</span><span class="sxs-lookup"><span data-stu-id="b56ed-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) 

<span data-ttu-id="b56ed-114">Или в следующих ресурсах группы Office 365:</span><span class="sxs-lookup"><span data-stu-id="b56ed-114">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="b56ed-115">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="b56ed-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="b56ed-116">[calendar](../resources/calendar.md) для групп;</span><span class="sxs-lookup"><span data-stu-id="b56ed-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="b56ed-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="b56ed-117">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="b56ed-118">Что использовать — расширенные свойства или открытые расширения</span><span class="sxs-lookup"><span data-stu-id="b56ed-118">Use extended properties or open extensions?</span></span>

<span data-ttu-id="b56ed-p102">В большинстве часто применяемых сценариев у вас должна быть возможность использования открытых расширений (они представлены объектом [openTypeExtension](../resources/opentypeextension.md) и ранее звались расширениями данных Office 365), чтобы хранить пользовательские данные и получать к ним доступ для экземпляров ресурса в почтовом ящике пользователя. Используйте расширенные свойства, только если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены в [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api).</span><span class="sxs-lookup"><span data-stu-id="b56ed-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="b56ed-121">Типы расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="b56ed-121">Types of extended properties</span></span>

<span data-ttu-id="b56ed-122">В зависимости от того, собираетесь ли вы хранить одно или несколько значений (одинакового типа) в расширенном свойстве, можно создавать расширенное свойство [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) или [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="b56ed-122">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="b56ed-123">Каждый из этих типов определяет свойство по идентификатору **id** и хранит данные в значении **value**.</span><span class="sxs-lookup"><span data-stu-id="b56ed-123">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="b56ed-124">Можно использовать идентификатор **id** для получения конкретного экземпляра ресурса с расширенным свойством или фильтровать расширенное свойство с одним значением для получения всех экземпляров с таким свойством.</span><span class="sxs-lookup"><span data-stu-id="b56ed-124">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="b56ed-125">**Примечание.** Невозможно использовать API REST для получения всех расширенных свойств конкретного экземпляра в одном вызове.</span><span class="sxs-lookup"><span data-stu-id="b56ed-125">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="b56ed-126">Форматы идентификаторов</span><span class="sxs-lookup"><span data-stu-id="b56ed-126">id formats</span></span>

<span data-ttu-id="b56ed-127">**Идентификатор** расширенного свойства можно указать в одном из трех форматах:</span><span class="sxs-lookup"><span data-stu-id="b56ed-127">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="b56ed-128">Как именованное свойство, указанный тип расширенные свойства, пространство имен и имя строки.</span><span class="sxs-lookup"><span data-stu-id="b56ed-128">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="b56ed-129">Как именованное свойство, определенный тип расширенные свойства, пространства имен и числовой идентификатор.</span><span class="sxs-lookup"><span data-stu-id="b56ed-129">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="b56ed-130">В формате важный параметр proptag, указанный тип расширенные свойства и [тег свойства MAPI](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span><span class="sxs-lookup"><span data-stu-id="b56ed-130">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="b56ed-131">Следующие 2 таблицах описаны эти форматы в качестве примененные к одной и несколькими значениями расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="b56ed-131">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="b56ed-132">{_Тип_} представляет тип значениями, расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="b56ed-132">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="b56ed-133">В примерах показаны типы string, integer и массивы этих типов.</span><span class="sxs-lookup"><span data-stu-id="b56ed-133">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="b56ed-134">**Действительные форматы идентификаторов для расширенных свойств с одним значением**</span><span class="sxs-lookup"><span data-stu-id="b56ed-134">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="b56ed-135">**Формат**</span><span class="sxs-lookup"><span data-stu-id="b56ed-135">**Format**</span></span>|<span data-ttu-id="b56ed-136">**Пример**</span><span class="sxs-lookup"><span data-stu-id="b56ed-136">**Example**</span></span>|<span data-ttu-id="b56ed-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b56ed-137">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="b56ed-138">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="b56ed-138">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="b56ed-139">Определяет свойство, пространства имен (GUID), он принадлежит, а имя строки.</span><span class="sxs-lookup"><span data-stu-id="b56ed-139">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="b56ed-140">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="b56ed-140">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="b56ed-141">Определяет свойство, пространства имен (GUID), он принадлежит и числовой идентификатор.</span><span class="sxs-lookup"><span data-stu-id="b56ed-141">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="b56ed-142">«{_Тип_} {_важный параметр proptag_}»</span><span class="sxs-lookup"><span data-stu-id="b56ed-142">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="b56ed-143">Идентифицирует предварительно заданные свойства, его свойство тег.</span><span class="sxs-lookup"><span data-stu-id="b56ed-143">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="b56ed-144">**Действительные форматы идентификаторов для расширенных свойств с несколькими значениями**</span><span class="sxs-lookup"><span data-stu-id="b56ed-144">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="b56ed-145">**Формат**</span><span class="sxs-lookup"><span data-stu-id="b56ed-145">**Format**</span></span>|<span data-ttu-id="b56ed-146">**Пример**</span><span class="sxs-lookup"><span data-stu-id="b56ed-146">**Example**</span></span>|<span data-ttu-id="b56ed-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b56ed-147">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="b56ed-148">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="b56ed-148">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="b56ed-149">Определяет свойство, пространства имен (GUID) и имя строки.</span><span class="sxs-lookup"><span data-stu-id="b56ed-149">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="b56ed-150">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="b56ed-150">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="b56ed-151">Определяет свойство, пространства имен (GUID) и числовой идентификатор.</span><span class="sxs-lookup"><span data-stu-id="b56ed-151">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="b56ed-152">«{_Тип_} {_важный параметр proptag_}»</span><span class="sxs-lookup"><span data-stu-id="b56ed-152">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="b56ed-153">Идентифицирует предварительно заданные свойства, его свойство тег.</span><span class="sxs-lookup"><span data-stu-id="b56ed-153">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="b56ed-154">Используйте один из форматов именованное свойство определение значение одним или несколькими значениями расширенные свойства в качестве настраиваемого свойства.</span><span class="sxs-lookup"><span data-stu-id="b56ed-154">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="b56ed-155">Между двумя форматы первый, который принимает строковое имя (**имя**) является предпочтительным форматом для упрощения ссылки.</span><span class="sxs-lookup"><span data-stu-id="b56ed-155">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="b56ed-156">Именованные свойства имеют свои [идентификаторы свойств](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) в 0x8000-0xfffe диапазона.</span><span class="sxs-lookup"><span data-stu-id="b56ed-156">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="b56ed-157">Используйте формат важный параметр proptag для доступа к свойствам предопределенное с MAPI или клиента или сервера, и еще не был представлен в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b56ed-157">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="b56ed-158">Эти свойства имеют идентификаторы свойств в 0x0001-0x7fff диапазона.</span><span class="sxs-lookup"><span data-stu-id="b56ed-158">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="b56ed-159">Не пытайтесь определение настраиваемого свойства в формате важный параметр proptag.</span><span class="sxs-lookup"><span data-stu-id="b56ed-159">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="b56ed-160">Информацию о соответствии расширенных свойств и существующих свойств MAPI, таких как идентификатор свойства или GUID, можно найти в статье \[\][MS-OXPROPS: Основной список свойств для протоколов Exchange Server](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b56ed-160">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="b56ed-161">**Примечание.** После выбора формата для свойства **id** получайте доступ к этому расширенному свойству, используя только этот формат.</span><span class="sxs-lookup"><span data-stu-id="b56ed-161">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="b56ed-162">Операции с API REST</span><span class="sxs-lookup"><span data-stu-id="b56ed-162">REST API operations</span></span>
 
<span data-ttu-id="b56ed-163">Ниже приведены операции с расширенными свойствами с одним значением.</span><span class="sxs-lookup"><span data-stu-id="b56ed-163">Single-value extended property operations:</span></span>

- [<span data-ttu-id="b56ed-164">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="b56ed-164">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="b56ed-165">Получение одного или коллекции экземпляров ресурсов с расширенным свойством с помощью параметра `$expand` или `$filter`</span><span class="sxs-lookup"><span data-stu-id="b56ed-165">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="b56ed-166">Ниже приведены операции с расширенными свойствами с несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="b56ed-166">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="b56ed-167">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="b56ed-167">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="b56ed-168">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`</span><span class="sxs-lookup"><span data-stu-id="b56ed-168">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/extended-properties-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
