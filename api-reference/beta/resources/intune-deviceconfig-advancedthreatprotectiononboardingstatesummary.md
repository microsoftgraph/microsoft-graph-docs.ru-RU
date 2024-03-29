---
title: расширенный тип ресурсаThreatProtectionOnboardingStateSummary
description: Windows защиты от угрозы, внося сводку состояния в учетную запись.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1ca587b9ac7a0c886f54260c53329334fa72e27
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101795"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a>расширенный тип ресурсаThreatProtectionOnboardingStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows защиты от угрозы, внося сводку состояния в учетную запись.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Чтение свойств и связей объекта [advancedThreatProtectionOnboardingStateSummary.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|
|[Обновление advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Обновление свойств объекта [advancedThreatProtectionOnboardingStateSummary.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор.|
|unknownDeviceCount|Int32|Количество неизвестных устройств.|
|notApplicableDeviceCount|Int32|Количество неприменимых устройств.|
|compliantDeviceCount|Int32|Количество устройств, соответствующих требованиям.|
|remediatedDeviceCount|Int32|Количество исправленных устройств.|
|nonCompliantDeviceCount|Int32|Количество устройств, не соответствующих требованиям.|
|errorDeviceCount|Int32|Количество устройств с ошибками.|
|conflictDeviceCount|Int32|Количество конфликтующих устройств.|
|notAssignedDeviceCount|Int32|Количество не назначенных устройств|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) collection|Н/Д|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```



