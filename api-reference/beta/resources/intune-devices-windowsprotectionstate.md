---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecdc3ab743502ff4aef78fa8923248399ce16f4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803103"
---
# <a name="windowsprotectionstate-resource-type"></a>Тип ресурса windowsProtectionState

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект состояния защиты устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|
|[Обновление windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для объекта состояния защиты устройства. Это идентификатор устройства для устройства.|
|Малварепротектионенаблед|Boolean|Защита от вредоносных программ включена или нет|
|Девицестате|[Виндовсдевицехеалсстате](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|Реалтимепротектионенаблед|Boolean|Защита в режиме реального времени включена или нет?|
|Нетворкинспектионсистеменаблед|Boolean|Система проверки сети включена или нет?|
|Куиккскановердуе|Boolean|Быстрая проверка просрочена или нет?|
|Фуллскановердуе|Boolean|Полная проверка просрочена или нет?|
|Сигнатуреупдатеовердуе|Boolean|Подпись устарела или нет?|
|Ребутрекуиред|Boolean|Требуется переЗагрузка или нет?|
|Фуллсканрекуиред|Boolean|Необходима полная проверка или нет?|
|Енгиневерсион|String|Текущая версия модуля Endpoint Protection|
|Сигнатуреверсион|String|Текущая версия определений вредоносных программ|
|Антималвареверсион|String|Текущая версия защиты от вредоносных программ|
|Ласткуиккскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|Ластфуллскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|Ласткуиккскансигнатуреверсион|String|Последняя версия подписи быстрого сканирования|
|Ластфуллскансигнатуреверсион|String|Версия последней полной проверки подписи|
|lastReportedDateTime|DateTimeOffset|Последнее состояние работоспособности устройства в отчете о времени|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Детектедмалварестате|Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)|Список вредоносных программ для устройств|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





