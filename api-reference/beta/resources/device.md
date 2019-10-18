---
title: Тип ресурса device
description: Представляет устройство, зарегистрированное в каталоге. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от directoryObject.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 07e6c8be79d105a15de1e7f0f052ebdc21df3406
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "37581254"
---
# <a name="device-resource-type"></a>Тип ресурса device

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройство, зарегистрированное в каталоге. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от [directoryObject](directoryobject.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение device](../api/device-get.md) | [device](device.md) |Чтение свойств и связей объекта Device.|
|[Список объектов device](../api/device-list.md) | Коллекция [device](device.md)| Получение списка устройств, зарегистрированных в каталоге. |
|[Обновление device](../api/device-update.md) | [device](device.md)  |Обновление свойств объекта Device. |
|[Удаление device](../api/device-delete.md) | Нет |Удаление объекта Device. |
|[Перечисление memberOf](../api/device-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, непосредственным участником которых является устройство. |
|[Перечисление транзитивных свойств memberOf](../api/device-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, участником которых является устройство. Эта операция является транзитивным. |
|[Список экземпляров registeredOwner](../api/device-list-registeredowners.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к зарегистрированным владельцам устройства, из свойства навигации registeredOwners.|
|[Перечисление registeredUsers](../api/device-list-registeredusers.md) |Коллекция [directoryObject](directoryobject.md)| Получение зарегистрированных пользователей устройства из свойства навигации registeredUsers.|
|[checkMemberObjects](../api/device-checkmemberobjects.md) | Коллекция String | Проверка участия в списке группы, роли каталога или объектах административных единиц. |
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
|approximateLastSignInDateTime|DateTimeOffset| Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|комплианцеекспиратиондатетиме|DateTimeOffset| Временная метка, в которой устройство больше не считается совместимым. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|deviceId|Guid| Уникальный идентификатор, задаваемый службой Azure Device Registration Service при регистрации. |
|deviceMetadata|String| Только для внутреннего использования. Задано значение NULL. |
|deviceVersion|Int32| Только для внутреннего использования. |
|displayName|Строка| Отображаемое имя устройства. Обязательный параметр. |
|id|String|Уникальный идентификатор устройства. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается. Только для чтения.|
|isCompliant|Логический|Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**. Только для чтения. С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS.|
|isManaged|Boolean|Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**. С помощью Intune можно обновлять любой тип ОС устройства или [утвержденное приложение MDM](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств Windows OS. |
|manufacturer|String| Производитель устройства. Только для чтения. |
|мдмаппид|String|Идентификатор приложения, используемый для регистрации устройства в MDM. <br><br>Только для чтения. Поддерживает параметр $filter.|
|model|String| Модель устройства. Только для чтения. |
|onPremisesLastSyncDateTime|DateTimeOffset|Время последней синхронизации объекта с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения.|
|operatingSystem|String| Тип операционной системы на устройстве. Обязательный параметр. |
|operatingSystemVersion|String| Версия операционной системы устройства. Обязательный параметр. |
|physicalIds|Коллекция String| Только для внутреннего использования. Значение NULL не допускается. |
|профилетипе|String|Тип профиля устройства. Возможные значения:<br />**Регистереддевице** (по умолчанию)<br />**секуревм**<br />**Printer**<br />**Shared**<br />**Интернета**|
|системлабелс|Коллекция строк| Список меток, примененных к устройству системой. |
|trustType|String| Тип доверия для присоединенного устройства. Только для чтения. Возможные значения: <br />**Workplace**. *Принесенные личные устройства*.<br />**AzureAd**. Устройства, присоединенные только через облако.<br />**ServerAd**. Устройства, присоединенные к Azure Active Directory через локальный домен. Дополнительные сведения см. в статье [Общие сведения об управлении устройствами в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction). |
|Имя| String | Понятное имя устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в составе проекта. |
|Status | String| Устройство подключено к сети или находится в автономном режиме. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в составе проекта. |
|Платформа |String|Платформа устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в составе проекта. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в составе проекта.|
|Kind| Строка| Форм фактор устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в составе проекта. |
|Модель| String| Модель устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в составе проекта. |
|Вычислитель| String| Производитель устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в составе проекта. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция объектов [extension](extension.md)|Коллекция открытых расширений, определенных для устройства. Только для чтения. Допускается значение null.|
|registeredOwners|Коллекция [directoryObject](directoryobject.md)| Пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца. Только для чтения. Допускается значение null.|
|registeredUsers|Коллекция [directoryObject](directoryobject.md)| Коллекция зарегистрированных пользователей устройства. В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев. Только для чтения. Допускается значение null.|
|extensions|Коллекция объектов [extension](extension.md)|Коллекция открытых расширений, определенных для устройства. Допускается значение null.|
|registeredOwners|Коллекция [directoryObject](directoryobject.md)|Пользователи, относящиеся к зарегистрированным владельцам устройства. Только для чтения. Допускается значение null.|
|registeredUsers|Коллекция [directoryObject](directoryobject.md)|Зарегистрированные пользователи устройства. Только для чтения. Допускается значение null.|
|Команды  | Коллекция [команд](command.md) | Набор команд, отправляемых на это устройство|

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
  "complianceExpirationDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "mdmAppId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "profileType": "string",
  "systemLabels": ["string"],
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
  "suppressions": []
}
-->
