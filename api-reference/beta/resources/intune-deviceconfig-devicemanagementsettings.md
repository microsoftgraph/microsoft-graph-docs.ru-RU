---
title: Тип ресурса deviceManagementSettings
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8238ec075189a138552cb524a22facd99f4d5401
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164269"
---
# <a name="devicemanagementsettings-resource-type"></a>Тип ресурса deviceManagementSettings

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения. Допустимые значения: от 0 до 120|
|isScheduledActionEnabled|Логический|Включена ли функция для запланированного действия для правила.|
|secureByDefault|Boolean|Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.|
|Енханцеджаилбреак|Логический|Функция включена или не включена для обнаружения расширенной жаилбреак.|
|Девицеинактивитибефореретирементиндай|Int32|Когда устройство не будет возвращать указанное количество дней, данные компании могут быть удалены, а устройство не будет управляться. Допустимые значения — от 30 до 270|
|Дериведкредентиалпровидер|[Дериведкредентиалпровидертипе](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|Производный поставщик учетных данных, который будет использоваться для этой учетной записи. Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|Дериведкредентиалурл|String|URI самообслуживания поставщика произВодных учетных данных.|

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
  "derivedCredentialUrl": "String"
}
```




