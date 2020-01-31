---
title: Тип ресурса Манажеддевицемобилеаппконфигуратионстате
description: Состояние конфигурации мобильного приложения для управляемого устройства для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3faa3547af9337483f0ded1306e7a64321d345a6
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636297"
---
# <a name="manageddevicemobileappconfigurationstate-resource-type"></a>Тип ресурса Манажеддевицемобилеаппконфигуратионстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние конфигурации мобильного приложения для управляемого устройства для данного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажеддевицемобилеаппконфигуратионстатес](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-list.md)|Коллекция [манажеддевицемобилеаппконфигуратионстате](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Список свойств и связей объектов [манажеддевицемобилеаппконфигуратионстате](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|
|[Получение Манажеддевицемобилеаппконфигуратионстате](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-get.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Чтение свойств и связей объекта [манажеддевицемобилеаппконфигуратионстате](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|
|[Создание Манажеддевицемобилеаппконфигуратионстате](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-create.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Создание нового объекта [манажеддевицемобилеаппконфигуратионстате](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|
|[Удаление Манажеддевицемобилеаппконфигуратионстате](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-delete.md)|Нет|Удаляет объект [манажеддевицемобилеаппконфигуратионстате](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md).|
|[Обновление Манажеддевицемобилеаппконфигуратионстате](../api/intune-deviceconfig-managedDeviceMobileAppConfigurationState-update.md)|[managedDeviceMobileAppConfigurationState](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md)|Обновление свойств объекта [манажеддевицемобилеаппконфигуратионстате](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationState.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|settingStates|Коллекция [манажеддевицемобилеаппконфигуратионсеттингстате](../resources/intune-deviceconfig-managedDeviceMobileAppConfigurationSettingState.md)|**TODO: Добавление описания.**|
|displayName|Строка|Имя политики для policyBase.|
|version|Int32|Версия политики.|
|platformType|[полициплатформтипе](../resources/intune-shared-policyPlatformType.md)|Тип платформы, к которой применяется политика. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|state|[комплианцестатус](../resources/intune-shared-complianceStatus.md)|Состояние соответствия политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32|Количество параметров в политике.|
|userId|String|Уникальный идентификатор пользователя, должен быть GUID|
|userPrincipalName|String|"User Principal Name" (Имя участника-пользователя);|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
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
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024,
  "userId": "String",
  "userPrincipalName": "String"
}
```

