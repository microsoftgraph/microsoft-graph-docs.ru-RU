---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f88561d91c4560038027245291f8a04ab270fa22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469255"
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
|енханцеджаилбреак|Boolean|Функция включена или не включена для обнаружения расширенной жаилбреак.|
|девицеинактивитибефореретирементиндай|Int32|Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться. Допустимые значения — от 30 до 270|
|дериведкредентиалпровидер|[дериведкредентиалпровидертипе](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|Производный поставщик учетных данных, который будет использоваться для этой учетной записи. Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|дериведкредентиалурл|String|URI самообслуживания поставщика производных учетных данных.|
|андроиддевицеадминистраторенроллментенаблед|Boolean|Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.|
|игноредевицесфорунсуппортедсеттингсенаблед|Boolean|Свойство, определяющее, следует ли игнорировать неподдерживаемые параметры соответствия для определенных моделей устройств.|

## <a name="relationships"></a>Отношения
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
  "ignoreDevicesForUnsupportedSettingsEnabled": true
}
```



