---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea20bce4019ff04c81170b895fd5d5445db027cd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707824"
---
# <a name="devicemanagementsettings-resource-type"></a>Тип ресурса deviceManagementSettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.|
|isScheduledActionEnabled|Boolean|Включена ли функция для запланированного действия для правила.|
|secureByDefault|Boolean|Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.|
|енханцеджаилбреак|Логический|Функция включена или не включена для обнаружения расширенной жаилбреак.|
|девицеинактивитибефореретирементиндай|Int32|Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться. Допустимые значения — от 30 до 270|
|дериведкредентиалпровидер|[дериведкредентиалпровидертипе](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|Производный поставщик учетных данных, который будет использоваться для этой учетной записи. Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|дериведкредентиалурл|Строка|URI самообслуживания поставщика производных учетных данных.|
|андроиддевицеадминистраторенроллментенаблед|Логический|Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.|
|игноредевицесфорунсуппортедсеттингсенаблед|Логический|Свойство, определяющее, следует ли игнорировать неподдерживаемые параметры соответствия для определенных моделей устройств.|
|енаблелогколлектион|Логический|Определяет, доступна ли функция сбора журналов для использования.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true,
  "ignoreDevicesForUnsupportedSettingsEnabled": true,
  "enableLogCollection": true
}
```





