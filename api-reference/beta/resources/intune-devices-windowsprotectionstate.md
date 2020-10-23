---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63ac9a9e5f6dd153238ea2666cf0bffd88ebf9da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731038"
---
# <a name="windowsprotectionstate-resource-type"></a>Тип ресурса windowsProtectionState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|малварепротектионенаблед|Логический|Защита от вредоносных программ включена или нет|
|девицестате|[виндовсдевицехеалсстате](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|реалтимепротектионенаблед|Логический|Защита в режиме реального времени включена или нет?|
|нетворкинспектионсистеменаблед|Логический|Система проверки сети включена или нет?|
|куиккскановердуе|Логический|Быстрая проверка просрочена или нет?|
|фуллскановердуе|Логический|Полная проверка просрочена или нет?|
|сигнатуреупдатеовердуе|Логический|Подпись устарела или нет?|
|ребутрекуиред|Логический|Требуется перезагрузка или нет?|
|фуллсканрекуиред|Логический|Необходима полная проверка или нет?|
|енгиневерсион|Строка|Текущая версия модуля Endpoint Protection|
|сигнатуреверсион|Строка|Текущая версия определений вредоносных программ|
|антималвареверсион|Строка|Текущая версия защиты от вредоносных программ|
|ласткуиккскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|ластфуллскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|ласткуиккскансигнатуреверсион|Строка|Последняя версия подписи быстрого сканирования|
|ластфуллскансигнатуреверсион|Строка|Версия последней полной проверки подписи|
|lastReportedDateTime|DateTimeOffset|Последнее состояние работоспособности устройства в отчете о времени|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|детектедмалварестате|Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)|Список вредоносных программ для устройств|

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





