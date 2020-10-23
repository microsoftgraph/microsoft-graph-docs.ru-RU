---
title: Тип ресурса deviceConfigurationSettingState
description: Состояние параметра конфигурации определенного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9ce56365b9be8b15f5e92b1aa148e2cf0896824
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726509"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a>Тип ресурса deviceConfigurationSettingState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние параметра конфигурации определенного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|setting|String|Параметр для отчета|
|settingName|String|Локализованное или понятное имя параметра для отчета|
|instanceDisplayName|String|Имя экземпляра параметра для отчета|
|state|[комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние соответствия для параметра. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|errorCode|Int64|Код ошибки для параметра|
|errorDescription|String|Описание ошибки|
|userId|String|ИД пользователя|
|userName|String|Имя пользователя|
|userEmail|String|Электронный адрес пользователя|
|userPrincipalName|String|Имя участника-пользователя.|
|sources|Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)|Соответствующие политики|
|currentValue|String|Текущее значение параметра на устройстве|
|сеттингинстанцеид|Строка|сеттингинстанцеид|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```





