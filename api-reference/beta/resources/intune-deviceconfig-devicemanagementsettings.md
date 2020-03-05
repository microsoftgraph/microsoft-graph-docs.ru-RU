---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f3c6e3f718cb7b3915daecc700e55b733947530c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526592"
---
# <a name="devicemanagementsettings-resource-type"></a>Тип ресурса deviceManagementSettings

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.|
|isScheduledActionEnabled|Логический|Включена ли функция для запланированного действия для правила.|
|secureByDefault|Boolean|Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.|
|енханцеджаилбреак|Логический|Функция включена или не включена для обнаружения расширенной жаилбреак.|
|девицеинактивитибефореретирементиндай|Int32|Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться. Допустимые значения — от 30 до 270|
|дериведкредентиалпровидер|[дериведкредентиалпровидертипе](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|Производный поставщик учетных данных, который будет использоваться для этой учетной записи. Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|дериведкредентиалурл|String|URI самообслуживания поставщика производных учетных данных.|
|андроиддевицеадминистраторенроллментенаблед|Логический|Свойство, определяющее, включена ли регистрация администратора устройств Android для этой учетной записи.|

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
  "androidDeviceAdministratorEnrollmentEnabled": true
}
```



