---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3329b4e7f3412d62acafdb6a82b5838c9dd93f02
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785418"
---
# <a name="devicemanagementsettings-resource-type"></a>Тип ресурса deviceManagementSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.|
|isScheduledActionEnabled|Boolean|Включена ли функция для запланированного действия для правила.|
|secureByDefault|Boolean|Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.|
|enhancedJailBreak|Логический|Включена функция или нет для расширенного обнаружения побега из тюрьмы.|
|deviceInactivityBeforeRetirementInDay|Int32|Если устройство не проверяется в течение определенного количества дней, данные компании могут быть удалены и устройство не будет под управлением. Допустимые значения от 30 до 270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|Поставщик производных учетных данных для использования для этой учетной записи. Возможные значения: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|Строка|URI самообслуживаемого поставщика учетных данных.|
|androidDeviceAdministratorEnrollmentEnabled|Логический|Свойство, определяющее, включена ли регистрация администратора устройства Android для этой учетной записи.|
|ignoreDevicesForUnsupportedSettingsEnabled|Boolean|Свойство для определения того, следует ли игнорировать неподтверченные параметры соответствия определенным моделям устройств.|
|enableLogCollection|Логический|Определяет, должна ли функция коллекции журналов быть доступной для использования.|

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



