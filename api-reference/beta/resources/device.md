---
title: Тип ресурса device
description: Представляет устройство, зарегистрированное в каталоге.
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fa201a61b1b2dd126cd75a9e90be1f6ec4b34d5e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721649"
---
# <a name="device-resource-type"></a>Тип ресурса device

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройство, зарегистрированное в каталоге. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от [directoryObject](directoryobject.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение device](../api/device-get.md) | [device](device.md) |Чтение свойств и связей объекта устройства.|
|[Список объектов device](../api/device-list.md) | Коллекция [device](device.md)| Получение списка устройств, зарегистрированных в каталоге. |
|[Обновление device](../api/device-update.md) | [device](device.md)  |Обновление свойств объекта устройства. |
|[Удаление device](../api/device-delete.md) | Нет |Удаление объекта устройства. |
|[Перечисление memberOf](../api/device-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, в которые устройство входит напрямую. |
|[Перечисление транзитивных свойств memberOf](../api/device-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп, в которые входит устройство. Эта операция является транзитной. |
|[Список экземпляров registeredOwner](../api/device-list-registeredowners.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к зарегистрированным владельцам устройства, из свойства навигации registeredOwners.|
|[Перечисление registeredUsers](../api/device-list-registeredusers.md) |Коллекция [directoryObject](directoryobject.md)| Получение зарегистрированных пользователей устройства из свойства навигации registeredUsers.|
|[Список usageRights](../api/device-list-usagerights.md) | Коллекция [usageRight](usageright.md) | Получите коллекцию прав на использование, предоставленных устройству.|
|[checkMemberObjects](../api/device-checkmemberobjects.md) | Коллекция String | Проверьте членство в списке групп, ролей каталогов или объектов административных единиц. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| Значение **true** указывает, что учетная запись включена. В противном случае используется значение **false**. значение по умолчанию верно.|
|alternativeSecurityIds|Коллекция alternativeSecurityId| Только для внутреннего использования. Значение NULL не допускается. |
|approximateLastSignInDateTime|DateTimeOffset| Тип timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|complianceExpirationDateTime|DateTimeOffset| Время, когда устройство больше не считается совместимым. Тип timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|deviceCategory|String|Свойство, определенное пользователем, задаваемо Intune для автоматического добавления устройств в группы и упрощения управления устройствами.|
|deviceId|Guid| Уникальный идентификатор, задаваемый службой Azure Device Registration Service при регистрации. |
|deviceMetadata|String| Только для внутреннего использования. Задано значение NULL. |
|deviceOwnership|String|Владение устройством. Это свойство заданной Intune. Возможные значения: неизвестные, компании, личные.|
|deviceVersion|Int32| Только для внутреннего использования. |
|displayName|String| Отображаемое имя устройства. Обязательный параметр. |
|domainName|String|Локальное доменное имя гибридного Azure AD присоединилось к устройствам. Это свойство заданной Intune.|
|enrollmentProfileName|String|Профиль регистрации, примененный к устройству. Например, профиль регистрации устройств Apple, регистрация устройств — идентификаторы корпоративных устройств или имя профиля Автопилота Windows. Это свойство заданной Intune.|
|enrollmentType|String|Тип регистрации устройства. Это свойство заданной Intune. Возможные значения: неизвестные, userEnrollment, deviceEnrollmentManager, appleBulkWithUser, appleBulkWithoutUser, windowsAzureADJoin, windowsBulkUserless, windowsAutoEnrollment, windowsBulkAzureDomainJoin, windowsCoManagement.|
|id|String|Уникальный идентификатор устройства. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается. Только для чтения.|
|isCompliant|Boolean|Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**. Только для чтения. Это может быть обновлено только intune для любого типа ОС устройства или утвержденным [приложением MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows.|
|isManaged|Boolean|Используется значение **true**, если устройство контролируется с помощью приложения для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**. Это может быть обновлено только intune для любого типа ОС устройства или утвержденным [приложением MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для устройств ОС Windows. |
|isRooted|Boolean|**true,** если устройство корневое; **false,** если устройство не работает в тюрьме. Это может быть обновлено только в Intune.|
|managementType|String|Канал управления устройством.  Это свойство заданной Intune. Возможные значения: eas, mdm, easMdm, intuneClient, easIntuneClient, configurationManagerClient, configurationManagerClientMdm, configurationManagerClientMdmEas, unknown, jamf, googleCloudDevicePolicyController.|
|manufacturer|String| Производитель устройства. Только для чтения. |
|mdmAppId|String|Идентификатор приложения, используемый для регистрации устройства в MDM. <br><br>Только для чтения. Поддерживает параметр $filter.|
|model|String| Модель устройства. Только для чтения. |
|onPremisesLastSyncDateTime|DateTimeOffset|Последний раз, когда объект синхронизировался с локальной каталоги. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полуночный UTC 1 января 2014 г. является `2014-01-01T00:00:00Z` только для чтения. |
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения.|
|operatingSystem|String| Тип операционной системы на устройстве. Обязательный параметр. |
|operatingSystemVersion|String| Версия операционной системы устройства. Обязательный параметр. |
|physicalIds|Коллекция String| Только для внутреннего использования. Значение NULL не допускается. |
|profileType|String|Тип профиля устройства. Возможные значения:<br />**RegisteredDevice** (по умолчанию)<br />**SecureVM**<br />**Printer**<br />**Shared**<br />**IoT**|
|registrationDateTime|DateTimeOffset|Дата и время регистрации устройства. Тип timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|systemLabels|Коллекция объектов string| Список меток, применяемых к устройству системой. |
|hostNames|Коллекция объектов string| Список имен hostNames для устройства.|
|trustType|String| Тип доверия для присоединенного устройства. Только для чтения. Возможные значения: <br />**Workplace**. *Принесенные личные устройства*.<br />**AzureAd**. Устройства, присоединенные только через облако.<br />**ServerAd**. Устройства, присоединенные к Azure Active Directory через локальный домен. Дополнительные сведения см. в статье [Общие сведения об управлении устройствами в Azure Active Directory](/azure/active-directory/device-management-introduction). |
|Имя| String | Удобное имя устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в рамках Project Rome. |
|Состояние | String| Устройство находится в сети или автономном режиме. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в рамках Project Rome. |
|Платформа |String|Платформа устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в рамках Project Rome. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в рамках Project Rome.|
|Kind| Строка| Форм-фактор устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в рамках Project Rome. |
|Модель| String| Модель устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в рамках Project Rome. |
|Производитель| String| Производитель устройства. Возвращается только в том случае, если пользователь входит в учетную запись Майкрософт в рамках Project Rome. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для устройства. Только для чтения. Допускается значение null.|
|registeredOwners|Коллекция [directoryObject](directoryobject.md)| Пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца. Только для чтения. Допускается значение null.|
|registeredUsers|Коллекция [directoryObject](directoryobject.md)| Коллекция зарегистрированных пользователей устройства. В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев. Только для чтения. Допускается значение null.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для устройства. Допускается значение null.|
|Команды  | [коллекция](command.md) команд | Набор команд, отправленных на это устройство|
|usageRight|Коллекция [usageRight](usageright.md)|Представляет права использования, предоставленные устройству. |

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
  "deviceCategory": "string",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceOwnership": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "domainName": "string",
  "enrollmentProfileName": "string",
  "enrollmentType": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "isRooted": true,
  "mdmAppId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "profileType": "string",
  "registrationDateTime": "String (timestamp)",
  "systemLabels": ["string"],
  "hostNames" : ["string"],
  "trustType": "string",
  "Name": "string",
  "Status": "string",
  "Platform": "string",
  "Kind": "string",
  "Model": "string",
  "managementType": "string",
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
