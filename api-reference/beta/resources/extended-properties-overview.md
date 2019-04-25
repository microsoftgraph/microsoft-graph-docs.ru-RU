---
title: Общие сведения о расширенных свойствах Outlook
description: 'Расширенные свойства позволяют хранить пользовательские данные и специально служить резервным механизмом для доступа приложений к '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ead40279547fa838b7224a25c3605d0825c3f797
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542915"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="1e3d4-103">Общие сведения о расширенных свойствах Outlook</span><span class="sxs-lookup"><span data-stu-id="1e3d4-103">Outlook extended properties overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e3d4-p101">Расширенные свойства позволяют хранить пользовательские данные и специально служат в качестве резервного механизма для приложений, чтобы получать доступ к пользовательским данным для свойств Outlook MAPI, когда эти свойства _еще не представлены в метаданных API Microsoft Graph_. Можно использовать расширенные свойства API REST, чтобы хранить или получать такие пользовательские данные в следующих пользовательских ресурсах:</span><span class="sxs-lookup"><span data-stu-id="1e3d4-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="1e3d4-106">message</span><span class="sxs-lookup"><span data-stu-id="1e3d4-106">message</span></span>](../resources/message.md)
- <span data-ttu-id="1e3d4-107">[mailFolder](../resources/mailfolder.md);</span><span class="sxs-lookup"><span data-stu-id="1e3d4-107">[mailFolder](../resources/mailfolder.md)</span></span>
- [<span data-ttu-id="1e3d4-108">event</span><span class="sxs-lookup"><span data-stu-id="1e3d4-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="1e3d4-109">calendar</span><span class="sxs-lookup"><span data-stu-id="1e3d4-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="1e3d4-110">contact</span><span class="sxs-lookup"><span data-stu-id="1e3d4-110">contact</span></span>](../resources/contact.md)
- <span data-ttu-id="1e3d4-111">[contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1e3d4-111">[contactFolder](../resources/contactfolder.md)</span></span>
- [<span data-ttu-id="1e3d4-112">Задача Outlook</span><span class="sxs-lookup"><span data-stu-id="1e3d4-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="1e3d4-113">Папка задач Outlook</span><span class="sxs-lookup"><span data-stu-id="1e3d4-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) 

<span data-ttu-id="1e3d4-114">Или в следующих ресурсах группы Office 365:</span><span class="sxs-lookup"><span data-stu-id="1e3d4-114">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="1e3d4-115">group [event](../resources/event.md);</span><span class="sxs-lookup"><span data-stu-id="1e3d4-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="1e3d4-116">[calendar](../resources/calendar.md) для групп</span><span class="sxs-lookup"><span data-stu-id="1e3d4-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="1e3d4-117">[post](../resources/post.md) для групп.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-117">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="1e3d4-118">Что использовать — расширенные свойства или открытые расширения</span><span class="sxs-lookup"><span data-stu-id="1e3d4-118">Use extended properties or open extensions?</span></span>

<span data-ttu-id="1e3d4-p102">В большинстве часто применяемых сценариев у вас должна быть возможность использования открытых расширений (они представлены объектом [openTypeExtension](../resources/opentypeextension.md) и ранее звались расширениями данных Office 365), чтобы хранить пользовательские данные и получать к ним доступ для экземпляров ресурса в почтовом ящике пользователя. Используйте расширенные свойства, только если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены в [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api).</span><span class="sxs-lookup"><span data-stu-id="1e3d4-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="1e3d4-121">Типы расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="1e3d4-121">Types of extended properties</span></span>

<span data-ttu-id="1e3d4-122">В зависимости от того, собираетесь ли вы хранить одно или несколько значений (одинакового типа) в расширенном свойстве, можно создавать расширенное свойство [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) или [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="1e3d4-122">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="1e3d4-123">Каждый из этих типов определяет свойство по идентификатору **id** и хранит данные в значении **value**.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-123">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="1e3d4-124">Можно использовать идентификатор **id** для получения конкретного экземпляра ресурса с расширенным свойством или фильтровать расширенное свойство с одним значением для получения всех экземпляров с таким свойством.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-124">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="1e3d4-125">**Примечание.** Невозможно использовать API REST для получения всех расширенных свойств конкретного экземпляра в одном вызове.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-125">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="1e3d4-126">форматы идентификаторов</span><span class="sxs-lookup"><span data-stu-id="1e3d4-126">id formats</span></span>

<span data-ttu-id="1e3d4-127">**Идентификатор** расширенного свойства можно указать в одном из трех форматов:</span><span class="sxs-lookup"><span data-stu-id="1e3d4-127">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="1e3d4-128">Как именованное свойство, определяемое типом расширенного свойства, пространством имен и строковым именем.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-128">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="1e3d4-129">Как именованное свойство, определяемое типом расширенного свойства, пространством имен и числовым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-129">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="1e3d4-130">В формате proptag, определяемом типом расширенного свойства и [тегом свойства MAPI](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span><span class="sxs-lookup"><span data-stu-id="1e3d4-130">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="1e3d4-131">В следующих двух таблицах эти форматы описываются как примененные к расширенным свойствам с одним и несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-131">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="1e3d4-132">{_Type_} представляет тип значения или значений расширенного свойства.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-132">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="1e3d4-133">В примерах показаны типы string, integer и массивы этих типов.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-133">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="1e3d4-134">**Действительные форматы идентификаторов для расширенных свойств с одним значением**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-134">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="1e3d4-135">**Формат**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-135">**Format**</span></span>|<span data-ttu-id="1e3d4-136">**Пример**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-136">**Example**</span></span>|<span data-ttu-id="1e3d4-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-137">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="1e3d4-138">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="1e3d4-138">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="1e3d4-139">Определяет свойство по пространству имен (GUID), к которому он принадлежит, и строковое имя.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-139">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="1e3d4-140">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="1e3d4-140">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="1e3d4-141">Определяет свойство по пространству имен (GUID), к которому он принадлежит, и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-141">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="1e3d4-142">"{_Type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="1e3d4-142">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="1e3d4-143">Определяет предопределенное свойство с помощью тега его свойства.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-143">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="1e3d4-144">**Действительные форматы идентификаторов для расширенных свойств с несколькими значениями**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-144">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="1e3d4-145">**Формат**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-145">**Format**</span></span>|<span data-ttu-id="1e3d4-146">**Пример**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-146">**Example**</span></span>|<span data-ttu-id="1e3d4-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1e3d4-147">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="1e3d4-148">"{_тип_} {_guid_} **Name** {_имя_}"</span><span class="sxs-lookup"><span data-stu-id="1e3d4-148">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="1e3d4-149">Определяет свойство с помощью пространства имен (GUID) и имени строки.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-149">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="1e3d4-150">"{_тип_} {_guid_} **Id** {_идентификатор_}"</span><span class="sxs-lookup"><span data-stu-id="1e3d4-150">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="1e3d4-151">Определяет свойство по пространству имен (GUID) и числовому идентификатору.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-151">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="1e3d4-152">"{_Type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="1e3d4-152">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="1e3d4-153">Определяет предопределенное свойство с помощью тега его свойства.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-153">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="1e3d4-154">Используйте один из именованных форматов свойств, чтобы определить одно или несколько расширенных свойств в качестве настраиваемого свойства.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-154">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="1e3d4-155">В двух форматах первый вариант, принимающий строку name (**Name**), является предпочтительным форматом для простоты справки.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-155">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="1e3d4-156">Именованные свойства имеют [идентификаторы свойств](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) в диапазоне 0x8000 – 0xFFFE.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-156">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="1e3d4-157">Используйте формат proptag для доступа к свойствам, предопределенным MAPI или клиентом или сервером и еще не предоставленных в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-157">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="1e3d4-158">Эти свойства имеют идентификаторы свойств в диапазоне 0x0001 — 0x7FFF.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-158">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="1e3d4-159">Не пытайтесь определить настраиваемое свойство с помощью формата proptag.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-159">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="1e3d4-160">Вы можете просмотреть сведения о сопоставлении расширенного свойства с существующим свойством MAPI, например идентификатор свойства или GUID, в статье \[MS-OXPROPS\] Microsoft Corporation, ["Основной список свойств для протоколов Exchange Server"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1e3d4-160">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="1e3d4-161">**Примечание.** После выбора одного формата для идентификатора **id** получайте доступ к этому расширенному свойству, используя только этот формат.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-161">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="1e3d4-162">Операции с API REST</span><span class="sxs-lookup"><span data-stu-id="1e3d4-162">REST API operations</span></span>
 
<span data-ttu-id="1e3d4-163">Ниже приведены операции с расширенными свойствами с одним значением.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-163">Single-value extended property operations:</span></span>

- [<span data-ttu-id="1e3d4-164">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="1e3d4-164">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="1e3d4-165">Получение одного или коллекции экземпляров ресурсов с расширенным свойством с помощью параметра `$expand` или `$filter`</span><span class="sxs-lookup"><span data-stu-id="1e3d4-165">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="1e3d4-166">Ниже приведены операции с расширенными свойствами с несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="1e3d4-166">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="1e3d4-167">Создание расширенного свойства в новом или существующем экземпляре ресурса</span><span class="sxs-lookup"><span data-stu-id="1e3d4-167">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="1e3d4-168">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`</span><span class="sxs-lookup"><span data-stu-id="1e3d4-168">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/extended-properties-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
