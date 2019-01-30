---
title: Тип ресурса device
description: Представляет устройство, зарегистрированные в каталоге. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1279a39f7aa8983697b980fd6cce44c203d1883e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641374"
---
# <a name="device-resource-type"></a>Тип ресурса device

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройство, зарегистрированные в каталоге. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от [directoryObject](directoryobject.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение device](../api/device-get.md) | [device](device.md) |Чтение свойства и связи объекта устройства.|
|[Список объектов device](../api/device-list.md) | Коллекция [device](device.md)| Получение списка устройств, зарегистрированных в каталоге. |
|[Обновление device](../api/device-update.md) | [device](device.md)  |Обновляет свойства объекта устройств. |
|[Удаление device](../api/device-delete.md) | Нет |Удалите объект устройства. |
|[Перечисление memberOf](../api/device-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, которые устройство является непосредственным членом. |
|[Перечисление транзитивных свойств memberOf](../api/device-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, которые устройства. Эта операция транзитивное. |
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
|accountEnabled|Boolean| Если учетная запись обеспечена — значение **true**, в противном случае — **false**. значение по умолчанию — true.|
|alternativeSecurityIds|Коллекция alternativeSecurityId| Только для внутреннего использования. Значение NULL не допускается. |
|approximateLastSignInDateTime|DateTimeOffset| Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|deviceId|Guid| Уникальный идентификатор, задаваемый службой Azure Device Registration Service при регистрации. |
|deviceMetadata|String| Только для внутреннего использования. Задано значение NULL. |
|deviceVersion|Int32| Только для внутреннего использования. |
|displayName|String| Отображаемое имя устройства. Обязательный параметр. |
|id|String|Уникальный идентификатор устройства. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается. Только для чтения.|
|isCompliant|Boolean|Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**. Только для чтения. Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.|
|isManaged|Boolean|Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM). В противном случае используется значение **false**. Это можно обновить, путем Intune для любого типа операционная система устройства или [утвержденных MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows. |
|onPremisesLastSyncDateTime|DateTimeOffset|Время последней синхронизации объекта с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения.|
|operatingSystem|String| Тип операционной системы на устройстве. Обязательный параметр. |
|operatingSystemVersion|String| Версия операционной системы устройства. Обязательный. |
|physicalIds|Коллекция String| Только для внутреннего использования. Значение NULL не допускается. |
|trustType|String| Тип доверия для присоединенного устройства. Только для чтения. Возможные значения: <br />**Workplace**. *Принесенные личные устройства*.<br />**AzureAd**. Устройства, присоединенные только через облако.<br />**ServerAd**. Устройства, присоединенные к Azure Active Directory через локальный домен. Дополнительные сведения см. в статье [Общие сведения об управлении устройствами в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction). |
|Имя| String | Понятное имя устройства. Возвращается только при входе пользователя с учетной записью Майкрософт в составе рим проекта. |
|Состояние | String| Устройство является сетевым и автономным. Возвращается только при входе пользователя с учетной записью Майкрософт в составе рим проекта. |
|Платформа |String|Платформа устройства. Возвращается только при входе пользователя с учетной записью Майкрософт в составе рим проекта. Возвращается только при входе пользователя с учетной записью Майкрософт в составе рим проекта.|
|Kind| String| Форм-фактора устройства. Возвращается только при входе пользователя с учетной записью Майкрософт в составе рим проекта. |
|Model| String| Модель устройства. Возвращается только при входе пользователя с учетной записью Майкрософт в составе рим проекта. |
|Производитель| String| Производителя устройства. Возвращается только при входе пользователя с учетной записью Майкрософт в составе рим проекта. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для устройства. Только для чтения. Допускается значение null.|
|registeredOwners|Коллекция [directoryObject](directoryobject.md)| Пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца. Только для чтения. Допускается значение null.|
|registeredUsers|Коллекция [directoryObject](directoryobject.md)| Коллекция зарегистрированных пользователей устройства. В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев. Только для чтения. Допускается значение null.|
|extensions|Коллекция [extension](extension.md)|Коллекция open расширения, определенные для устройства. Допускается значение null.|
|registeredOwners|Коллекция [directoryObject](directoryobject.md)|Пользователи, относящиеся к зарегистрированным владельцам устройства. Только для чтения. Допускается значение null.|
|registeredUsers|Коллекция [directoryObject](directoryobject.md)|Зарегистрированные пользователи устройства. Только для чтения. Допускается значение null.|
|команды | Collection(Microsoft.Graph.Command) | Набор команд, отправленные на это устройство|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
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
  "trustType": "string",
  "Name": "string",
  "Status": "string",
  "Platform": "string",
  "Kind": "string",
  "Model": "string",
  "Manufacturer": "string"
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/device.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
