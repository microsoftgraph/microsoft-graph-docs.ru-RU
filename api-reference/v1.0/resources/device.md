---
title: Тип ресурса device
description: Представляет устройство, зарегистрированное в организации. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab03eed26f5e34c2ac149815b3ba66b37fc2090c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984999"
---
# <a name="device-resource-type"></a>Тип ресурса device

Представляет устройство, зарегистрированное в организации. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от [directoryObject](directoryobject.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение device](../api/device-get.md) | [device](device.md) |Считывание свойств и отношений объекта device.|
|[Список объектов device](../api/device-list.md) | Коллекция [device](device.md)| Получение списка устройств, зарегистрированных в каталоге. |
|[Обновление device](../api/device-update.md) | [device](device.md) |Обновление свойств, принадлежащих объекту device. |
|[Удаление device](../api/device-delete.md) | Нет |Удаление объекта device. |
|[Перечисление memberOf](../api/device-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, которые устройство является непосредственным членом. |
|[Перечисление registeredOwners](../api/device-list-registeredowners.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к зарегистрированным владельцам устройства, из свойства навигации registeredOwners.|
|[Перечисление registeredUsers](../api/device-list-registeredusers.md) |Коллекция [directoryObject](directoryobject.md)| Получение зарегистрированных пользователей устройства из свойства навигации registeredUsers.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| Если учетная запись обеспечена — значение **true**, в противном случае — **false**. Обязательный параметр.|
|alternativeSecurityIds|Коллекция alternativeSecurityId| Только для внутреннего использования. Значение NULL не допускается. |
|approximateLastSignInDateTime|DateTimeOffset| Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|deviceId|string| Уникальный идентификатор, задаваемый службой Azure Device Registration Service при регистрации. |
|deviceMetadata|String| Только для внутреннего использования. Задано значение NULL. |
|deviceVersion|Int32| Только для внутреннего использования. |
|displayName|String|Отображаемое имя устройства. Обязательный параметр. |
|id|Строка|Уникальный идентификатор устройства. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается. Только для чтения.|
|isCompliant|Boolean|Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**. Только для чтения. Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.|
|isManaged|Boolean|Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM). В противном случае используется значение **false**. Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows. |
|onPremisesLastSyncDateTime|DateTimeOffset|Время последней синхронизации объекта с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения. |
|operatingSystem|String| Тип операционной системы на устройстве. Обязательный параметр. |
|operatingSystemVersion|Строка|Версия операционной системы на устройстве. Обязательный параметр. |
|physicalIds|Коллекция String| Только для внутреннего использования. Значение NULL не допускается. |
|trustType|String| Тип доверия для присоединенного устройства. Только для чтения. Возможные значения: <br />**Workplace**. *Принесенные личные устройства*.<br />**AzureAd**. Устройства, присоединенные только через облако.<br />**ServerAd**. Устройства, присоединенные к Azure Active Directory через локальный домен. Дополнительные сведения см. в статье [Общие сведения об управлении устройствами в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction). |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для устройства. Только для чтения. Допускается значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы, в которых состоит эта группа. Методы HTTP: GET (поддерживается для всех групп). Только для чтения. Допускается значение null.|
|registeredOwners|Коллекция [directoryObject](directoryobject.md)|Пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца. Только для чтения. Допускается значение null. |
|registeredUsers|Коллекция [directoryObject](directoryobject.md)|Коллекция зарегистрированных пользователей устройства. В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
