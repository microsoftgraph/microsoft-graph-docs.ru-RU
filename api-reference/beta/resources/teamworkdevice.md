---
title: тип ресурса teamworkDevice
description: Представляет сведения о устройстве с Microsoft Teams, которое предназначено для клиента.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7cd91f9901c02d1008e5c08a72c47e416222ab75
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262717"
---
# <a name="teamworkdevice-resource-type"></a>тип ресурса teamworkDevice

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о устройстве с Microsoft Teams, которое предназначено для клиента.

Наследуется [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список teamworkDevices](../api/teamworkdevice-list.md)|[teamworkDevice collection](../resources/teamworkdevice.md)|Получите список всех устройств с Microsoft Teams, которые были предусмотрены для клиента.|
|[Get teamworkDevice](../api/teamworkdevice-get.md)|[teamworkDevice](../resources/teamworkdevice.md)|Получите свойства устройства с Microsoft Teams включенной поддержкой.|
|[перезапуск](../api/teamworkdevice-restart.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Перезапустите указанное Microsoft Teams устройство с включенной поддержкой.|
|[runDiagnostics](../api/teamworkdevice-rundiagnostics.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Запуск и создание журналов диагностики для указанного Microsoft Teams включенного устройства.|
|[updateSoftware](../api/teamworkdevice-updatesoftware.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Обновление программного обеспечения для Microsoft Teams устройства с включенной поддержкой.|
|[Операции со списком](../api/teamworkdeviceoperation-list.md)|[коллекция teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Получите список операций, которые работают на устройстве с Teams с включенной поддержкой.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|activityState|teamworkDeviceActivityState|Состояние активности устройства. Допустимые значения: `unknown`, `busy`, `idle`, `unavailable`, `unknownFutureValue`.|
|companyAssetTag|String|Тег активов компании, назначенный администратором на устройстве.|
|createdBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, который зарегистрировал устройство в клиенте.|
|createdDateTime|DateTimeOffset|Дата и время регистрации устройства в клиент.|
|currentUser|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Подписанный пользователь на устройстве.|
|deviceType|[teamworkDeviceType](../resources/teamworkdevice.md#teamworkdevicetype-values)|Тип устройства. Возможные значения: `unknown`, , `teamsRoom``ipPhone`, , `surfaceHub`, `collaborationBar`, `teamsDisplay`, `sip``touchConsole``lowCostPhone``teamsPanel``unknownFutureValue`.|
|hardwareDetail|[teamworkHardwareDetail](../resources/teamworkhardwaredetail.md)|Коллекция свойств, связанных с оборудованием. Например, **oemSerialNumber** и **model**.|
|healthStatus|[teamworkDeviceHealthStatus](../resources/teamworkdevice.md#teamworkdevicehealthstatus-values)|Состояние здоровья устройства. Допустимые значения: `unknown`, `offline`, `critical`, `nonUrgent`, `healthy`, `unknownFutureValue`.|
|id|String|Идентификатор устройства. Наследуется [от сущности](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, который в последний раз изменил сведения об устройстве.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения деталей устройства.|
|notes|String|Заметки, добавленные администратором на устройство.|


### <a name="teamworkdevicetype-values"></a>значения teamworkDeviceType

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|unknown|0|Неизвестное устройство.|
|ipPhone|1|IP Телефон устройства — это настольные телефоны для пользователей, которые могут принимать звуковые вызовы или присоединяться к собраниям.|
|teamsRoom|2|Комнаты Microsoft Teams — Windows устройства на основе IoT, предназначенные для расширения возможности проведения собраний в конференц-зале.|
|surfaceHub|3|Surface Hub устройства — это устройства, установленные на стене или на стендах на роликах, с интерактивной доской.|
|collaborationBar|4|Бары совместной Комнаты Microsoft Teams на Android, используемые для небольших пространств собраний.|
|teamsDisplay|5|Teams устройства отображения — это эволюция Teams телефонов. Эти устройства являются категорией специальных устройств с Teams, которые имеют сенсорный сенсорный экран с сенсорным экраном и без рук с питанием от Кортана.|
|touchConsole|6 |Сенсорные устройства консоли являются необязательными периферийными устройствами для Комнаты Teams android для выполнения всех операций устройства.|
|lowCostPhone|7 |Недорогие телефонные устройства являются экономически эффективными Microsoft Teams телефонов.|
|teamsPanel|8 |Microsoft Teams панели — это компактные сенсорные устройства, на которые отображаются сведения о собраниях, запланированные Teams.|
|sip|9 |Устройства протокола инициации сеансов, Teams вызовы с шлюзом SIP от Майкрософт.|
|unknownFutureValue|10 |Эволюционирующее значение sentinel. Не следует использовать.|


### <a name="teamworkdevicehealthstatus-values"></a>значения teamworkDeviceHealthStatus

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|unknown|0|Неизвестное состояние здоровья.|
|автономный режим|1|Устройство находится в автономном режиме и не может использоваться.|
|критически важное значение|2|Состояние требует срочного внимания и действий, так как оно может существенно повлиять на производительность устройства или сделать его непригодным для звонков или собраний.|
|nonUrgent|3|Состояние требует внимания из-за проблем или уведомлений, которые могут иметь минимальное влияние на производительность устройства в Интернете.|
|здоровый|4|Устройство находится в режиме онлайн и находится в хорошем состоянии.|
|unknownFutureValue|5|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|действие|[teamworkDeviceActivity](../resources/teamworkdeviceactivity.md)|Свойства действий, которые изменяются в зависимости от использования устройства.|
|configuration|[teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md)|Свойства конфигурации устройства.|
|здоровье|[teamworkDeviceHealth](../resources/teamworkdevicehealth.md)|Свойства здоровья устройства.|
|operations|[коллекция teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Операции async на устройстве.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDevice",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDevice",
  "activityState": "String",
  "companyAssetTag": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "currentUser": {
    "@odata.type": "microsoft.graph.teamworkUserIdentity"
  },
  "deviceType": "String",
  "hardwareDetail": {
    "@odata.type": "microsoft.graph.teamworkHardwareDetail"
  },
  "healthStatus": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "notes": "String"
}
```

