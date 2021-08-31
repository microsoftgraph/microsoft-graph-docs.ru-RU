---
title: тип ресурса userExperienceAnalyticsAppHealthDevicePerformance
description: Объект аналитики производительности устройства пользовательского интерфейса содержит сведения о производительности устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59df08aa5f6cf4b70a6c667d4bd951bc7430ebd4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58770478"
---
# <a name="userexperienceanalyticsapphealthdeviceperformance-resource-type"></a>тип ресурса userExperienceAnalyticsAppHealthDevicePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект аналитики производительности устройства пользовательского интерфейса содержит сведения о производительности устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsAppHealthDevicePerformances](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-list.md)|[коллекция userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|
|[Get userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-get.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|
|[Создание userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-create.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Создание нового [объекта userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|
|[Удаление userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).|
|[Обновление userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-update.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Обновление свойств объекта [userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности устройства для аналитики пользовательского интерфейса.|
|deviceModel|String|Имя модели устройства.|
|deviceManufacturer|Строка|Имя производителя устройства.|
|appCrashCount|Int32|Количество сбоей приложения для устройства. Допустимые значения 2147483648 2147483647|
|crashedAppCount|Int32|Количество различных сбоей приложения для устройства. Допустимые значения 2147483648 2147483647|
|appHangCount|Int32|Для устройства зависает число приложений. Допустимые значения 2147483648 2147483647|
|processedDateTime|DateTimeOffset|Дата и время последнего вычисления статистики.|
|meanTimeToFailureInMinutes|Int32|Время сбоя устройства в минутах. Допустимые значения 2147483648 2147483647|
|deviceAppHealthScore|Двойное с плавающей точкой|Оценка состояния приложения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|deviceAppHealthStatus|Строка|Общее состояние состояния здоровья приложения на устройстве.|
|deviceId|String|ID устройства.|
|deviceDisplayName|String|Имя устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "appCrashCount": 1024,
  "crashedAppCount": 1024,
  "appHangCount": 1024,
  "processedDateTime": "String (timestamp)",
  "meanTimeToFailureInMinutes": 1024,
  "deviceAppHealthScore": "4.2",
  "deviceAppHealthStatus": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```



