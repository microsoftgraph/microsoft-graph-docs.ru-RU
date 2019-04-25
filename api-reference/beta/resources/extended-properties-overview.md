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
# <a name="outlook-extended-properties-overview"></a>Общие сведения о расширенных свойствах Outlook

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Расширенные свойства позволяют хранить пользовательские данные и специально служат в качестве резервного механизма для приложений, чтобы получать доступ к пользовательским данным для свойств Outlook MAPI, когда эти свойства _еще не представлены в метаданных API Microsoft Graph_. Можно использовать расширенные свойства API REST, чтобы хранить или получать такие пользовательские данные в следующих пользовательских ресурсах:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md);
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md).
- [Задача Outlook](../resources/outlooktask.md)
- [Папка задач Outlook](../resources/outlooktaskfolder.md) 

Или в следующих ресурсах группы Office 365:

- group [event](../resources/event.md);
- [calendar](../resources/calendar.md) для групп
- [post](../resources/post.md) для групп. 

## <a name="use-extended-properties-or-open-extensions"></a>Что использовать — расширенные свойства или открытые расширения

В большинстве часто применяемых сценариев у вас должна быть возможность использования открытых расширений (они представлены объектом [openTypeExtension](../resources/opentypeextension.md) и ранее звались расширениями данных Office 365), чтобы хранить пользовательские данные и получать к ним доступ для экземпляров ресурса в почтовом ящике пользователя. Используйте расширенные свойства, только если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены в [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api).

## <a name="types-of-extended-properties"></a>Типы расширенных свойств

В зависимости от того, собираетесь ли вы хранить одно или несколько значений (одинакового типа) в расширенном свойстве, можно создавать расширенное свойство [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) или [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

Каждый из этих типов определяет свойство по идентификатору **id** и хранит данные в значении **value**. 

Можно использовать идентификатор **id** для получения конкретного экземпляра ресурса с расширенным свойством или фильтровать расширенное свойство с одним значением для получения всех экземпляров с таким свойством. 

**Примечание.** Невозможно использовать API REST для получения всех расширенных свойств конкретного экземпляра в одном вызове.
  

### <a name="id-formats"></a>форматы идентификаторов

**Идентификатор** расширенного свойства можно указать в одном из трех форматов:

- Как именованное свойство, определяемое типом расширенного свойства, пространством имен и строковым именем.
- Как именованное свойство, определяемое типом расширенного свойства, пространством имен и числовым идентификатором.
- В формате proptag, определяемом типом расширенного свойства и [тегом свойства MAPI](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).

В следующих двух таблицах эти форматы описываются как примененные к расширенным свойствам с одним и несколькими значениями. {_Type_} представляет тип значения или значений расширенного свойства. В примерах показаны типы string, integer и массивы этих типов.

**Действительные форматы идентификаторов для расширенных свойств с одним значением**

|**Формат**|**Пример**|**Описание**|
|:---------|:----------|:--------------|
| "{_тип_} {_guid_} **Name** {_имя_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Определяет свойство по пространству имен (GUID), к которому он принадлежит, и строковое имя.         |
| "{_тип_} {_guid_} **Id** {_идентификатор_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | Определяет свойство по пространству имен (GUID), к которому он принадлежит, и числовому идентификатору.  |
| "{_Type_} {_proptag_}"                    | ```"String 0x4001001E"```                                           | Определяет предопределенное свойство с помощью тега его свойства. |

**Действительные форматы идентификаторов для расширенных свойств с несколькими значениями**

|**Формат**|**Пример**|**Описание**|
|:---------|:----------|:--------------|
| "{_тип_} {_guid_} **Name** {_имя_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | Определяет свойство с помощью пространства имен (GUID) и имени строки.         |
| "{_тип_} {_guid_} **Id** {_идентификатор_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | Определяет свойство по пространству имен (GUID) и числовому идентификатору.   |
| "{_Type_} {_proptag_}"                    | ```"StringArray 0x4002101E"```                                           | Определяет предопределенное свойство с помощью тега его свойства. |


Используйте один из именованных форматов свойств, чтобы определить одно или несколько расширенных свойств в качестве настраиваемого свойства. В двух форматах первый вариант, принимающий строку name (**Name**), является предпочтительным форматом для простоты справки. Именованные свойства имеют [идентификаторы свойств](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) в диапазоне 0x8000 – 0xFFFE.

Используйте формат proptag для доступа к свойствам, предопределенным MAPI или клиентом или сервером и еще не предоставленных в Microsoft Graph. Эти свойства имеют идентификаторы свойств в диапазоне 0x0001 — 0x7FFF. Не пытайтесь определить настраиваемое свойство с помощью формата proptag. 

Вы можете просмотреть сведения о сопоставлении расширенного свойства с существующим свойством MAPI, например идентификатор свойства или GUID, в статье \[MS-OXPROPS\] Microsoft Corporation, ["Основной список свойств для протоколов Exchange Server"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).

**Примечание.** После выбора одного формата для идентификатора **id** получайте доступ к этому расширенному свойству, используя только этот формат.

## <a name="rest-api-operations"></a>Операции с API REST
 
Ниже приведены операции с расширенными свойствами с одним значением.

- [Создание расширенного свойства в новом или существующем экземпляре ресурса](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [Получение одного или коллекции экземпляров ресурсов с расширенным свойством с помощью параметра `$expand` или `$filter`](../api/singlevaluelegacyextendedproperty-get.md)

Ниже приведены операции с расширенными свойствами с несколькими значениями.

- [Создание расширенного свойства в новом или существующем экземпляре ресурса](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`](../api/multivaluelegacyextendedproperty-get.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/extended-properties-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
