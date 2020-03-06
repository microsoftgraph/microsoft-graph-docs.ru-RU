---
title: Тип ресурса deviceCompliancePolicySettingState
description: Состояние параметров политики соответствия требованиям для определенного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1d75c82cfdd53d1df51537980487e7f7ed780414
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530817"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a>Тип ресурса deviceCompliancePolicySettingState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние параметров политики соответствия требованиям для определенного устройства.

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
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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




