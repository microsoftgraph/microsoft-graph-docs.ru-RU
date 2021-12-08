---
title: Тип ресурса mobileThreatDefenseConnector
description: Объект, представляющий подключение к партнеру по Mobile Threat Defense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 338366d99bf17cad44b63bfee7ad3fb13709ddf0
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348189"
---
# <a name="mobilethreatdefenseconnector-resource-type"></a>Тип ресурса mobileThreatDefenseConnector

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий подключение к партнеру по Mobile Threat Defense.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileThreatDefenseConnectors](../api/intune-onboarding-mobilethreatdefenseconnector-list.md)|Коллекция [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Получение объекта mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-get.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Создание объекта mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-create.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Создание объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Удаление объекта mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-delete.md)|Нет|Удаляет объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|
|[Обновление объекта mobileThreatDefenseConnector](../api/intune-onboarding-mobilethreatdefenseconnector-update.md)|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)|Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|lastHeartbeatDateTime|DateTimeOffset|Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных|
|partnerState|[mobileThreatPartnerTenantState](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|Синхронизация данных партнер для этой учетной записи. Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.|
|AndroidMobileApplicationManagementEnabled|Boolean|Для Android установите, следует ли использовать данные партнера синхронизации данных во время оценок управления мобильными приложениями (MAM). Для оценки управления мобильными приложениями (MAM) может быть включен только один партнер на платформе.|
|iosMobileApplicationManagementEnabled|Boolean|Для IOS получите или установите, следует ли использовать данные партнера синхронизации данных во время оценок управления мобильными приложениями (MAM). Для оценки управления мобильными приложениями (MAM) может быть включен только один партнер на платформе.|
|androidEnabled|Логическое|Для ОС Android следует указать в настройках, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям|
|iosEnabled|Логическое|Для ОС IOS следует получить или задать настройки, необходимо ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям|
|windowsEnabled|Boolean|Чтобы Windows, получите или установите, следует ли использовать данные партнера синхронизации данных во время оценки соответствия требованиям.|
|macEnabled|Boolean|Для Mac получите или установите, следует ли использовать данные партнера синхронизации данных во время оценки соответствия требованиям.|
|androidDeviceBlockedOnMissingPartnerData|Логическое|Для ОС Android следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям|
|iosDeviceBlockedOnMissingPartnerData|Логическое|Для ОС IOS следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям|
|windowsDeviceBlockedOnMissingPartnerData|Boolean|Для Windows установите, должен ли Intune получать данные от партнера синхронизации данных до маркировки устройства, удовлетворяемой требованиям.|
|macDeviceBlockedOnMissingPartnerData|Boolean|Для Mac получите или установите, должен ли Intune получать данные от партнера по синхронизации данных до маркировки устройства, удовлетворяемой требованиям.|
|partnerUnsupportedOsVersionBlocked|Логическое|Получение или задание настроек, следует ли блокировать устройства на включенных платформах, которые не соответствуют минимальным требованиям к версии партнера по синхронизации данных|
|partnerUnresponsivenessThresholdInDays|Int32|Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.|
|allowPartnerToCollectIOSApplicationMetadata|Boolean|Для устройств IOS администратор может настроить, может ли партнер синхронизации данных также собирать метаданные об установленных приложениях из Intune.|
|allowPartnerToCollectIOSPersonalApplicationMetadata|Boolean|Для устройств IOS администратор может настроить, может ли партнер синхронизации данных также собирать метаданные о лично установленных приложениях из Intune.|
|MicrosoftDefenderForEndpointAttachEnabled|Boolean|При TRUE включено управление профилем конфигурации через Microsoft Defender для конечной точки. При FALSE управление профилем конфигурации с помощью Microsoft Defender для конечной точки отключено.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 1024,
  "allowPartnerToCollectIOSApplicationMetadata": true,
  "allowPartnerToCollectIOSPersonalApplicationMetadata": true,
  "microsoftDefenderForEndpointAttachEnabled": true
}
```




