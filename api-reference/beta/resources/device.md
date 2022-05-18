---
title: Тип ресурса device
description: Представляет устройство, зарегистрированное в каталоге.
ms.localizationpriority: medium
author: sandeo-MSFT
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f8233f2f54a49fbe02f5cb5d51ad5250dbf7fff
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461571"
---
# <a name="device-resource-type"></a>Тип ресурса device

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройство, зарегистрированное в каталоге. Экземпляры device создаются в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется от [directoryObject](directoryobject.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview). Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение device](../api/device-get.md) | [device](device.md) |Чтение свойств и связей объекта устройства.|
|[Список объектов device](../api/device-list.md) | Коллекция [device](device.md)| Получение списка устройств, зарегистрированных в каталоге. |
|[Обновление device](../api/device-update.md) | [device](device.md)  |Обновите свойства объекта устройства. |
|[Удаление device](../api/device-delete.md) | Нет |Удалите объект устройства. |
|[Список memberOf](../api/device-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп и административных единиц, непосредственным участником которых является устройство. |
|[Перечисление транзитивных свойств memberOf](../api/device-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп и административных единиц, в которые входит устройство. Эта операция является транзитивной. |
|[Список экземпляров registeredOwner](../api/device-list-registeredowners.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к зарегистрированным владельцам устройства, из свойства навигации registeredOwners.|
|[Перечисление registeredUsers](../api/device-list-registeredusers.md) |Коллекция [directoryObject](directoryobject.md)| Получение зарегистрированных пользователей устройства из свойства навигации registeredUsers.|
|[Список usageRights](../api/device-list-usagerights.md) | Коллекция [usageRight](usageright.md) | Получение коллекции прав на использование, предоставленных устройству.|
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | Коллекция String | Проверка членства в списке групп. Это транзитивная проверка. |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | Коллекция String | Возвращает все группы, в которые входит устройство. Это транзитивная проверка. |
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | Коллекция String | Проверьте членство в списке групп, роли каталога или объектов административной единицы. |
|[getMemberObjects](../api/directoryobject-checkmemberobjects.md) | Коллекция String | Возвращает все группы, административные единицы и роли каталога, членом которых является устройство. Это транзитивная проверка. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#device-properties).

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Логический| Если учетная запись обеспечена — `true`, в противном случае — `false`. Значение по умолчанию: `true`. <br/><br/> Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). Задать это свойство могут только вызывающие объекты с ролями глобального администратора и администратора облачных устройств.|
|alternativeSecurityIds|Коллекция [alternativeSecurityId](alternativeSecurityId.md)| Только для внутреннего использования. Значение null не допускается. Поддерживает `$filter` (`eq`, `not`, `ge`, `le`). |
|approximateLastSignInDateTime|DateTimeOffset| Тип метки времени представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. `$filter` Поддерживает (`eq`, `ne`, `not`, `ge`, и `le`для `eq` `null` значений) и `$orderBy`. |
|complianceExpirationDateTime|DateTimeOffset| Метка времени, когда устройство больше не считается соответствующим требованиям. Тип метки времени представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|deviceCategory|Строка|Определяемые пользователем свойства заданы Intune автоматически добавлять устройства в группы и упрощать управление устройствами.|
|deviceId|String| Идентификатор, задающийся службой регистрации устройств Azure во время регистрации. Поддерживает `$filter` (`eq`, `ne`, `not`, `startsWith`). |
|deviceMetadata|String| Только для внутреннего использования. Установите значение `null`. |
|deviceOwnership|Строка|Владение устройством. Это свойство задается Intune. Возможные значения: `unknown`, `company`, `personal`.|
|deviceVersion|Int32| Только для внутреннего использования. |
|displayName|String| Отображаемое имя устройства. Обязательный параметр. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`), `$search` и `$orderBy`.  |
|domainName|String|Локальное доменное имя гибридных Azure AD присоединенных устройств. Это свойство задается Intune.|
|enrollmentProfileName|Строка|Профиль регистрации, применяемый к устройству. Например, `Apple Device Enrollment Profile`или `Device enrollment - Corporate device identifiers``Windows Autopilot profile name`. Это свойство задается Intune.|
|enrollmentType|String|Тип регистрации устройства. Это свойство задается Intune. Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
| extensionAttributes | [onPremisesExtensionAttributes](onpremisesextensionattributes.md) | Содержит атрибуты расширения 1–15 для устройства. Отдельные атрибуты расширения невозможно выбрать. Эти свойства хранятся в облаке и могут быть заданы во время создания или обновления объекта устройства в Azure AD. <br><br>Поддерживает `$filter` (`eq`, `not`, `startsWith` и `eq` по `null` значениям).|
|id|String|Уникальный идентификатор устройства. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается. Только для чтения. Поддерживает `$filter` (`eq`, `ne`, `not`, `in`). |
|isCompliant|Boolean|`true` if the device complies with Mobile Device Management (MDM) policies; otherwise, `false`. Только для чтения. Его можно обновить только Intune для любого типа ОС устройства или утвержденного приложения [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для Windows ОС. Поддерживает `$filter` (`eq`, `ne`, `not`).|
|isManaged|Boolean|`true`Значение , если устройство управляется мобильным приложением Управление устройствами (MDM); в противном случае — значение `false`. Его можно обновить только Intune для любого типа ОС устройства или утвержденного приложения [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) для Windows ОС. Поддерживает `$filter` (`eq`, `ne`, `not`). |
|isRooted|Boolean|`true` Значение , если устройство является корневым; `false` Значение , если устройство не работает. Это может быть обновлено только Intune.|
|managementType|String|Канал управления устройством.  Это свойство задается Intune. Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|manufacturer|String| Производитель устройства. Только для чтения. |
|mdmAppId|Строка|Идентификатор приложения, используемый для регистрации устройства в MDM. Только для чтения. Поддерживает `$filter` (`eq`, `ne`, `not`, `startsWith`).|
|model|String| Модель устройства. Только для чтения. |
|onPremisesLastSyncDateTime|DateTimeOffset|Время последней синхронизации объекта с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь в формате UTC 1 января 2014 г. доступна `2014-01-01T00:00:00Z` только для чтения. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
|onPremisesSyncEnabled|Логический|Значение `true` указывает, что этот объект синхронизируется из локального каталога. Значение `false` указывает, что этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Значение `null` указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения. Поддерживает `$filter` (`eq`, `ne`, `not`, `in` и `eq` по `null` значениям). |
|operatingSystem|String| Тип операционной системы на устройстве. Обязательный параметр. `$filter` Поддерживает (`eq`, `ne`, `not`, `ge`, `le`, , и `startsWith`для `eq` `null` значений). |
|operatingSystemVersion|String| Версия операционной системы устройства. Обязательный. `$filter` Поддерживает (`eq`, `ne`, `not`, `ge`, `le`, , и `startsWith`для `eq` `null` значений). |
|physicalIds|Коллекция String| Только для внутреннего использования. Значение NULL не допускается. `$filter` Поддерживает (`eq`, `not`, `ge`, `le`, и `startsWith`подсчитывает пустые коллекции). |
|profileType|Строка|Тип профиля устройства. Возможные значения: `RegisteredDevice` (по умолчанию), `SecureVM`, `Printer`, `Shared`, `IoT`.|
|registrationDateTime|DateTimeOffset|Дата и время регистрации устройства. Тип метки времени представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|systemLabels|Коллекция String| Список меток, примененных системой к устройству. Поддерживает ( `$filter` при`eq` подсчете пустых коллекций). |
|имена узлов|Коллекция String| Список имен узлов для устройства.|
|trustType|String| Тип доверия для присоединенного устройства. Только для чтения. Возможные значения: `Workplace` (указывает на использование собственных личных *устройств),*`AzureAd` (устройства, присоединенные только к облаку), `ServerAd` (устройства, присоединенные к локальному домену, присоединенные к Azure AD). Дополнительные сведения см. в статье [Общие сведения об управлении устройствами в Azure Active Directory](/azure/active-directory/device-management-introduction). |
|name| String | Понятное имя устройства. Возвращается, только если пользователь входит с помощью учетной записи Майкрософт в Project Rome. |
|status | String| Устройство имеет или `online` `offline`. Возвращается, только если пользователь входит с помощью учетной записи Майкрософт в Project Rome. |
|платформа |Строка|Платформа устройства. Возвращается, только если пользователь входит с помощью учетной записи Майкрософт в Project Rome. Возвращается, только если пользователь входит с помощью учетной записи Майкрософт в Project Rome.|
|kind| Строка| Форм-фактор устройства. Возвращается, только если пользователь входит с помощью учетной записи Майкрософт в Project Rome. |
|model| String| Модель устройства. Возвращается, только если пользователь входит с помощью учетной записи Майкрософт в Project Rome. |
|manufacturer| String| Производитель устройства. Возвращается, только если пользователь входит с помощью учетной записи Майкрософт в Project Rome. |

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|Команды  | [коллекция команд](command.md) | Набор команд, отправляемых на это устройство.|
|extensions|Коллекция объектов [extension](extension.md)|Коллекция открытых расширений, определенных для устройства. Только для чтения. Допускается значение null. |
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы и административные единицы, в которые входит это устройство. Только для чтения. Допускается значение null. Поддерживает `$expand`. |
|registeredOwners|Коллекция [directoryObject](directoryobject.md)| Пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца. Только для чтения. Допускается значение null. Поддерживает `$expand`. |
|registeredUsers|Коллекция [directoryObject](directoryobject.md)| Коллекция зарегистрированных пользователей устройства. В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев. Только для чтения. Допускается значение null. Поддерживает `$expand`. |
|transitiveMemberOf |Коллекция [directoryObject](directoryobject.md)| Группы и административные единицы, в которые входит это устройство. Эта операция является транзитивной. Поддерживает `$expand`.  |
|usageRights|Коллекция [usageRight](usageright.md)|Представляет права на использование, предоставленные устройству. |

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
  "extensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
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
