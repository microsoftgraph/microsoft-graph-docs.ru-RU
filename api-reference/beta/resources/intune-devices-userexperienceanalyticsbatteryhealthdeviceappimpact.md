---
title: тип ресурса userExperienceAnalyticsBatteryHealthDeviceAppImpact
description: Объект воздействия на приложение приложения для анализа пользовательского интерфейса содержит сведения об использовании аккумулятора на уровне приложения для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d6ea7bbec4f14daf98333e76d280d7d4b539e1b
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697444"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceappimpact-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthDeviceAppImpact

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект воздействия на приложение приложения для анализа пользовательского интерфейса содержит сведения об использовании аккумулятора на уровне приложения для данного устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейExperienceAnalyticsBatteryHealthDeviceAppImpacts](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-list.md)|[коллекция userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Список свойств и связей [объектов userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|
|[Get userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-get.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Ознакомьтесь с свойствами и отношениями [объекта userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|
|[Создание userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-create.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Создание нового [объекта userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|
|[Удаление userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md).|
|[Обновление userExperienceAnalyticsBatteryHealthDeviceAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact-update.md)|[userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта приложения-приложения для аналитики пользовательского интерфейса.|
|deviceId|String|Уникальный идентификатор устройства, идентификатор устройства Intune DeviceID или SCCM.|
|appName|String|Имя приложения. Например: oltk.exe|
|appDisplayName|String|Удобное для пользователя имя отображения приложения. Например: Outlook|
|appPublisher|String|Издатель приложения. Например: корпорация Майкрософт|
|isForegroundApp|Логический|верно, если у пользователя было активное взаимодействие с приложением.|
|batteryUsagePercentage|Double|Процент общей мощности батареи, используемой этим приложением, когда устройство не подключено к заряду переменного тока, составляет более 14 дней. Единица в процентах. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact",
  "id": "String (identifier)",
  "deviceId": "String",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "isForegroundApp": true,
  "batteryUsagePercentage": "4.2"
}
```



