---
title: тип ресурса userExperienceAnalyticsBatteryHealthAppImpact
description: Объект воздействия приложения на здоровье приложения для аналитики пользовательского интерфейса содержит сведения об использовании батареи на уровне приложения для клиента.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef986108396bd1dbdb013be810aea01ebd1e6627
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342414"
---
# <a name="userexperienceanalyticsbatteryhealthappimpact-resource-type"></a>тип ресурса userExperienceAnalyticsBatteryHealthAppImpact

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект воздействия приложения на здоровье приложения для аналитики пользовательского интерфейса содержит сведения об использовании батареи на уровне приложения для клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsBatteryHealthAppImpacts](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-list.md)|[коллекция userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Список свойств и связей [объектов userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|
|[Get userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-get.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Чтение свойств и отношений [объекта userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|
|[Создание userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-create.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Создание нового [объекта userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|
|[Удаление userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md).|
|[Обновление userExperienceAnalyticsBatteryHealthAppImpact](../api/intune-devices-userexperienceanalyticsbatteryhealthappimpact-update.md)|[userExperienceAnalyticsBatteryHealthAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|Обновление свойств объекта [userExperienceAnalyticsBatteryHealthAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthappimpact.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта воздействия приложения-приложения для аналитики пользовательского интерфейса.|
|activeDevices|Int32|Количество активных устройств для использования этого приложения в течение 14 дней. Допустимые значения 2147483648 2147483647|
|appName|String|Имя приложения. Например: oltk.exe|
|appDisplayName|String|Удобное для пользователя имя отображения приложения. Например: Outlook|
|appPublisher|String|Издатель приложения. Например: корпорация Майкрософт|
|isForegroundApp|Boolean|верно, если у пользователя было активное взаимодействие с приложением.|
|batteryUsagePercentage|Double|Процент общей мощности батареи, используемой этим приложением, когда устройство не подключено к мощности переменного тока, в течение 14 дней вычисляется на всех устройствах в клиенте. Единица в процентах. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthAppImpact",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "isForegroundApp": true,
  "batteryUsagePercentage": "4.2"
}
```




