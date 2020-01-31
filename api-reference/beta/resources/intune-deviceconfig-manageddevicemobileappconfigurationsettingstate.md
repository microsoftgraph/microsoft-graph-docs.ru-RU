---
title: Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате
description: Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d828b57e6ae76e3a0babcc2b27a009e60f7a6407
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636299"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a>Тип ресурса Манажеддевицемобилеаппконфигуратионсеттингстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние параметров конфигурации мобильных приложений для управляемых устройств для данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|setting|Строка|Параметр для отчета|
|settingName|Строка|Локализованное или понятное имя параметра для отчета|
|instanceDisplayName|Строка|Имя экземпляра параметра для отчета|
|state|[комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние соответствия для параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|errorCode|Int64|Код ошибки для параметра|
|errorDescription|Строка|Описание ошибки|
|userId|String|ИД пользователя|
|userName|Строка|Имя пользователя|
|userEmail|Строка|Электронный адрес пользователя|
|userPrincipalName|Строка|Имя участника-пользователя.|
|sources|Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)|Соответствующие политики|
|currentValue|String|Текущее значение параметра на устройстве|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



