---
title: Тип ресурса zebraFotaDeploymentSettings
description: Сложный тип развертывания Zebra FOTA, описывающий параметры, необходимые для создания развертывания FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b055ae91e93919a3f6b8af63d7ae7a207ffaaac
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213598"
---
# <a name="zebrafotadeploymentsettings-resource-type"></a>Тип ресурса zebraFotaDeploymentSettings

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип развертывания Zebra FOTA, описывающий параметры, необходимые для создания развертывания FOTA.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceModel|String|Развертывание обновления только для устройств с этой моделью.|
|updateType|[zebraFotaUpdateType](../resources/intune-androidfotaservice-zebrafotaupdatetype.md)|Тип обновления развертывания. Возможные значения : custom, latest и auto. Если задан пользовательский режим, запрос должен предоставлять значения артефактов. При установке последнего типа последнее выпущенное обновление становится целевой ОС. Если указана последняя версия, целевые значения встроенного ПО не требуются. Примечание. Последняя версия может обновить устройство до новой версии Android. Если задано значение "Автоматически", устройство всегда ищет последний доступный пакет и пытается обновить его каждый раз, когда доступен новый пакет. Это продолжается до тех пор, пока администратор не отменит автоматическое обновление. В то время как другие режимы возвращают идентификатор, начиная с FOTA-x, автоматический режим возвращает идентификатор, начиная с AUTO-x. Возможные значения: `custom`, `latest`, `auto`, `unknownFutureValue`.|
|timeZoneOffsetInMinutes|Int32|Этот атрибут указывает смещение времени развертывания (например,`180` `+03:00``-270` представляет смещение и смещение ).`-04:30` Смещение времени — это часовой пояс, в котором находятся устройства. Данные начала и окончания развертывания используют этот часовой пояс.|
|firmwareTargetBoardSupportPackageVersion|Строка|Пакет поддержки платы развертывания (BSP). Например, "01.18.02.00"). Требуется только для пользовательского типа обновления.|
|firmwareTargetPatch|Строка|Имя целевого исправления (например, "U06"). Требуется только для пользовательского типа обновления.|
|firmwareTargetOsVersion|String|Целевая версия ОС (например, "8.1.0"). Требуется только для пользовательского типа обновления.|
|scheduleMode|[ZebraFotaScheduleMode](../resources/intune-androidfotaservice-zebrafotaschedulemode.md)|Режим расписания установки развертывания. Значение по умолчанию — installNow. Все даты и время запланированных развертываний находятся в часовом поясе устройства. Для параметра "Установить сейчас" дата и время находятся в формате UTC (то же дата и время в любой точке мира). Возможные значения: `installNow`, `scheduled`, `unknownFutureValue`.|
|scheduleDurationInDays|Int32|Максимум 28 дней. Значение по умолчанию — 28 дней. Последовательность дат: 1) Дата начала загрузки. 2) Дата начала установки. 3) Дата окончания расписания. Если какие-либо из значений не указаны, используется дата, указанная на предыдущем шаге последовательности. Если значения не указаны, используется строковое значение текущего формата UTC.|
|downloadRuleNetworkType|[zebraFotaNetworkType](../resources/intune-androidfotaservice-zebrafotanetworktype.md)|Скачайте тип сети, как описано в разделе "zebraFotaNetworkType". Значение по умолчанию: any. Возможные значения: `any`, `wifi`, `cellular`, `wifiAndCellular`, `unknownFutureValue`.|
|downloadRuleStartDateTime|DateTimeOffset|Дата и время в часовом поясе устройства, когда начнется скачивание (например, ). `2018-07-25T10:20:32` Значение по умолчанию — UTC, а максимальное значение — 10 дней с создания развертывания.|
|installRuleStartDateTime|DateTimeOffset|Дата и время начала установки в часовом поясе устройства. По умолчанию — скачайте startDate, если настроено, в противном случае значение по умолчанию — NOW. Игнорируется, если для типа обновления развертывания задано значение auto.|
|installRuleWindowStartTime|TimeOfDay|Время суток (00:00:00–23:30:00), когда должна начаться установка. Время выражается в 24-часовом формате в формате чч:мм и находится в часовом поясе устройства. По умолчанию — 00:00:00. Учитывается для всех значений типа обновления, включая AUTO.|
|installRuleWindowEndTime|TimeOfDay|Время суток, после которого не удается начать установку. Возможный диапазон: от 00:30:00 до 23:59:59. Значение должно быть больше значения installRuleWindowStartTime на 30 минут. Время выражается в 24-часовом формате в формате чч:мм и находится в часовом поясе устройства. По умолчанию — 23:59:59. Учитывается для всех значений типа обновления, включая AUTO.|
|batteryRuleMinimumBatteryLevelPercentage|Int32|Минимальный уровень заряда батареи (%), необходимый для скачивания и установки. Значение по умолчанию: -1 (системные значения по умолчанию). Максимальное значение — 100.|
|batteryRuleRequireCharger|Логический|Флаг, указывающий, требуется ли зарядное приложение. Если задано значение false, клиент может установить обновления независимо от того, находится ли устройство в зарядной установке или из нее. Применяется только для установки. Значение по умолчанию: false.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeploymentSettings",
  "deviceModel": "String",
  "updateType": "String",
  "timeZoneOffsetInMinutes": 1024,
  "firmwareTargetBoardSupportPackageVersion": "String",
  "firmwareTargetPatch": "String",
  "firmwareTargetOsVersion": "String",
  "scheduleMode": "String",
  "scheduleDurationInDays": 1024,
  "downloadRuleNetworkType": "String",
  "downloadRuleStartDateTime": "String (timestamp)",
  "installRuleStartDateTime": "String (timestamp)",
  "installRuleWindowStartTime": "String (time of day)",
  "installRuleWindowEndTime": "String (time of day)",
  "batteryRuleMinimumBatteryLevelPercentage": 1024,
  "batteryRuleRequireCharger": true
}
```




