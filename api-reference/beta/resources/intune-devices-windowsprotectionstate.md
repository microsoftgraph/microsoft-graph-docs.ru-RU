---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbacf6bacdb368418ad2338078e52885b208d69d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941655"
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
|id|Строка|Уникальный идентификатор для объекта состояния защиты устройства. Это идентификатор устройства для устройства.|
|Малварепротектионенаблед|Логический|Защита от вредоносных программ включена или нет|
|Девицестате|[Виндовсдевицехеалсстате](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|Реалтимепротектионенаблед|Логический|Защита в режиме реального времени включена или нет?|
|Нетворкинспектионсистеменаблед|Логический|Система проверки сети включена или нет?|
|Куиккскановердуе|Логический|Быстрая проверка просрочена или нет?|
|Фуллскановердуе|Логический|Полная проверка просрочена или нет?|
|Сигнатуреупдатеовердуе|Логический|Подпись устарела или нет?|
|Ребутрекуиред|Логический|Требуется перезагрузка или нет?|
|Фуллсканрекуиред|Логический|Необходима полная проверка или нет?|
|Енгиневерсион|Строка|Текущая версия модуля Endpoint Protection|
|Сигнатуреверсион|Строка|Текущая версия определений вредоносных программ|
|Антималвареверсион|Строка|Текущая версия защиты от вредоносных программ|
|Ласткуиккскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|Ластфуллскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|Ласткуиккскансигнатуреверсион|Строка|Последняя версия подписи быстрого сканирования|
|Ластфуллскансигнатуреверсион|Строка|Версия последней полной проверки подписи|
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




